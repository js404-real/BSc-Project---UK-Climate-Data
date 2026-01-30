# BSc-Project---UK-Climate-Data

## About The Project
This repository contains the code and analysis for my BSc Physics project. The primary aim is to investigate climate trends in the United Kingdom using the ERA5 reanalysis dataset from ECMWF.

The project compares **Classical Statistical Methods** (linear regression, trend analysis) against **Machine Learning techniques** to analyse temperature changes over recent decades.

## Key Objectives
* **Data Processing:** Handling multidimensional NetCDF climate data (Time, Latitude, Longitude).
* **Classical Analysis:**
    * Spatial averaging of UK grid points.
    * Temporal averaging (Monthly and Annual aggregation).
    * Comparison of 2-metre Air Temperature (`t2m`) vs. Soil Temperature Level 1 (`stl1`).
    * Linear curve fitting to quantify warming rates per decade.
* **Machine Learning (In Progress):** Applying ML models to predict future trends or identify non-linear patterns.

## Data Source
The data is sourced from the **ECMWF ERA5 Reanalysis** dataset.
* **Format:** NetCDF (`.nc`).

> **Note:** The code includes handling for ERA5 `expver` coordinates, merging Consolidated (final) and Preliminary (real-time) data streams automatically.

## Repository Structure
* `notebooks/` - Jupyter Notebooks containing the main analysis and visualizations.
* `scripts/` - Python scripts for data cleaning or batch processing.
* `plots/` - Generated figures and temperature trend graphs.

## Getting Started

### Prerequisites
The analysis relies on the standard Python scientific stack. You can install the dependencies via pip:

```bash
pip install xarray netCDF4 matplotlib numpy scipy cartopy
