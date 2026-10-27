# Airbnb Data Analytics & Market Analysis

This project provides an end-to-end data analytics workflow on Airbnb listing and calendar data using standard Python data science libraries (`pandas` and `matplotlib`).

## Key Project Steps & Architecture

1. Data Cleaning & Type Casting
   - Stripped currency symbols (`$`) and comma separators from `price` fields.
   - Converted temporal columns (`date`) to datetime objects.
   - Encoded availability flags (`available` == 'f') into a binary integer field (`isbooked`).

2. Exploratory Data Analysis (EDA) & Visualizations
   - Price Distributions: Boxplots and Histograms for outlier and variance checks.
   - Host Dynamics: Horizontal bar plots of top-performing hosts by listing volume.
   - Demand Drivers: Scatter plots evaluating price versus review count.
   - Behavioral Indicators: Availability vs. minimum night requirements.
   - Correlation Matrix: Heatmaps analyzing feature relationships.

3. Benchmarking Analysis
   - Evaluated individual listing prices against their respective neighborhood median values (`transform('median')`).
   - Grouped neighborhood-level statistics (count, mean, median, min, max).

4. Temporal & Trend Analysis
   - Merged listing and calendar datasets across datetime dimensions.
   - Computed monthly average price variations across individual neighborhoods using grouped aggregations and pivot matrices.

## Tech Stack
- Python 3.x
- Pandas
- Matplotlib
