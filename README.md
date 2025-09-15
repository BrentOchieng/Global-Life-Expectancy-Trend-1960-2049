# Global-Life-Expectancy-Trend-1960-2049

This project analyzes global life expectancy data from **1960 to 2023** and projects future trends using statistical forecasting. The goal is to uncover how life expectancy has evolved across different regions, highlight major patterns and disruptions, and demonstrate the use of data wrangling, visualization, and forecasting techniques in a reproducible workflow.
----
Data -source:https://data.worldbank.org/indicator/SP.DYN.LE00.IN?locations=KE						
<img width="575" height="21" alt="image" src="https://github.com/user-attachments/assets/ef68d21c-4dee-47c8-906f-7fcd9d3c06aa" />

---

## Project Overview
The notebook takes you through a full data-analysis pipeline:
1. **Data Loading & Cleaning:**  
   - Import life expectancy data in wide format (countries as rows, years as columns).
   - Handle missing values and ensure correct data types.

2. **Reshaping & Transformation:**  
   - Convert the dataset to long format (one row per country-year) using `pandas.melt()`.  
   - Create a datetime column for time-series analysis and modeling.

3. **Exploratory Data Analysis (EDA):**  
   - Plot global, continental, and country-level life expectancy trends.  
   - Focused examples include **America** (steady growth with a sharp dip in 2020–21) and **East Africa** (long-term gains with more variability).  
   - Compute mean regional life expectancy for custom groups (e.g., East African countries).

4. **Forecasting with Prophet:**  
   - Prepare Europe’s average life expectancy as a time series.
   - Fit a **Prophet** model to capture the trend.
   - Generate forecasts up to 2049 with prediction intervals to show uncertainty.

5. **Visualization & Insights:**  
   - Clear, well-labeled plots show historical patterns, regional differences, and forecasts.
   - Highlight global health improvements and disruptions (e.g., COVID-19 pandemic effects).

---

## Key Insights
- **Global Upward Trend:** Life expectancy has increased consistently across most countries since 1960, reflecting better healthcare, sanitation, and living conditions.
- **Europe:** From ~68 years (1960) to ~80 years (2020). Forecasts suggest continued growth to ~82–84 years by 2049.
- **America:** Steady growth to ~75 years by 2023, but a notable drop in 2020–2021 (pandemic impact) followed by partial recovery.
- **East Africa:** Gains are clear but more gradual, with life expectancy remaining lower than the global average — a sign of continued health challenges but also progress.

---

## Technologies & Libraries
- **pandas**, **numpy** — data wrangling and cleaning  
- **matplotlib**, **seaborn** — visualizations and trend plots  
- **prophet** — time-series forecasting  
- **jupyter notebook** — interactive environment for reproducible analysis
- **country Converter**-Grouping Countries into Continents

---


