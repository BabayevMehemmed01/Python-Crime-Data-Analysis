# Chicago Crime Data Analysis

This project cleans and explores crime incident records from the City of Chicago. It uses **Pandas** for data cleaning and exploratory data analysis (EDA), and **Matplotlib** and **Seaborn** to visualize the results.

The analysis identifies the most common crime types and shows how incidents are distributed across months, hours, and days of the week.

## Overview

The workflow is organized in a Jupyter notebook and covers two stages:

1. **Data cleaning** — inspect the raw records, handle missing values, drop columns that are not needed, standardize data types, add time-based fields, and check for duplicates.
2. **Exploratory data analysis** — summarize the dataset, rank the predominant crime types, and examine temporal patterns, arrest and domestic-incident trends, and the areas with the highest crime counts.

Time features are derived from the incident date:

- **Month**
- **Hour**
- **Day of week**

These fields are used to compare when crimes occur and to highlight the busiest periods.

## Dataset

The source data is the City of Chicago public safety dataset, [Crimes - 2001 to Present](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2/about_data).

Place the file in the project folder as `chicago_crime.csv` before running the notebook. CSV files are listed in `.gitignore`, so the data file is kept locally and is not uploaded to GitHub.

Key columns used in the analysis include case identifiers, date, primary crime type, description, location description, arrest and domestic flags, police district and community area, and geographic coordinates.

## Tech stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project structure

```text
chicago_crime/
├── 01-Chicago Crime - Python Project Activities.ipynb
├── 02-Chicago Crime - Python Project Activities Solutions.ipynb
├── chicago_crime.csv          # local only; not committed
├── .gitignore
└── README.md
```

`02-Chicago Crime - Python Project Activities Solutions.ipynb` contains the completed cleaning and EDA workflow.

## How to run

1. Clone this repository.
2. Download the Chicago crime CSV and save it in the project folder as `chicago_crime.csv`.
3. Create a virtual environment and install the required packages:

```bash
python -m venv .venv
.venv\Scripts\activate
pip install pandas numpy matplotlib seaborn jupyter
```

4. Start Jupyter and open the solutions notebook:

```bash
jupyter notebook "02-Chicago Crime - Python Project Activities Solutions.ipynb"
```

5. Run the cells from top to bottom. The notebook expects `chicago_crime.csv` in the same directory.

## What the analysis covers

- Familiarization with the raw crime records
- Missing values, unused columns, data types, and duplicate checks
- The most frequent primary crime types
- Crime counts by month, hour, and day of the week
- Arrest and domestic-incident patterns
- Districts and community areas with the highest incident counts
