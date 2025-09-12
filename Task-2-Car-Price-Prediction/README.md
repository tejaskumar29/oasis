This Python script performs car price prediction using a Random Forest Regressor machine learning model. The process involves a full data science pipeline, from data preparation to model evaluation and visualization.

1. Data Loading and Preprocessing
The script loads a dataset named car data.csv. It then performs feature engineering by creating a new Car_Age feature from the Year column, as the age of a car is a stronger predictor of its price than the year of manufacture. The original Year and Car_Name columns are dropped. To prepare the categorical data (Fuel_Type, Selling_type, Transmission) for the model, a LabelEncoder is used to convert them into numerical values.

2. Model Training
The processed data is split into training and testing sets with an 80/20 ratio. A Random Forest Regressor model is initialized with 200 estimators and trained on the training data. This type of model is well-suited for regression tasks and is known for its ability to handle complex, non-linear relationships between features and the target variable (selling price).

3. Evaluation and Visualization
After training, the model's performance is evaluated using the test data. The script calculates and prints two key metrics:

R² Score: A measure of how well the model's predictions match the actual values. An R² score close to 1 indicates a good fit.

Root Mean Squared Error (RMSE): A measure of the average difference between the predicted and actual values. A lower RMSE indicates better model accuracy.

Finally, the script generates a scatter plot of the actual selling prices versus the predicted prices. This visual representation provides a clear way to see how closely the model's predictions align with the real-world data, with points clustered along a diagonal line indicating high accuracy. The plot is saved to the Task-2-Car-Price-Prediction/results directory.
