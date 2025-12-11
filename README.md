Protein-Ligand Binding Affinity Analysis Script (Time-stamped)
------------------------------------------------
Description:
    This script automates the analysis of Microscale Thermophoresis (MST) 
    or similar binding affinity data. It processes CSV files in the current 
    directory, calculates binding kinetics using a one-site binding model, 
    and generates fitted plots.

    * Feature: Creates a unique output folder based on current time (HH:MM:SS)
      to prevent overwriting previous results.

    If outliers are marked in the raw data (column 'Is Outlier'), 
    the script performs analysis twice:
    1. Clean Data (Outliers excluded) - Primary Analysis
    2. All Data (Outliers included) - For validation/transparency

Author: [hanbyeonggu@gmail.com/BCK Lab]
Date: 2025-12-09
Dependencies: pandas, matplotlib, numpy, scipy
