# Stock Prices Data Analysis Project

## Project Overview

This project demonstrates an **end-to-end data analysis workflow** on a large historical stock price dataset. It follows a **clean, industry-aligned structure** covering **data cleaning**, **exploratory data analysis (EDA)**, **feature engineering**, and a **summary of insights**.

The objective is to transform raw stock market data into a **clean, reliable, and analysis-ready dataset**, and to extract meaningful insights and features that reflect real-world stock behavior. This project is designed at a **fresher / entry-level Data Analyst standard**.

---

## 📂 Project Structure

```
├── task1_stock_price_dataset_cleaning.ipynb
├── task2_stock_price_dataset_EDA.ipynb
├── task3_stock_price_dataset_feature_engineering.ipynb
├── task4_stock_price_dataset_insights.ipynb
├── complete_stock_dataset_cleaned.csv
├── stock_data_feature_engineered.csv
└── README.md
```

---

## 🔹 Task 1 – Data Cleaning

**Notebook:** `task1_stock_price_dataset_cleaning.ipynb`

### Purpose

Prepare the raw stock dataset by fixing data quality issues and ensuring logical correctness.

### Key Steps

* Loaded raw historical stock price data
* Checked dataset structure, data types, and size
* Handled missing values using **symbol-wise forward and backward fill**
* Removed logically invalid records (e.g., `low price > high price`)
* Checked for duplicate records using `symbol + date`
* Validated dataset integrity after cleaning
* Saved the cleaned dataset

### Output

* `complete_stock_dataset_cleaned.csv`

> Data cleaning was completed **before any analysis or feature engineering**.

---

## 🔹 Task 2 – Exploratory Data Analysis (EDA)

**Notebook:** `task2_stock_price_dataset_EDA.ipynb`

### Purpose

Understand the dataset characteristics and validate market behavior using the **cleaned dataset**.

### Key Steps

* Loaded the cleaned dataset
* Verified absence of missing values and duplicates
* Reviewed summary statistics and distributions
* Performed logical validation checks
* Analyzed price trends, volatility patterns, and trading volume behavior

> EDA was performed on **cleaned data** to ensure accurate and trustworthy insights.

---

## 🔹 Task 3 – Feature Engineering

**Notebook:** `task3_stock_price_dataset_feature_engineering.ipynb`

### Purpose

Create meaningful financial and technical features for deeper analysis or modeling.

### Features Engineered

* **Daily Return** – Percentage change in closing price (symbol-wise)
* **Price Range** – Difference between daily high and low prices
* **10-day Moving Average (MA10)** – Short-term trend indicator
* **10-day Volatility** – Rolling standard deviation of daily returns

### Additional Steps

* Ensured proper time-series ordering by `symbol` and `date`
* Handled NaN values created by rolling window calculations
* Saved the feature-engineered dataset

### Output

* `stock_data_feature_engineered.csv`

---

## 🔹 Task 4 – Summary of Insights (EDA)

**Notebook:** `task4_stock_price_dataset_insights.ipynb`

### Purpose

Summarize and interpret insights derived from the EDA and engineered features.

### Key Insights

#### Dataset Overview

* Contains multi-year daily stock data for many companies
* Includes prices and trading volume
* Dataset is clean with no missing values or duplicate records

#### Trend Analysis

* Stock prices show regular daily fluctuations
* Some stocks exhibit clear upward long-term trends
* Others show sideways or stable movement

#### Volatility Insights

* Volatility measured using price range, daily return, and rolling volatility
* Stocks with higher price range are more volatile
* Rolling volatility highlights periods of market uncertainty

#### Volume Insights

* Trading volume varies significantly across stocks
* High-volume stocks show consistent market participation
* Sudden volume spikes often align with major events or news

#### Moving Average Insights

* Moving averages smooth short-term noise
* Upward MA10 indicates short-term bullish phases
* Price crossing below MA10 may indicate weakening momentum

### Overall Conclusion

* Feature engineering enhances understanding of stock behavior
* The dataset is now fully prepared for advanced analysis such as visualization, forecasting, or machine learning

---

## 🛠️ Tools & Technologies Used

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Jupyter Notebook** – Development environment

---

##  Fresher-Level Suitability

This project demonstrates:

* Strong understanding of data cleaning and validation
* Practical EDA on real-world financial data
* Correct handling of time-series data
* Clean separation of cleaning, EDA, feature engineering, and insights

It is well-suited for **Data Analyst / Business Analyst fresher roles**.

---

##  Future Enhancements

* Data visualization dashboards
* Sector-wise or symbol-wise comparisons
* Time-series forecasting models
* Machine learning for price movement prediction

---

## 📌 Author

**Pravin Kamble**

---

> This project reflects a clean, structured, and industry-aligned approach to stock market data analysis.
