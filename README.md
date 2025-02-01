# Interactive Visual Analytics for Disease Mortality

## Overview
This project provides an **interactive visualization and forecasting system** for COVID-19, pneumonia, and influenza-related deaths across U.S. states. Try it out!

- Explore **weekly death trends** across multiple years
- Compare **relative mortality rates** between states
- Analyze **historical data** and extract insights
- Forecast future deaths using **Auto ARIMA** time series modeling

The system is built with **Streamlit**, **Plotly**, and **Pmdarima**, for an intuitive and interactive user interface.

## Features
### 1. **Comparing Weekly Death Trends Across Years**
   - Displays **yearly mortality trends** by disease (COVID-19, Pneumonia, Influenza)
   - Allows selection of a specific **state** and **cause of death**
   - Uses **color-coded** trends for intuitive comparison

### 2. **Following Weekly Death Trends by State**
   - Provides a detailed **time-series visualization**
   - Enables **interactive filtering** by state and disease
   - Includes a **time-slider** for better focus on specific periods

### 3. **Comparing Relative Death Counts Across States**
   - Shows **percentage breakdowns** of disease-related deaths
   - Supports filtering by **month, year, and up to 5 states**
   - Uses **stacked bar charts** for clear visual comparisons

### 4. **Forecasting Disease-Related Deaths**
   - Uses **Auto ARIMA modeling** to predict future trends
   - Provides **95% confidence intervals** for uncertainty estimation
   - Adjustable forecasting window (1 to 52 weeks)

## Dataset
The dataset is sourced from the **Centers for Disease Control and Prevention (CDC)**:
[Provisional COVID-19 Death Counts by Week Ending Date and State](https://data.cdc.gov/NCHS/Provisional-COVID-19-Death-Counts-by-Week-Ending-D/r8kw-7aab/about_data).

It contains **17.5k records**, covering weekly mortality data for **COVID-19, Pneumonia, and Influenza** across U.S. states since **2020**.

## Installation & Setup
### **1. Create and Activate the Conda Environment**
```bash
conda env create -f environment.yml
conda activate tu_mdg
```

### **2. Run the Streamlit App**
```bash
streamlit run app.py
```
- The app will launch in your default browser.
- If not redirected automatically, use the **Local URL** displayed in the terminal.

## Running Jupyter Notebooks in PyCharm
1. Open a **Jupyter Notebook (`.ipynb`)** in PyCharm.
2. Execute the **first cell** (to load all imports).
3. **Avoid running multiple notebooks simultaneously** (PyCharm may crash the Jupyter server).
4. Restart the Jupyter server if needed:
   - **Stop** the server (Red Stop Button in PyCharm's Jupyter tab).
   - **Restart** it (Green Start Button), then rerun your notebook.

## Technologies Used
- **Python**
- **Streamlit** (Web App Framework)
- **Pandas** (Data Processing)
- **Plotly** (Interactive Graphs & Visualizations)
- **Pmdarima** (Auto ARIMA Time Series Modeling)
- **Statsmodels** (Statistical Analysis)
- **Matplotlib** (Basic Data Visualization)

## Insights & Findings
- **COVID-19 and Pneumonia deaths peaked in Winter 2020-2022.**
- **Seasonal trends** indicate a rise in mortality during winter months.
- **Co-morbidity analysis** suggests a correlation between pneumonia and COVID-19 deaths.
- **Forecasting models indicate potential spikes in pneumonia-related deaths** in early months of the year.

## Authors
- **Anton Zamyatin**
- **Hannah Teis**

## License
This project is licensed under the MIT License. See `LICENSE` for details.

