# Bad_Loan_Prediction_JPMC

Bad Loan (Loan Default) Prediction: An End-to-End Data Science Project
This repository contains a complete data science project focused on predicting loan defaults. The project includes a thorough Exploratory Data Analysis (EDA), and the logic flows on the neural networks as I'm new to the concept.

Business Problem

The challenge is to build a model that predicts at application time whether an applicant will default on their loan. The data consists of a set of variables that describe the requested loan and the applicant's credit attributes. The goal is to leverage data analysis and machine learning to identify key risk drivers and provide strategic recommendations to optimize the loan portfolio and stipulation process.

Project Structure

EDA - Bad Loan Prediction.ipynb: A Jupyter Notebook containing the comprehensive Exploratory Data Analysis, from initial data inspection to multivariate analysis and key findings.

PyTorch_Loan_Classifier.txt: A text file with a logic flow on building out a neural network to indicate bad loans.

README.md: This file, providing an overview of the project.

Note: As per the instructions, the raw datasets (training_loan_data.csv and testing_loan_data.csv) are not included in this repository.

How to Run the Code
1. Environment Setup
This project requires Python 3.8+ and several common data science libraries. You can install all dependencies using pip:

pip install pandas numpy scikit-learn torch matplotlib seaborn jupyter

2. Execution Steps
Place Data Files: Download the training_loan_data.csv and testing_loan_data.csv files and place them in the root directory of this project.

Run Exploratory Data Analysis: Open and run all cells in the EDA_Bad_Loan_Prediction.ipynb notebook to see the initial data analysis, visualizations, and insights.

Run Model Training and Inference: Please read through the logic flows in Pytorch_Neural_Networks.txt

Key Findings & Strategic Recommendations
The analysis produced several actionable insights crucial for optimizing portfolio performance.

Key Findings
Interest Rate is the Dominant Risk Factor: The int_rate is the single most powerful predictor of default. This pattern holds true across all customer segments.

A High-Risk Segment Was Identified: Loans for small businesses and renewable energy are especially risky given the top 2 bad flag rates across all loan purposes

Lower income population, people who push on their bank card limits, people who have higher DTI, people who inquire on credit more frequently in a short period of time, people who have higher credit utilization tend to point towards a defaulted loan.

The Third-Party Score is Not a Strong Predictor given its ineffectiveness when comparing to the bad flag indicator.

Review Third-Party Tools: 

Assumptions: Missing numerical values were imputed with the median of the training data, and categorical values were imputed with the mode. This will be a robust baseline approach that is less sensitive to outliers than using the mean.
