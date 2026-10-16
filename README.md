# UK Grocery Sales Analysis

Data cleaning and exploratory analysis of 8,000+ UK grocery transactions (2024–2025) using Python.

## Tools
Python · pandas · NumPy · matplotlib · Jupyter

## Data cleaning
- Removed 150 duplicate rows
- Converted prices stored as text (£1.54) to numbers
- Standardised 4 date formats (ISO, UK, US, text); resolved ambiguous UK/US dates using other lines of the same transaction
- Fixed 83 impossible quantities (-1, 0, 99) by reverse-calculating from price, discount and sales
- Filled missing cities from store IDs and missing prices/sales using the sales formula

## Key findings
- Total revenue £31,370 from 2,282 orders (average order £13.75)
- Sales peak in November–December and drop sharply in January
- Revenue differences between categories come from price, not volume
- Two daily peaks: lunchtime (12:00) and after work (16:00–18:00)
- Multibuy "3 for 2" is the most efficient promotion (14p discount per £1 of sales)
- Frozen has the highest refund rate (5.8%)

## Files
- `grocery_sales_analysisis.ipynb` – full analysis notebook
- `uk_grocery_sales_raw.csv` – original data
- `uk_grocery_sales_clean.csv` – cleaned data
