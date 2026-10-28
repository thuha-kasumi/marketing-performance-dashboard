# Marketing Performance Dashboard

Final course project for **BAN 601 (Python fundamentals)**. The live app retains
its original title, **Digital Marketing Performance Auditor**.

An interactive Streamlit dashboard for exploring marketing campaign data with
filters, visualizations, and descriptive statistics. Inspect metric
distributions and pairwise relationships without writing code.

[Open the live demo](https://digital-marketing-performance-auditor-thuhakasumi.streamlit.app/)

## Features

- Upload campaign data in **CSV format**.
- Optionally filter the data by one categorical column and value.
- Select numeric columns as KPIs for analysis.
- View individual KPI distributions with histograms or explore pairwise
  relationships with a pairplot.
- Review descriptive statistics for the selected metrics, including count,
  mean, standard deviation, minimum, quartiles, and maximum.

## Input data

Use a CSV with a header row and at least one numeric column. The dashboard
detects available columns; it does not require specific KPI names.

For example:

```csv
Campaign,Region,Spend,Clicks,Conversions
Campaign A,West,1200,350,22
Campaign B,East,950,280,18
```

Excel workbooks (`.xlsx`) are not supported directly. Save the relevant sheet
as CSV before uploading it.

## Run locally

Clone this repository and open its directory. With Python installed, install
the dependencies:

```bash
python -m pip install -r requirements.txt
```

Start the dashboard:

```bash
python -m streamlit run app.py
```

Upload a CSV, choose any available filters, select at least one numeric KPI,
and choose a plot type from the sidebar.

## Tools

Python, Streamlit, pandas, Seaborn, and Matplotlib.
