# TERM DEPOSIT PREDICTION 

## Project Overview
This project aims to build a machine learning model that predicts whether a bank client will subscribe to a term deposit based on historical marketing data. It forms part of a broader data analytics initiative to support targeted decision-making in financial services marketing.
By leveraging client and campaign data, the predictive model identifies potential subscribers of term deposit products, helping the bank allocate marketing resources more efficiently and improve subscription rates.

## Data Description
The dataset contains 41,188 rows and 17 features, capturing information such as:
- Client demographics (e.g., age, job, marital status).
- Financial status (e.g., default, housing and personal loan).
- Marketing campaign interactions (e.g., contact method, previous outcome).

The target variable is y(renamed to subscription), which indicates whether a client subscribed to a term deposit (yes or no).

The dataset used in this project is  a bank marketing campaign data and includes client information and campaign outcomes.For more detailed information about the dataset and its variables, [click here](data_files/bank-names.txt).


## Worklow or Methodology

### Exploratory Data Analysis (EDA)
- Analyzed distribution of features
- Detected imbalances in the target class
- Identified key correlations and trends

### Feature Engineering & Data Preprocessing  
- Encoded target
- Normalized numerical data
- Handled class imbalance using upsampling

### Model Training
- Trained a model using XGBoost, a powerful gradient boosting algorithm
- Evaluated performance using metrics like accuracy, precision, recall, and F1-score

### Model Evaluation
- Dealt with class imbalance
- Assessed model performance with a confusion matrix and classification report



##Key Insights

- The dataset is highly imbalanced, with only 11% positive subscriptions.
- Features like contact method, previous outcome, and duration show strong predictive power.
- XGBoost was chosen for its performance and ability to handle feature interactions effectively.


## Result
The final model achieved a reasonable balance between precision and recall, providing actionable insights to support more focused marketing strategies.



## User Guide

1. Clone the repository:
    ```bash
    git clone https://github.com/princekwusu/Term_Deposit_Prediction.git
    ```

2. Navigate to the directory:
    ```bash
    cd Term_Deposit_Prediction
    ```

3. Create a virtual environment ('myvenv' can be replaced with any name of choice ):
   ```bash
   python -m venv myvenv
   ```

4. Activate the virtual environment:
   ```bash
   source myvenv/Scripts/activate
   ```

5. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

6. Access `src/T_D_prediction.ipynb` to execute the scripts in the cells or adjust the scripts to suite needs.   


## CONTRIBUTION

Pull requests and suggestions are welcome. For major changes, please open an issue first to discuss what you would like to change.

## LICENSE

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.