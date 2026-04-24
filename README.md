# BEPS Applied Energy Replication Package

This repository contains the replication materials for the paper:

**“Building Energy Performance Standards: Impacts on Building Energy Efficiency and GHG Emissions in Washington, DC”**

The repository provides the raw data, Python scripts, and documentation required to reproduce the analytical dataset, empirical results, tables, and figures presented in the manuscript.

---

## Repository Structure

```text
/data_raw
    Raw benchmarking and climate datasets

/data_clean
    Intermediate and final cleaned datasets generated from the scripts

/code_cleaning
    Python scripts for data cleaning, merging, recoding, and variable construction

/code_analysis
    Python scripts for descriptive analysis, econometric estimation, robustness checks, tables, and figures

/output_tables
    Replicated tables from the manuscript

/output_figures
    Replicated figures from the manuscript
```

---

## Data Sources

The analysis uses publicly available data from the following sources:

1. Open Data DC Benchmarking Dataset  
   Source: https://opendata.dc.gov/

2. Degree Days Climate Data (CDD/HDD)  
   Source: https://www.degreedays.net/

Please refer to the manuscript and source documentation for additional details regarding data definitions and reporting standards.

---

## Software Requirements

All analyses were conducted in Python.

Recommended environment:

- Python 3.11+
- pandas
- numpy
- statsmodels
- linearmodels
- matplotlib
- seaborn
- scipy
- geopandas (if spatial analysis is included)

Install required packages using:

```bash
pip install -r requirements.txt
```

---

## Replication Instructions

### Step 1: Download Raw Data
Place all raw datasets into the `/data_raw` folder.

### Step 2: Run Data Cleaning Scripts
Run the scripts in `/code_cleaning` in the following order:

```text
01_data_cleaning.py
02_variable_construction.py
03_gap_construction.py
```

These scripts:
- clean and validate benchmarking records,
- harmonize property categories,
- construct treatment intensity measures,
- merge climate variables,
- and generate the final analytical dataset.

### Step 3: Run Main Analysis
Run the scripts in `/code_analysis`:

```text
04_descriptive_analysis.py
05_main_regressions.py
06_event_study.py
07_robustness_checks.py
```

These scripts reproduce:
- descriptive statistics,
- baseline regressions,
- event-study estimates,
- robustness checks,
- tables,
- and figures presented in the paper.

### Step 4: Output Files
Replicated tables and figures will be saved automatically in:

```text
/output_tables
/output_figures
```

---

## Notes

- All data cleaning procedures follow the data dictionary and user guidance provided by the original data sources.
- The repository is designed to provide full computational reproducibility of the published results.
- File paths may need adjustment depending on the user’s local directory structure.

---

## Citation

If using these materials, please cite:

Gbadegesin, T. (2026). *Replication package for “Building Energy Performance Standards: Impacts on Building Energy Efficiency and GHG Emissions in Washington, DC”*. Zenodo. [DOI LINK]
