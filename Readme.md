# Customer Churn Prediction

A machine learning project to predict whether a customer is likely to churn based on telecom service usage, billing information, and customer profile data.

## Project Overview

Customer churn is one of the most important business metrics for subscription-based companies. This project analyzes customer behavior and builds a predictive model to estimate whether a customer is likely to leave a service provider.

The notebook explores the dataset, cleans and transforms the data, performs exploratory data analysis (EDA), and trains a classification model to predict churn.

## Objective

The main goals of this project are:

- Understand patterns in customer behavior
- Identify variables associated with churn
- Prepare and clean the dataset for machine learning
- Train a predictive model
- Evaluate model performance
- Derive business insights for customer retention

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Dataset

This project uses a telecom customer churn dataset containing customer information such as:

- Gender
- Senior citizen status
- Partner/dependents information
- Tenure
- Phone service and internet service usage
- Contract type
- Monthly charges
- Total charges
- Churn label (`Yes` / `No`)

The notebook expects the file named:

```bash
WA_Fn-UseC_-Telco-Customer-Churn.csv
```

Place the dataset in the project root directory before running the notebook.

## Project Workflow

The project follows these steps:

1. Load the dataset
2. Inspect columns and data types
3. Handle missing values
4. Convert data types where needed
5. Analyze churn patterns visually
6. Encode categorical variables
7. Split data into training and testing sets
8. Train a machine learning model
9. Evaluate classification performance
10. Interpret results and business implications

## Data Preprocessing

The notebook includes:

- Missing value checks
- Numeric conversion for `TotalCharges`
- Dropping rows with missing values in critical columns
- Encoding categorical variables using one-hot encoding
- Train/test splitting with stratification

## Model

The project uses a supervised classification model to predict customer churn. The workflow includes:

- Feature selection and transformation
- Train/test split
- Model training
- Prediction on the test set
- Performance metrics such as accuracy, confusion matrix, and classification report

## Evaluation Metrics

The model is evaluated using metrics such as:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Classification report

## Business Insights

The analysis helps identify which customer characteristics are more strongly associated with churn. This can support actions like:

- Targeting at-risk customers
- Improving retention campaigns
- Reducing customer churn
- Adjusting service plans and pricing strategies

## Repository Structure

```bash
Customer_Churn_Prediction/
├── Customer_Churn_Prediction.ipynb
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── Readme.md
└── .gitignore
```

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Customer_Churn_Prediction.git
cd Customer_Churn_Prediction
```

### 2. Create a virtual environment (optional but recommended)

```bash
python -m venv venv
```

On Windows:

```bash
venv\Scripts\activate
```

On macOS/Linux:

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Run the notebook

```bash
jupyter notebook
```

Open `Customer_Churn_Prediction.ipynb` and run all cells.

## How to Use

1. Place the dataset in the project folder.
2. Open the Jupyter notebook.
3. Run the cells in order.
4. Review the EDA charts and model evaluation output.
5. Use the findings to inform customer retention strategy.

## Results

The notebook produces visualizations of:

- Churn distribution
- Churn by contract type
- Tenure distribution by churn status
- Monthly charges compared across churn groups

These insights help explain the relationship between customer attributes and churn risk.

## License

This project is intended for educational and learning purposes.

## Author

Created as a customer churn prediction project using machine learning and data analysis techniques.

## Future Improvements

- Compare multiple models such as Random Forest, XGBoost, or Gradient Boosting
- Tune hyperparameters for better performance
- Add SHAP or feature importance analysis
- Build a web app for prediction
- Deploy the model for real-world use

---

