# Inventory Management Automation with Python & Excel

This project automates inventory analysis using Python and Excel. It reads product data from an Excel file, calculates inventory values, tracks low-stock items, and generates a summary report — all with zero manual effort.

## Features
- Counts products per supplier  
- Calculates total inventory value per supplier  
- Flags products with inventory less than 10  
- Writes inventory value back into the Excel sheet  
- Creates a summary sheet with supplier stats

## Tech Stack
- Python 3.13  
- [openpyxl](https://pypi.org/project/openpyxl/) for Excel automation  
- Excel (.xlsx) as the data source

## Installation
```bash
pip install openpyxl
```

## File Structure
- `inventory.xlsx` – Input file with product data  
- `main.py` – Python script for automation  
- `inventory_with_summary.xlsx` – Output file with updated values and summary

## Sample Excel Format
| Product # | Inventory | Price | Supplier   | Inventory Value |
|-----------|-----------|-------|------------|-----------------|
| 101       | 100       | 1.00  | Supplier A |                 |
| 102       | 5         | 0.50  | Supplier B |                 |

## Usage
Run the script:
```bash
python main.py
```

Output:
- Inventory values are written to column 5  
- A new sheet named `Summary` is created with:
  - Supplier Name  
  - Number of Products  
  - Total Inventory Value

## Sample Output (Terminal)
```python
Products per supplier: {'Supplier A': 1, 'Supplier B': 1}
Total value per supplier: {'Supplier A': 100.0, 'Supplier B': 2.5}
Products under 10 inventory: {102: 5}
```

## Why It Matters
This project demonstrates how Python can solve real-world business problems by automating repetitive tasks and generating actionable insights. It’s a great example of combining programming with practical data operations.

---

Would you like me to help you add a license, contribution guide, or GitHub badges to make it even more complete?
