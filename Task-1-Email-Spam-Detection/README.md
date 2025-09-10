This Python script is designed to build and evaluate a machine learning model for email spam detection. It uses a Logistic Regression classifier with a focus on optimizing its performance for identifying spam emails.

1. Data Preparation and Cleaning
The code begins by loading an email spam dataset (emailspam.csv). It renames the columns to 'label' and 'text' and converts the categorical labels ('ham', 'spam') into numerical values (0 and 1) for model training.

2. Data Splitting and Feature Extraction
The dataset is split into training and testing sets using a 80/20 ratio. To prepare the text data for the model, a TF-IDF Vectorizer is used. This process converts the email text into numerical feature vectors by giving more weight to words that are important and rare across the dataset, such as "free" or "offer," which are often found in spam emails.

3. Model Training and Optimization
A Logistic Regression model is trained on the vectorized data. The model is configured with class_weight='balanced' to handle the potential class imbalance between ham and spam emails. After training, the model predicts the probability of each email in the test set being spam.

4. Threshold Tuning
This is a critical step where the script optimizes the classification threshold. Instead of using the default 0.5 threshold, it tests different values (from 0.30 to 0.60). For each threshold, it calculates the F1-Score for spam emails. The F1-Score is a better metric than accuracy for imbalanced datasets as it considers both precision and recall. The goal is to find the threshold that yields the highest F1-Score for spam detection.

5. Final Evaluation and Visualization
Once the best threshold is found, the script applies it to the test set to make the final predictions. It then prints the performance metrics—accuracy, recall, and F1-Score—for the selected threshold. Finally, it generates and saves a confusion matrix  as a heatmap, providing a visual summary of the model's true positives, true negatives, false positives, and false negatives. This visualization helps to understand where the model is succeeding and where it's making errors.
