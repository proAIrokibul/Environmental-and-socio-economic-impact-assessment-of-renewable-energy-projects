# Environmental and Socio-Economic Impact Assessment of Renewable Energy Projects

## Project Overview
This project aims to assess the environmental and socio-economic impacts of renewable energy projects using machine learning models. The focus is on predicting CO2 emissions based on various factors such as energy production, investments, population, GDP, and other relevant variables. This analysis can provide insights for policymakers and stakeholders in the renewable energy sector.

## Dataset
The dataset used in this project includes various features related to renewable energy, such as:
- **Country**: The name of the country.
- **Year**: The year of the data.
- **Energy Type**: The type of renewable energy.
- **Production (GWh)**: The energy produced in gigawatt-hours.
- **Installed Capacity (MW)**: The installed capacity in megawatts.
- **Investments (USD)**: Financial investments in renewable energy projects.
- **Population**: Population statistics.
- **GDP**: Gross Domestic Product.
- **Energy Consumption**: Total energy consumption.
- **CO2 Emissions**: The target variable for prediction.

## Methodology
1. **Data Preprocessing**:
   - The dataset was cleaned and unnecessary columns were dropped.
   - Missing values were identified and handled appropriately.
   - The dataset was split into features (X) and target variable (y).

2. **Modeling**:
   - Three machine learning models were implemented:
     - Linear Regression
     - Random Forest Regressor
     - XGBoost Regressor
   - The dataset was further split into training and testing sets to evaluate model performance.

3. **Evaluation**:
   - Models were evaluated based on Mean Squared Error (MSE) and R² score.

## Results
The results from the models are as follows:

| Model              | Mean Squared Error (MSE) | R² Score      |
|--------------------|---------------------------|---------------|
| Linear Regression   | 0.999657                  | -0.012188     |
| Random Forest       | 1.023255                  | -0.036081     |
| XGBoost             | 1.110665                  | -0.124587     |

### Model Comparison
- **Linear Regression**: 
  - MSE: 0.999657
  - R²: -0.012188
  - The linear regression model showed the best performance among the three, with the lowest MSE, indicating its predictive capability.

- **Random Forest**:
  - MSE: 1.023255
  - R²: -0.036081
  - The random forest model performed slightly worse than the linear regression model, suggesting that it did not generalize well to the test data.

- **XGBoost**:
  - MSE: 1.110665
  - R²: -0.124587
  - The XGBoost model had the highest MSE, indicating that it struggled to predict CO2 emissions effectively based on the input features.

Overall, all models exhibited poor predictive performance as indicated by negative R² scores, suggesting that the features may not be sufficiently informative for predicting CO2 emissions or that further feature engineering is required.

## Conclusion
This analysis highlights the complexity of predicting CO2 emissions in relation to renewable energy projects. Future work should explore additional data sources, feature engineering, and potentially other machine learning algorithms to improve prediction accuracy.

