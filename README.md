# Practical-Application-Assignment-11.1
Predictive modeling project analyzing 426K used car listings to identify the key factors influencing vehicle price. Includes extensive data cleaning, feature engineering, exploratory analysis, and implementation of multiple regression techniques (Linear, Polynomial, Ridge, and Lasso), following the full CRISP-DM workflow.

**UC Berkeley Executive Education – Machine Learning and Artificial Intelligence Program**  
**Author:** Jonathan O’Dea  
**Date:** November 2025 

**Overview**
This project analyzes a dataset of 426,000 used vehicles to understand which factors most influence their selling price. Following the CRISP-DM methodology, this notebook moves through the full analytical workflow: defining the business need, examining the dataset, preparing and cleaning the data, building regression models, and summarizing the results. The goal is to provide a fictional used-car dealership with a model that can help them easily evaluate the resale value of a used car based different vehicle attributes.

**Objective**
The objective of this assignment is to identify the vehicle attributes that have the strongest impact on used car prices and to build models capable of estimating price using those key variables. Through a combination of data cleaning, exploratory analysis, and regression modeling (Linear, Polynomial, Ridge, and Lasso), the project aims to quantify how price varies with factors such as vehicle age, mileage, and manufacturer. The final outcome is a set of practical insights and a predictive model that the dealership can use to support pricing decisions.

**Dataset**
The dataset, vehicles.csv, contains 426,000 used car listings with fields such as year, manufacturer, model, odometer, title status, drive, fuel, cylinders, and price. It is a reduced version of a larger Kaggle dataset originally containing about 3 million listings. The raw CSV was not modified directly; all cleaning and processing were done inside this notebook.

**Notebook Structure**
This notebook, Practical_Assignment_11.1_Jonathan_O'Dea.ipynb, includes the following sections:

1. Business Understanding
2. Data Understanding
3.Initial assumptions
4. Data Preparation
5. Exploratory Data Analysis (EDA)
6. Modeling
- Simple and Multiple Linear Regression
- Polynomial Regression
- Ridge Regression (L2)
- LASSO Regression (L1)
7. Evaluation
8. Deployment
9. Findings & Recommendations

**Summary of Findings**
Based on this dataset and the cleaning applied to it, this analysis shows that the price of a used car can be driven by three factors: age, mileage, and manufacturer. Newer cars and cars with lower mileage consistently sell for more, and brands with stronger reputations tend to hold their value better.

Using these features, the Ridge Regression model with degree-4 polynomial features provided the most accurate predictions, estimating prices within roughly ±$5.6K on average (MAE). While the model performs well with the available data, more detailed information (such as model trim level, engine type, and condition) would improve accuracy further.

**Actionable Ideas for the Client**
Prioritize vehicles that are newer and have lower mileage, as these factors most reliably increase resale value.
Highlight brand reputation when pricing or marketing vehicles.

**Next Steps for Future Modeling**
Clean the model column further to extract trim level details, body style, and engine.
Incorporate vehicle condition if a reliable subset of the data can be validated.
Repeat categorical encoding for drivetrain, fuel type, and transmission as was done with manufacturer.

**How to Run**
1. The public project repository can be located at: https://github.com/Jonny802/Practical-Application-Assignment-11.1
2. Download the project file Practical_Assignment_11.1_Jonathan_O'Dea.ipynb and vehicles.csv csv locally
3. The dataet should be located in /data locally
4. Run cells top-to-bottom.
