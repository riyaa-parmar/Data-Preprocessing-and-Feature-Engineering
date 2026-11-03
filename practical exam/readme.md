# 🛒 Customer Purchase Behavior Analysis & Data Preprocessing

## 📌 Project Overview

This project focuses on analyzing customer purchase data and demonstrating the complete data analysis and preprocessing workflow using Python.

The project uses customer information, transaction records, product details, and external API data collected from different sources and formats.

The main objective is to understand the datasets, perform Exploratory Data Analysis (EDA), handle data quality issues, apply preprocessing techniques, and prepare a final processed dataset for further analysis.

## 🎯 Project Objectives

* Import data from CSV, JSON, SQL, and REST API sources.
* Understand dataset structure and data types.
* Perform Exploratory Data Analysis (EDA).
* Identify and handle missing values.
* Detect and handle outliers.
* Process date and time variables.
* Convert categorical data into numerical format.
* Apply feature scaling techniques.
* Create new features from existing data.
* Perform mathematical data transformations.
* Export the final processed dataset.

## 🗂️ Project Structure

```text
Customer_Purchase_Behavior_Analysis/
│
├── Data/
│   ├── customers.csv
│   ├── transactions.json
│   └── products.sql
│
├── Notebook/
│   └── Customer_Purchase_Analysis.ipynb
│
├── Output/
│   └── final_customer_purchase_data.csv
│
└── README.md
```

## 📊 Datasets Used

The project uses the following data sources:

### 1. Customers Dataset (CSV)

Contains customer demographic information.

* Customer ID
* Name
* Age
* Gender
* City
* Income

### 2. Transactions Dataset (JSON)

Contains customer purchase transaction details.

* Transaction ID
* Customer ID
* Product ID
* Transaction Amount
* Payment Mode
* Transaction Date

### 3. Products Dataset (SQL)

Contains product information.

* Product ID
* Product Name
* Category
* Price
* Stock

### 4. External API Data

**API:** DummyJSON Users API

**Endpoint:** `https://dummyjson.com/users`

The API is used to fetch user information from an external source using Python Requests. The JSON response is converted into a Pandas DataFrame.

API data is treated as a separate data source because its user IDs do not correspond to the customer IDs in the original datasets.

## 🛠️ Technologies & Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SQLite
* Requests
* Scikit-learn
* Jupyter Notebook

## 🔍 Project Workflow

### 1. Project Planning

Defined the project objective, problem statement, and data analysis workflow.

### 2. Data Import and Understanding

* Imported CSV data using Pandas.
* Loaded JSON data using Python.
* Executed SQL scripts using SQLite.
* Fetched external data using REST API.
* Examined dataset shape, columns, data types, and statistical summaries.

### 3. Exploratory Data Analysis (EDA)

Performed:

* Univariate Analysis
* Bivariate Analysis
* Multivariate Analysis
* Histograms
* Boxplots
* Bar Charts
* Correlation Heatmap

### 4. Missing Data Handling

* Identified missing values.
* Demonstrated Mean Imputation.
* Demonstrated Median Imputation.
* Demonstrated Mode Imputation.

The original datasets did not contain missing values. Therefore, missing values were introduced only in a temporary copy to demonstrate imputation techniques.

### 5. Outlier Detection and Handling

* Used Boxplots for visualization.
* Applied the Interquartile Range (IQR) method.
* Identified potential outliers.
* Demonstrated outlier capping using the IQR boundaries.

### 6. Mixed Data and Date-Time Handling

* Identified different data types.
* Converted date columns into DateTime format.
* Extracted year, month, day, and day name.
* Performed daily transaction analysis.

### 7. Categorical Data Encoding

Applied:

* Label Encoding
* One-Hot Encoding

Converted categorical variables into numerical representations.

### 8. Feature Scaling

Applied and compared:

* Min-Max Scaling
* Standardization (StandardScaler)

### 9. Feature Construction and Data Transformation

Created new features:

* Total Purchase Value
* Age Group
* Income Category
* Log Transformed Amount

Applied mathematical transformation to numerical data.

### 10. Final Output

* Prepared the final processed dataset.
* Checked missing values and duplicate records.
* Examined the final dataset structure.
* Exported the final dataset as a CSV file.

## 📈 Key Findings and Limitations

* The original datasets contain 8 customer records, 8 transaction records, and 6 product records.
* No missing values were found in the original datasets.
* Each customer has one transaction in the provided transaction data.
* All original transaction customer IDs and product IDs match the corresponding records.
* The dataset is small, so the analysis is mainly intended to demonstrate data analysis and preprocessing techniques.
* The available data is insufficient to establish reliable long-term customer purchase behavior patterns.

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the Project Folder

```bash
cd Customer_Purchase_Behavior_Analysis
```

### 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn requests jupyter
```

### 4. Open Jupyter Notebook

```bash
jupyter notebook
```

### 5. Run the Project

1. Open `Customer_Purchase_Analysis.ipynb`.
2. Make sure the Data and Output folders are available.
3. Update file paths if your folder structure is different.
4. Run all cells from top to bottom.
5. The final processed CSV file will be generated in the Output folder.

## 📁 Final Output

The final processed dataset is saved as:

`final_customer_purchase_data.csv`

It contains the merged customer, transaction, and product information along with the additional engineered features.

## 🚀 Future Improvements

* Use larger and more diverse datasets.
* Perform deeper customer segmentation.
* Analyze repeat purchase behavior using more transaction records.
* Build interactive dashboards.
* Apply machine learning techniques for customer behavior analysis.

## 👩‍💻 Author

**Riya Parmar**

Aspiring AI & Data Science Professional

Skills: Python | SQL | Excel | Power BI | Data Analysis

---

⭐ If you find this project useful, consider giving the repository a star!
