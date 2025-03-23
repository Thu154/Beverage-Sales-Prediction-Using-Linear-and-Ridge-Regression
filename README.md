Objective
The goal of this project is to develop and evaluate machine learning models to predict beverage sales based on key influencing factors such as temperature and promotional activity. The project explores the relationship between these factors and beverage sales using both Linear Regression and Ridge Regression to identify the best predictive model.

Dataset Overview
The dataset, downloaded from Kaggle (victoriajabdulkadir/beverage-sales-prediction), includes the following key features:

Temperature (°C): The daily temperature in degrees Celsius.
Promotion: A binary value (0 or 1) indicating whether a promotional activity was conducted on that day.
Beverage Sales: The total number of beverage sales on that day (target variable).
Project Workflow
Data Loading and Cleaning
The dataset is downloaded using the Kaggle API and read into a Pandas DataFrame.
The dataset is inspected for structure and missing values.
Exploratory Data Analysis (EDA)
Histograms are plotted for each feature to understand their distribution.
A correlation matrix is generated to identify relationships between features.
An interaction term (Temp_Promo) is created by multiplying Temperature (°C) and Promotion to capture any combined effect.
Feature Engineering
Independent variables (X) include Temperature (°C), Promotion, and the interaction term Temp_Promo.
Dependent variable (y) is Beverage Sales.
Data is split into training and testing sets (80% train, 20% test).
Modeling
Linear Regression:
A baseline model using Linear Regression is fitted to the training data.
The model is evaluated using Mean Squared Error (MSE) and R-squared (R²) score.
Ridge Regression:
A Ridge Regression model is tuned using Grid Search Cross-Validation to optimize the regularization parameter (alpha).
The best model is selected and evaluated using MSE and R² score.
Results and Evaluation
Predictions from both models are plotted against the actual values.
Performance comparison between Linear and Ridge models is conducted based on error metrics and R² values.
Conclusion and Next Steps
Identified which model performs better in predicting beverage sales.
Suggested improvements such as adding more features (e.g., weather conditions, holiday effects) or using more advanced models (e.g., Lasso Regression, Decision Trees).
Technologies and Tools
✅ Python
✅ Pandas
✅ Matplotlib
✅ Seaborn
✅ Scikit-learn
✅ Kaggle API
Outcome
Established a baseline model with Linear Regression.
Improved predictive performance using Ridge Regression with hyperparameter tuning.
Identified the interaction effect between temperature and promotion as a significant factor influencing beverage sales.
Potential Improvements
Include more features such as humidity, day of the week, and competitors' promotions.
Try more complex models such as Gradient Boosting or Neural Networks.
Fine-tune Ridge model with different cross-validation strategies.

