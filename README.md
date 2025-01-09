Credit Card Fraud Detection using Machine Learning
This project implements a machine learning-based fraud detection system using logistic regression to predict fraudulent credit card transactions. The dataset used for training and testing the model contains anonymized credit card transaction data, with features representing transaction details and the target variable (Class) indicating whether a transaction is legitimate (0) or fraudulent (1).

Key Steps in the Project:
Data Loading:

The project begins by loading the credit card transaction data into a Pandas DataFrame from a CSV file.
Data Preprocessing:

The dataset is cleaned by dropping rows with missing values.
The features are scaled using StandardScaler to improve the performance of the logistic regression model.
Data Exploration:

The distribution of legitimate and fraudulent transactions is analyzed.
Statistical measures like mean, median, and standard deviation are computed for the transaction amounts.
The data is balanced by randomly sampling an equal number of legitimate and fraudulent transactions to avoid class imbalance.
Feature Engineering:

The Class column (target variable) is separated from the features, and the data is split into training and test sets using an 80-20 split.
Model Training:

Logistic Regression is used as the machine learning algorithm to build the model.
The model is trained on the scaled training data.
Hyperparameters such as max_iter are adjusted to ensure convergence during training.
Model Evaluation:

The model's accuracy is evaluated on both the training and test sets using accuracy_score.
The results are compared to assess the model’s performance in identifying fraudulent transactions.
Key Libraries Used:
Pandas: For data manipulation and analysis.
NumPy: For numerical operations.
Scikit-learn: For building and evaluating the logistic regression model, as well as preprocessing the data.
Results:
The model successfully predicts fraudulent transactions with an acceptable accuracy, making it suitable for real-world applications in fraud detection systems.
