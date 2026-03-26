# Quantity Analysis: Retail Demand Forecasting

## Project Overview
This project focuses on predicting future product demand using historical sales data. By leveraging Time Series Analysis and the ARIMA model, I developed a pipeline to forecast daily quantities, enabling data-driven inventory management.

## The Business Problem
Retailers often struggle with "Stockouts" (lost sales) or "Overstocking" (wasted capital). This project aims to provide a 2-year look-back analysis to predict future requirements with a measurable margin of error.

## Tech Stack
- **Language:** Python 3.10+
- **Libraries:** Pandas, Statsmodels, Matplotlib, Seaborn, Scikit-Learn
- **Model:** ARIMA (AutoRegressive Integrated Moving Average)

## Workflow & Methodology
1. **Data Cleaning:** Handled transactional data, missing dates, and extreme outliers.
2. **Stationarity Testing:** Applied the Augmented Dickey-Fuller (ADF) test ($p=0.026$) to validate the data for modeling.
3. **Decomposition:** Analyzed Trend and Weekly Seasonality.
4. **Model Tuning:** Used ACF/PACF plots to identify optimal parameters $(2, 0, 2)$.
5. **Evaluation:** Achieved a **Mean Absolute Error (MAE) of 366.33**.

## Key Results
- Identified a strong **7-day seasonal cycle**, indicating peak demand periods.
- The model successfully follows the general sales trend, providing a reliable baseline for procurement teams.

## How to Run
1. Clone the repo: `git clone https://github.com/yourusername/retail-demand-forecasting-arima.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebook in the `notebooks/` folder.

---
*Developed during my Data Science Internship at @Skillfied Mentor.*
