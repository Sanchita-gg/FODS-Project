# EV Charging Demand and Revenue Optimization Using Machine Learning

## 1. Project Overview

Electric vehicle adoption is increasing the demand for efficient and reliable charging infrastructure. Understanding EV charging patterns is important for forecasting electricity demand, improving charging station utilisation and supporting revenue-related business decisions.

This project focuses on analysing historical EV charging data, identifying demand patterns, developing machine-learning models for charging demand prediction and presenting analytical insights through a Power BI dashboard.

The project uses the UrbanEV open benchmark dataset, which contains hourly EV charging information from different zones in Shenzhen, China.

## 2. Project Objectives

The main objectives of this project are:

- To understand and analyse historical EV charging demand patterns.
- To perform data cleaning, preprocessing and validation.
- To conduct Exploratory Data Analysis (EDA) to identify temporal and zone-wise trends.
- To develop machine-learning models for predicting future EV charging volume.
- To compare model performance using appropriate evaluation metrics.
- To analyse electricity prices, service prices and charging station utilisation.
- To visualise important findings through a Power BI dashboard.
- To generate insights that can support better operational and revenue-related decisions.

## 3. Dataset Description

The project uses the UrbanEV open benchmark dataset.

The dataset contains six major attributes:

- Charging Volume
- 11 kW Charging Volume
- Charging Duration
- Electricity Price
- Service Price
- Occupancy

The original dataset consists of hourly observations across 275 traffic zones in Shenzhen, China.

The observation period is from September 2022 to February 2023.

The six source files are integrated using time and zone ID to create a unified dataset for further analysis.

## 4. Project Methodology

The project follows these major stages:

1. Dataset Understanding and Collection
2. Data Validation and Preprocessing
3. Data Integration and Transformation
4. Exploratory Data Analysis
5. Feature Engineering
6. Machine-Learning Model Development
7. Model Evaluation and Comparison
8. Power BI Dashboard Development
9. Interpretation of Results and Business Insights

## 5. Machine-Learning Models

The following models were developed and evaluated for EV charging demand prediction:

- Baseline Lag24
- Linear Regression
- Decision Tree
- Random Forest

The models predict two targets:

- Total EV Charging Volume
- 11 kW Reference Charging Volume

## 6. Feature Engineering

The following features were created to capture temporal and historical demand patterns:

- Hour
- Day of Week
- Month
- Weekend Indicator
- Peak-Hour Indicator
- Previous Hour Demand
- Previous Day Demand
- Previous Week Demand
- 24-Hour Rolling Mean

The peak-hour indicator uses predefined time periods of 7–10 AM and 5–9 PM as a project assumption.

## 7. Model Evaluation

Model performance was evaluated using the following metrics:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R-squared (R²)

Random Forest achieved the best overall performance among the tested models for both prediction targets.

## 8. Power BI Dashboard

The Power BI dashboard presents the analytical findings through the following pages:

1. Revenue Overview
2. Electricity Tariff Analysis
3. Utilization and Demand Patterns
4. Business Insights and Optimization

The dashboard supports the interpretation of EV charging demand, electricity pricing, service pricing and utilisation patterns.

## 9. Repository Structure

EV-Charging-Demand-Revenue-Optimization/
|
|-- dashboard/
|-- models/
|-- notebooks/
|-- outputs/
|-- report/
|
|-- README.md
|-- requirements.txt

## 10. Team Contributions

The project is divided among three team members:

- Sanchita: Dataset Understanding, Data Validation, Preprocessing and Exploratory Data Analysis.
- Pawni: Machine-Learning Model Development and Demand Prediction.
- Rushpreet: Power BI Dashboard Development and Data Visualisation.

## 11. Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook
- Power BI
- GitHub
- LaTeX
- Overleaf

## 12. Project Limitations

- The dataset covers a limited observation period of six months.
- The data is aggregated at hourly and zone levels, so individual vehicle and charging-session behaviour cannot be analysed directly.
- Charging volume is estimated using charging-pile rated power and may differ from actual vehicle-side energy consumption.
- Revenue optimisation requires additional analysis of pricing strategies, charging capacity, operating costs and other constraints.

## 13. Conclusion

This project demonstrates the application of data science and machine-learning techniques to EV charging demand analysis and prediction.

By integrating historical charging data, identifying demand patterns, developing predictive models and visualising results through Power BI, the project provides insights that can support charging infrastructure planning and revenue-related business decisions.

Among the evaluated models, Random Forest achieved the best overall prediction performance for both charging-volume targets.
