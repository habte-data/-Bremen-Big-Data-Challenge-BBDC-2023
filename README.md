# **Bremen Big Data Challenge (BBDC) 2023**  

## **Overview**  
This repository contains our work on the **Bremen Big Data Challenge 2023 (BBDC 2023)**. The goal of the challenge is to develop a **forecasting model** for water sample measurements collected by the **Alfred-Wegener-Institut** near Helgoland (North Sea). The dataset spans **54 years (1962–2015)** and includes multiple environmental factors.  

## **Dataset Description**  
- **Time Period:** 01.01.1962 - 31.12.2015  
- **Data Source:** Alfred-Wegener-Institut  
- **Measurement Values:**  
  - SECCHI (water transparency)  
  - Temperature  
  - Salinity  
  - NO₂ (Nitrite)  
  - NO₃ (Nitrate)  
  - NOₓ (Total Nitrogen Oxides)  
- **Challenges:**  
  - Missing values (`NA`) and uncertain values (`?`)  
  - Data formatted with English decimal separators (`.` for decimals, `,` for thousands)  

## **Forecasting Task**  
- Develop a predictive model based on historical data.  
- Predict values for two evaluation periods:  
  - **2004 (01.01.2004 - 31.12.2004)**  
  - **2011-2013 (01.01.2011 - 31.12.2013)**  
- Predictions must be submitted in the provided **"bbdc_2023_AWI_data_evaluate_skeleton.csv"** file.  

## **Evaluation Metric**  
- **Root Mean Squared Error (RMSE)**  
- Data will be **Z-normalized** before RMSE calculation to ensure consistency across different variable scales.  

## **Preprocessing Steps**  
1. **Handle Missing and Uncertain Values**  
   - Remove or impute missing values (`NA`).  
   - Handle uncertain values marked with `?`.  

2. **Feature Engineering**  
   - Convert date and time into structured features.  
   - Normalize numeric data for better model performance.  

3. **Exploratory Data Analysis (EDA)**  
   - Visualize trends over time.  
   - Identify seasonality and anomalies.  
