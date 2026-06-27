# Multi-Currency Revenue Reporter
Aggregates realized hotel revenue (Completed bookings only) in INR and converts to USD using Frankfurter historical FX rates — not today's spot rate.
Place `hotel_bookings.csv` in the project root, then run `jupyter notebook multi_currency_revenue_reporter.ipynb` or `python multi_currency_revenue_reporter.py`.
Install dependencies with `pip install -r requirements.txt` (Python 3.10+ required).
Outputs are saved to the `outputs/` folder: merged CSV, Chart 1 (INR trend), Chart 2 (USD vs INR dual-axis), and console insight summary.
Key finding: FX adjustment reveals the gap between reported INR revenue growth and real USD-equivalent growth — invisible from the bookings dataset alone.
