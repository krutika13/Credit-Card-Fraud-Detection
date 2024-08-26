Sure, here’s a template for a README file tailored for a Credit Card Fraud Detection project using Linear Regression.

---

# Credit Card Fraud Detection

## Overview

This project involves detecting fraudulent credit card transactions using a Linear Regression model. The goal is to identify potentially fraudulent transactions based on various features in the dataset.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Data](#data)
- [Model](#model)
- [Results](#results)
- [License](#license)

## Prerequisites

Make sure you have the following installed:
- Python 3.10.12


## Setup

1. **Clone the Repository:**
   ```bash git clone https://github.com/krutika13/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
   ```

  

## Data

The dataset used for this project is [Credit Card Fraud Detection Dataset]([https://www.kaggle.com/datasets?search=credit+card+fraud](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/data)). The dataset includes various features related to credit card transactions, including:

- `Amount`: Transaction amount
- `Time`: Time of transaction
- `Class`: Target variable indicating fraud (1 for fraud, 0 for non-fraud)
## Handling Imbalanced Data

The dataset was highly imbalanced, with only 473 fraudulent transactions (class 1) compared to 283,253 non-fraudulent transactions (class 0). To address this imbalance, I performed resampling by upsampling the minority class (fraudulent transactions) to ensure the model receives a balanced view of the classes during training.
## Feature Importance

To identify the most important features influencing the model's predictions, I used the permutation_importance function from sklearn.inspection. This method shuffles the values of each feature and measures how much the model's performance decreases, giving insight into which features are most critical.
I found that V14 is the most important feature in predicting fraudulent transactions.

## Model

### Linear Regression

Linear Regression is used to predict the likelihood of fraud based on transaction features. Here’s a brief outline of the model:

1. **Data Preprocessing:**
   - Handling missing values
   - Feature scaling
   - Encoding categorical variables if any

2. **Model Training:**
   - Splitting the data into training and testing sets
   - Training the Linear Regression model on the training data

3. **Model Evaluation:**
   - Evaluating the model performance using metrics like ROC AUC Score, R-squared score, Accuracy,Precision,Recall etc.




## Results

- **Model Performance:**
  - ROC AUC Score: 0.9765434324521155
  - Accuracy: 0.9383947326613828
  - Precision: 0.9597889475145793
  - Recall: 0.9151294769730455

- **Sample Predictions:**
  The model outputs predictions for whether a transaction is fraudulent or not.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

