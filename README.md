# Customer Churn Prediction Using Machine Learning

## 📌 Project Overview

Customer churn occurs when customers stop using a company's products or services. Predicting churn helps businesses identify customers who may leave and take steps to improve customer retention.

This project uses **Machine Learning to predict customer churn** based on customer information, service usage, contract details, and billing data. A Logistic Regression model is trained to classify customers as likely to churn or not churn.

## 🎯 Objectives

- Analyze customer data to understand patterns and characteristics.
- Perform Exploratory Data Analysis (EDA) using visualizations and statistical summaries.
- Clean and preprocess the dataset for machine learning.
- Train a Logistic Regression model to predict customer churn.
- Evaluate model performance using accuracy, F1-score, and a classification report.

## 🛠️ Technologies Used

- **Python** – Programming language
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Data preprocessing, model training, and evaluation
- **Jupyter Notebook** – Development environment

## 📂 Project Structure

```text
Customer-Churn-Prediction/
│
├── CustomerChurnPrediction_FIXED.ipynb
├── Customer.csv
└── README.md
```

## 📊 Dataset

The project uses a customer churn dataset containing information about customer demographics, subscriptions, services, and billing.

Important features include:

- Customer tenure
- Senior citizen status
- Partner and dependent information
- Phone and internet services
- Online security and technical support
- Contract type and payment method
- Monthly charges and total charges

**Target variable:** `Churn`

- `Yes` – Customer has churned.
- `No` – Customer has not churned.

The notebook also includes a setup cell that can generate `Customer.csv` from the original Telco Customer Churn dataset if the CSV file is not already present.

## ⚙️ Methodology

### 1. Data Exploration
- Inspect dataset structure and data types.
- Generate descriptive statistics.
- Check missing values.
- Visualize numerical distributions and relationships.
- Analyze correlations using a heatmap.

### 2. Data Preprocessing
- Convert `Total Charges` into a numerical format.
- Replace missing or invalid total-charge values with `0`.
- Remove `Customer ID` and `LoyaltyID` from the model features.
- Convert categorical variables into numerical representations using Label Encoding.
- Scale features using StandardScaler.

### 3. Model Training
- Separate the dataset into features (`X`) and target (`y`).
- Split the data into training and testing sets using an 80:20 ratio.
- Train a Logistic Regression model with a maximum of 1,000 iterations.

### 4. Model Evaluation

The model is evaluated using:

- **Accuracy:** Measures the proportion of correct predictions.
- **F1-score:** Balances precision and recall.
- **Classification Report:** Provides precision, recall, F1-score, and support for each class.

The notebook prints the evaluation results after training and prediction.

## 🚀 How to Run the Project

**Prerequisites:** Python 3, Jupyter Notebook, and the required Python libraries.

1. Clone or download this repository.

2. Install the dependencies:

   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn jupyter
   ```

3. Ensure `Customer.csv` is in the same directory as the notebook. Alternatively, run the notebook's setup cell to generate the dataset.

4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `CustomerChurnPrediction_FIXED.ipynb` and run the cells in order.

6. Review the data visualizations, model predictions, accuracy, F1-score, and classification report.

## 📈 Results

The project trains a Logistic Regression model to classify customer churn and evaluates its performance on the test dataset.

- **Model:** Logistic Regression
- **Training/testing split:** 80% / 20%
- **Evaluation metrics:** Accuracy, F1-score, precision, and recall

The actual performance values are generated when the notebook is executed. They should be added here after verifying the output.

## 🔮 Future Improvements

- Compare Logistic Regression with Decision Tree, Random Forest, and other classification models.
- Apply more advanced categorical encoding techniques.
- Address class imbalance if present.
- Use cross-validation and hyperparameter tuning.
- Identify the most influential factors contributing to customer churn.
- Develop a simple web application for interactive churn predictions.

## 👩‍💻 Author

**Archana A**

B.Tech Computer Science and Engineering Student

GitHub: [archanaprajith](https://github.com/archanaprajith)

---

*This project was developed for learning and exploring machine learning, data analysis, and customer churn prediction.*
