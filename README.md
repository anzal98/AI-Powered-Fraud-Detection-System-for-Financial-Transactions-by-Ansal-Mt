# Financial Transaction Fraud Detection

This Jupyter Notebook provides a Thorough guide to detecting fraudulent financial transactions using a Random Forest Classifier. The notebook is structured into several sections, each focusing on a specific aspect of the data analysis and model building process. Please note that the data used for this model is synthetically created through Python, and there may be small possibilities of issues. This project is a concept prototype and not intended for production use.

We begin by importing essential Python libraries such as pandas and numpy for data manipulation and numerical computations, matplotlib and seaborn for visualizations to understand the dataset, and sklearn for data preprocessing, model training, and evaluation.

Next, we load and explore the synthetic financial transaction data. This involves inspecting the dataset structure, column types, and summary statistics, checking for missing values to ensure data integrity, and displaying the first few rows for an overview of the dataset.

To understand the data better, we visualize it by comparing the number of fraudulent and non-fraudulent transactions using a count plot and examining how transaction amounts vary for fraudulent and non-fraudulent transactions with a histogram and KDE plot.

In the preprocessing stage, we convert categorical columns (MerchantCategory, TransactionType) to numerical values using LabelEncoder, split the dataset into features (X) and the target variable (y), normalize numerical data using StandardScaler for consistent model performance, and divide the data into training and testing sets for model evaluation.

We then train the model using a Random Forest Classifier, a robust machine learning algorithm for detecting fraud. The model is trained on the training dataset to learn patterns and evaluated on the test dataset using a classification report.

Model performance is evaluated by visualizing predictions against actual outcomes with a confusion matrix to identify true positives, true negatives, false positives, and false negatives, and analyzing the model’s ability to distinguish between classes using the Receiver Operating Characteristic (ROC) curve.

For deployment, we save the trained Random Forest model and the data scaler using joblib to ensure consistent preprocessing during deployment. We also load the saved model and make sample predictions to verify its functionality.

Finally, we visualize insights by analyzing fraud percentages across different merchant categories to identify high-risk areas and examining fraud rates for various transaction types to gain deeper insights into patterns.
