<h1>Credit Card Fraud Detection</h1>

<h2>1. Introduction</h2>
<p>Traditional fraud detection systems often fail to identify suspicious activities quickly due to the massive amount of transaction data. Therefore, automated fraud detection systems are essential for improving financial security.

This project uses data analysis and machine learning techniques to study transaction behavior and identify factors related to fraudulent transactions.</p>

<h2>2. Problem Statement</h2>

<p>Financial institutions and online payment systems process millions of credit card transactions every day. Among these transactions, some are fraudulent and unauthorized, leading to major financial losses for both customers and banks.

Due to the huge volume of transaction data, manually identifying fraudulent activities is difficult, time-consuming, and inefficient. Fraudulent transactions often occur within seconds, making it essential to detect suspicious activities automatically and accurately.</p>

<h3>Incorrect fraud detection decisions can result in:</h3>

* Financial losses for banks and customers<br>
* Unauthorized transactions<br>
* Poor fraud risk management<br>
* Reduced customer trust and security<br>

<p>Therefore, there is a need for an automated system that can analyze transaction data, identify unusual patterns, and help detect fraudulent credit card transactions.

This project focuses on Exploratory Data Analysis (EDA), Linear Regression, and Dashboard Visualization to understand transaction behavior and identify factors influencing fraud detection.</p>

 <h2>3. Objectives</h2>

<p>The main objective of this project is to perform Exploratory Data Analysis, build a Linear Regression model, and create an interactive dashboard for fraud analysis.</p>

<h3>Specific Objectives</h3>

1. Load and understand the dataset.<br>
2. Perform data cleaning and preprocessing.<br>
3. Analyze transaction behavior using statistical methods.<br>
4. Compare normal and fraudulent transactions.<br>
5. Identify high-risk transaction patterns.<br>
6. Visualize relationships among features.<br>
7. Build a Linear Regression model.<br>
8. Evaluate model performance.<br>
9. Create an interactive dashboard using Plotly.<br>
10. Generate insights to support fraud prevention.<br>



## Dataset Features

| Column Name | Description                             |
| ----------- | --------------------------------------- |
| Time        | Time elapsed between transactions       |
| Amount      | Transaction amount                      |
| V1 – V28    | Anonymized transaction features         |
| Class       | Target variable (0 = Normal, 1 = Fraud) |

## Removed Columns

The following types of columns were removed:

* Duplicate transaction records
* Unnecessary identifiers
* Highly sparse columns
* Irrelevant metadata columns

These columns were removed to simplify analysis and improve model performance.

---

# 5. Technologies Used

| Technology       | Purpose                   |
| ---------------- | ------------------------- |
| Python           | Programming Language      |
| Pandas           | Data manipulation         |
| NumPy            | Numerical operations      |
| Matplotlib       | Data visualization        |
| Seaborn          | Statistical visualization |
| Scikit-learn     | Machine learning          |
| Plotly           | Interactive dashboard     |
| Jupyter Notebook | Development environment   |

---

# 6. Methodology

## 6.1 Data Collection

The dataset was downloaded from Kaggle and loaded into Python using the Pandas library.

## 6.2 Data Cleaning and Preprocessing

The following preprocessing steps were performed:

* Checked missing values
* Removed duplicate records
* Verified data types
* Prepared dataset for analysis


## 6.3 Descriptive Statistics

Statistical analysis was performed to understand transaction behavior.

### Calculations Included

* Average transaction amount
* Fraud vs normal transaction count
* Transaction distribution
* Feature variation analysis

# 7. Exploratory Data Analysis (EDA)

Exploratory Data Analysis helps understand patterns and relationships in the dataset.

## 7.1 Fraud Distribution Analysis

Fraudulent transactions were compared with normal transactions.

### Observation

The dataset is highly imbalanced because fraud transactions are very small compared to normal transactions.

## 7.2 Transaction Amount Analysis

Transaction amounts were analyzed to identify suspicious patterns.

### Observation

Fraudulent transactions often show unusual transaction amounts compared to normal transactions.

## 7.3 Time-Based Analysis

Transaction time was analyzed to identify unusual activity periods.

### Observation

Certain time intervals showed increased fraud activity.

## 7.4 Correlation Analysis

A correlation heatmap was generated to identify relationships among features.

### Observation

