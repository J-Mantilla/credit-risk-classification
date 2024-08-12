Credit Risk Analysis Using Logistic Regression
Overview of the Analysis
The purpose of this analysis is to assess the performance of a logistic regression model in predicting credit risk. By analyzing data on loan statuses, we aim to develop a model that can accurately distinguish between healthy loans (low risk) and high-risk loans. The results of this analysis will inform whether the model is suitable for deployment in a real-world setting to assist in credit risk evaluation.

Instructions
1. Split the Data into Training and Testing Sets
To begin the analysis:

Open the provided starter code notebook.
Load the lending_data.csv file from the Resources folder into a Pandas DataFrame.
Create the labels set (y) from the loan_status column.
Create the features set (X) by selecting the remaining columns.
Split the data into training and testing sets using train_test_split.

2. Create a Logistic Regression Model with the Original Data
Next, use logistic regression to build a predictive model:

Fit the logistic regression model using the training data (X_train and y_train).
Generate predictions on the test set (X_test) using the fitted model.
Evaluate the model’s performance by:
Generating a confusion matrix.
Printing the classification report.
Analyzing how well the model predicts both healthy loans (label 0) and high-risk loans (label 1).

3. Write a Credit Risk Analysis Report
Finally, summarize the analysis and results in this README file:

Overview of the Analysis: Explain the objective of the analysis (see above).
Results: Present the key metrics of the model’s performance.
Summary: Provide an overall assessment of the model, including whether it should be recommended for use by the company. Justify your recommendation based on the model's performance.
Results:

Accuracy: 99%
Precision Score Class-0 (healthy loan): 100%
Precision for class 1 (high-risk loan): 85%
Recall Score Class-0 (healthy loan): 99%
Recall for class-1 (high-risk loan): 91%

Summary:
When it comes to forecasting loan risk, the logistic regression model excels, especially when it comes to differentiating between low-risk and high-risk loans. The model demonstrates very good precision (100%) and recall (99%) for forecasting healthy loans, with an overall accuracy of 99%. It generates a 91% recall and 85% precision for loans that have a high risk. The primary issue is false negatives for high-risk loans, even though there aren't many of them. This might be resolved by adding more high-risk loan data to enhance model training.

In spite of this, the model performs well overall, particularly when it comes to correctly predicting healthy loans—a critical function in reducing financial risk. These metrics indicate that the logistic regression model is a viable option for credit risk assessment since it strikes a fair balance between recall and precision, which makes it a dependable predictor of loan status.
