# RFM Customer Segmentation (Retail Analytics)

This project performs Recency–Frequency–Monetary (RFM) analysis to segment customers and produce BI‑ready tables and visuals. It includes data preparation, RFM scoring, rule‑based segment mapping, and export of results for dashboards.

## Project Contents
- **rfm_analysis_project.ipynb** — Jupyter Notebook: data prep, RFM scoring, segment mapping, and visualization.
- **sample-orders (rfm).csv** — Example transactions data used as input (orders with CustomerID, InvoiceDate, Quantity/Amount).
- **rfm-table.csv** — Customer‑level R, F, M features and scores.
- **rfm-segmentation.csv** — Final segments per customer (e.g., Loyal, At Risk).
- **rfm_for_bi.csv** — BI‑ready wide table for reporting dashboards.
- **requirements.txt** — Python dependencies.

## Features
- Compute Recency (days since last purchase), Frequency (order count), and Monetary (revenue).
- Score customers (e.g., quintiles) and derive segments via rule‑based mapping (e.g., Loyal, At Risk).
- Visualize distribution of R, F, M and segment composition.
- Export CSVs for BI tools (e.g., Power BI, Tableau, Google Data Studio).
- Optional interactivity via ipywidgets and Plotly.

## Technology Stack
- Python, Jupyter Notebook
- pandas, numpy
- scikit‑learn (optional utilities)
- matplotlib, seaborn, plotly
- ipywidgets (optional)

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
3. Open `rfm_analysis_project.ipynb` and run all cells. Update the input path to your transactions CSV if different.

## Outputs
- `rfm-table.csv`: base R, F, M features and scores per customer.
- `rfm-segmentation.csv`: customer segment labels (e.g., Loyal, At Risk).
- `rfm_for_bi.csv`: consolidated, BI‑ready export.
- Plots showing segment distribution and R/F/M histograms.

## Notes
- The included CSVs are samples for demonstration. Replace with your organization’s data as needed (ensure columns for customer ID, transaction date, and amount exist).
