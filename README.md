>Loan Approval Prediction System :
This project is a machine learning-based application designed to predict the likelihood of loan approval based on various financial and personal factors. It includes a complete pipeline from data preprocessing and model training to a user-friendly web interface powered by Streamlit.

>Project Overview :
The system evaluates loan applications by analyzing several key metrics, such as CIBIL score, annual income, loan amount, and asset values. The model is trained on a dataset of over 4,000 records.

>Key Features
1.Predictive Modeling: Uses a trained Logistic Regression model to classify loan status as 'Approved' or 'Rejected'.

2.Web Interface: A Streamlit app that allows users to input their data via sliders and dropdowns for real-time predictions.

3.Data Processing: Includes custom feature engineering, such as aggregating residential, commercial, luxury, and bank assets into a single "Assets" feature.

>File Structure
Loan_Approval_Pred_Model.ipynb: Jupyter notebook containing data cleaning, exploratory data analysis, and model training.

1.app.py: Streamlit application script for the user interface.

2.loan_approval_dataset.csv: The raw dataset used for training and testing.

3.model.pkl: The serialized trained Logistic Regression model.

4.scaler.pkl: The serialized StandardScaler used to normalize input data.

>Installation & Usage
Prerequisites :
1.Ensure you have Python installed, along with the following libraries:

2.pandas, streamlit, scikit-learn, pickle

3.Running the Application :
Clone this repository to your local machine.

Navigate to the project directory.

Run the Streamlit app using the following command:streamlit run app.py (Bash Command)


>Model Details
The prediction is based on the following input features:

-Number of Dependents: (0 to 5)

-Education: Graduate or Not Graduate

-Self-Employed: Yes or No

-Annual Income

-Loan Amount

-Loan Term

-CIBIL Score

Total Assets: Calculated as the sum of residential, commercial, luxury, and bank asset values.

Dataset Information
The dataset contains various features that influence loan approval:

CIBIL Score: A critical factor in determining creditworthiness.

Loan Status: The target variable (Approved/Rejected).

Assets: A combined metric representing the applicant's total financial backing.
