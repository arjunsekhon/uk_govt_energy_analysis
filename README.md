# Supply and Use of Crude Oil and Natural Gas Liquids from UK Government Website

## Installation and Running the Project

Install Poetry (if not already installed):

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

To launch Jupyter Lab within the Poetry virtual environment, run:

```bash
poetry install --no-root
poetry run jupyter lab
```

If additional dependencies are required, add them with:

```bash
poetry add seaborn
```

## Jupyter Notebook: Energy Data Analysis

I have prepared a Jupyter Notebook to walk through the **data cleaning** and **exploratory analysis** steps.  

- **View the notebook:** [energy_analytics.ipynb](./energy_analytics.ipynb)  
- **Cleaned CSV data:** [cleaned_energy_data.csv](./cleaned_energy_data.csv)

### Why Scrape JSON‑LD?

The UK Government website embeds structured metadata in JSON‑LD, which offers key benefits:

- **Reliability:** The structured format is less prone to breaking with changes in the DOM.
- **Simplicity:** Data extraction is straightforward, as key information is provided in a standard format.
- **Consistency:** Ensures uniform formatting for download URLs and document metadata.

### Notebook Contents

- **Data Ingestion & Cleaning:** Demonstrates how the raw spreadsheet is downloaded (via JSON‑LD extraction), cleaned and converted to a tidy, long format.
- **Exploratory Data Analysis (EDA):** Contains visualisations and statistics to understand trends, seasonal patterns, supply-demand balance and inventory dynamics.
- **Key Insights:** Summaries of market indicators, correlations and outlier detection to inform trading strategies.
