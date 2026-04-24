# BEPS Applied Energy Replication Package

This repository contains the replication materials for the paper:

**“Building Energy Performance Standards: Impacts on Building Energy Efficiency and GHG Emissions in Washington, DC”**

The repository provides the raw data, Python code, and documentation required to reproduce the analytical dataset, empirical results, tables, and figures presented in the manuscript.

---

## Repository Structure

```text
/data_raw
    Raw benchmarking and climate datasets

/data_clean
    Intermediate and final cleaned datasets generated from the replication code

/code
    Master Python replication script for data cleaning, variable construction,
    econometric estimation, robustness checks, tables, and figures

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
- matplotlib
- scipy
- linearmodels

Install required packages using:

```bash
pip install -r requirements.txt
```

---

## Replication Instructions

### Step 1: Download Raw Data
Place all raw datasets into the `/data_raw` folder.

### Step 2: Run the Master Replication Script
Run the master Python script located in the `/code` folder:

```text
master_replication.py
```

The script performs the following tasks sequentially:

- data cleaning and validation,
- harmonization of property categories,
- construction of treatment intensity measures,
- merging of climate variables,
- descriptive statistics,
- econometric estimation,
- event-study analysis,
- robustness checks,
- and generation of all tables and figures presented in the manuscript.

### Step 3: Output Files
Replicated tables and figures will be automatically saved in:

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