Some anonymized features showed strong correlation with fraud transactions.

# 8. Data Visualization

Different visualizations were used for better understanding of transaction patterns.

## Visualizations Used

### 1. Bar Chart

Used to display fraud vs normal transaction distribution.
<img width="703" height="487" alt="Screenshot 2026-05-28 200019" src="https://github.com/user-attachments/assets/f013dcaf-eb0b-481e-82f8-b998116b651f" />


### 2. Histogram

Used to analyze transaction amount distribution.
<img width="865" height="586" alt="image" src="https://github.com/user-attachments/assets/d0f80386-ae93-49aa-8db3-6a28e6c07b43" />


### 3. Scatter Plot

Used to visualize relationships between time and transaction amount.
<img width="897" height="587" alt="image" src="https://github.com/user-attachments/assets/e62f6627-4899-4c02-b865-8839ebda854d" />


### 4. Box Plot

Used to detect outliers in transaction amounts.
<img width="705" height="497" alt="image" src="https://github.com/user-attachments/assets/38d1fd22-b478-4e30-91d0-a7148e4afae5" />


### 5. Heatmap

Used to visualize feature correlations.
<img width="1088" height="876" alt="image" src="https://github.com/user-attachments/assets/14aab97c-5380-4734-b1c7-aa3ccd86e571" />


# 9. Risk Analysis

Transactions were categorized into risk levels based on transaction amount.

## Risk Categories

| Amount Range   | Risk Level  |
| -------------- | ----------- |
| Less than 100  | Low Risk    |
| 100 – 999      | Medium Risk |
| 1000 and above | High Risk   |

### Purpose

This classification helps identify suspicious transactions more effectively.
# 10. Predictive Modeling

## 10.1 Linear Regression

Linear Regression was used to analyze transaction trends and relationships.

### Independent Variables

* Time
* Amount

### Dependent Variable

* Transaction amount prediction / fraud-related analysis

## 10.2 Model Training

The dataset was divided into training and testing sets.
The model was trained using Linear Regression.
## 10.3 Prediction

The trained model was used to predict transaction trends.

# 11. Model Evaluation

The model performance was evaluated using:

## 11.1 R² Score

Measures how well the model explains variation in data.
R2 Score: 0.00015552801701912422

## 11.2 Mean Squared Error (MSE)

Measures prediction error.
Mean Squared Error: 58643.98795669793

### Observation

The evaluation metrics help determine prediction accuracy and model performance.

# 12. Dashboard Visualization

An interactive dashboard was created using Plotly.

## Dashboard Features

### Fraud Distribution Visualization

Displays comparison between fraud and normal transactions.

### Transaction Amount Trends

Visualizes transaction patterns over time.

### Correlation Heatmap

Shows relationships among features.

### Risk Analysis Charts

Displays low, medium, and high-risk transactions.

## Interactive Features

* Dynamic charts
* Interactive filtering
* Zoom and hover analysis


# 13. Results and Findings

The analysis produced the following findings:

1. Fraud transactions are very rare compared to normal transactions.
2. Transaction amount is an important factor in fraud analysis.
3. Certain anonymized features strongly influence fraud behavior.
4. High-risk transactions can be identified using transaction patterns.
5. Visual dashboards improve fraud analysis and decision-making.

# 14. Advantages of the Project

* Helps identify suspicious transactions quickly
* Improves fraud risk management
* Reduces financial losses
* Supports data-driven decision making
* Enhances customer trust and security


# 15. Limitations

* Dataset is highly imbalanced
* Linear Regression may not provide high fraud classification accuracy
* Real-time fraud detection requires more advanced machine learning models

# 16. Future Enhancements

Future improvements can include:

* Using advanced machine learning algorithms
* Real-time fraud detection system
* Deep learning models
* Streamlit or Power BI dashboards
* Automated alert generation
* Fraud probability scoring system

# 17. Conclusion

This project successfully analyzed credit card transaction data using Exploratory Data Analysis, Linear Regression, and Dashboard Visualization techniques.

The study helped identify fraud patterns, transaction behaviors, and high-risk activities. Data visualization and statistical analysis provided valuable insights into fraud detection.

Although Linear Regression has limitations for fraud classification, the project demonstrates how data analysis and visualization can support fraud prevention strategies in financial systems.
