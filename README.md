# Customer Churn Prediction using RFM Analysis

## Overview

This project focuses on customer churn prediction by analyzing customer behavior using Recency, Frequency, and Monetary (RFM) metrics. The goal is to classify customers as "Churned" or "Retained" based on their purchasing patterns. A logistic regression model is used to predict customer churn, enabling businesses to target at-risk customers and improve retention strategies.

## Dataset

The dataset includes customer purchase data, which is used to calculate RFM metrics and predict customer churn. The key features in the dataset include:

- **Customer ID**: Unique identifier for each customer.
- **InvoiceDate**: Date of the transaction.
- **Quantity**: Number of items purchased.
- **Price**: Price of the purchased items.
- **RFM Metrics**:
  - **Recency**: Number of days since the last purchase.
  - **Frequency**: Number of transactions or purchases.
  - **Monetary**: Total spending amount by the customer.

## Objective

- To create RFM metrics based on customer purchasing patterns.
- To define a target variable ("Churned" or "Retained") based on thresholds for the RFM metrics.
- To train a logistic regression model to classify and predict customer churn.

## Key Steps

### 1. Data Cleaning:
   - Handle missing values and outliers in the dataset.
   - Standardize or normalize features for better model performance.

### 2. RFM Analysis:
   - **Recency**: Days since the last purchase for each customer.
   - **Frequency**: Total number of transactions.
   - **Monetary**: Total amount spent by the customer.
   - Based on thresholds for Recency, Frequency, and Monetary, a target variable (`Churned` or `Retained`) is created. This target variable is used in the logistic regression model for prediction.

### 3. Logistic Regression:
   - A logistic regression model is applied to classify customers as "Churned" or "Retained."
   - The features used in the model include the RFM metrics:
     - Recency
     - Frequency
     - Monetary
   - Model performance is evaluated using key metrics like:
     - **Accuracy**
     - **Precision**
     - **Recall**
     - **F1-Score**
   
### 4. Model Evaluation:
   - The model is evaluated to determine how well it predicts churned customers.
   - Confusion matrix, ROC curve, and other performance metrics are used to assess the model's accuracy and predictive power.

### 5. Insights and Recommendations:
   - Identifying high-risk customers who are likely to churn.
   - Recommendations for targeted marketing campaigns to retain customers based on their RFM scores.

## Results

- **Logistic Regression Performance**:
  - **Accuracy**: The overall accuracy of the model in predicting customer churn.
  - **Precision & Recall**: Key metrics to evaluate the model's ability to correctly identify churned customers.
  - **F1-Score**: The harmonic mean of precision and recall.

- **RFM Segmentation Insights**:
  - Customers are segmented based on RFM values into different groups such as High-Value, At-Risk, and Low-Engagement.
  - Business decisions and targeted retention strategies can be informed using these segments.

## Dependencies

To run this project, the following libraries are required:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

Install the dependencies using:
```bash
pip install -r requirements.txt
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/customer-churn-rfm-analysis.git
   ```

2. Navigate to the project directory:
   ```bash
   cd customer-churn-rfm-analysis
   ```

3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Customer_Churn_Analysis.ipynb
   ```

4. Run the notebook to generate RFM metrics and perform churn prediction using logistic regression.

## Conclusion

This project successfully segments customers based on RFM metrics and uses a logistic regression model to predict churn. The analysis provides valuable insights into customer behavior and can be used to design targeted retention strategies for at-risk customers.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
```

### Key Changes:
1. **RFM Analysis**: I've added sections detailing the creation of Recency, Frequency, and Monetary metrics.
2. **Target Variable**: The README now explains the process of defining a churn/retained target variable.
3. **Logistic Regression**: I've updated the model description to highlight logistic regression for classification and added relevant evaluation metrics.

Let me know if you need further adjustments or more specifics!
