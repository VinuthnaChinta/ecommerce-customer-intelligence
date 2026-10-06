# E-Commerce Customer Intelligence

An end-to-end customer analytics project using over **1 million e-commerce transactions** to understand customer behavior, measure customer value, identify customer segments, and develop actionable business strategies.

The project combines:

- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- Revenue analysis
- RFM analysis
- Log transformation
- K-Means clustering
- Customer segmentation
- Segment-level revenue analysis
- Business strategy recommendations

---

## 📌 Project Overview

The objective of this project is to answer a simple business question:

> **Which customers are most valuable, how engaged are they, and how should the business treat different customer segments?**

Using transaction-level e-commerce data, I transformed raw sales records into customer-level behavioral features using **RFM analysis** and then applied **K-Means clustering** to identify distinct customer segments.

The final analysis provides both quantitative customer insights and actionable strategies for customer retention, reactivation, and revenue growth.

---

## 🎯 Business Objectives

The project focuses on answering the following questions:

1. How large is the transaction dataset?
2. What is the overall revenue generated?
3. How many unique customers and products are present?
4. Which customers generate the most revenue?
5. How frequently do customers purchase?
6. How recently have customers purchased?
7. Which customers have the highest monetary value?
8. Can customers be grouped into meaningful behavioral segments?
9. Which segments contribute the most revenue?
10. What business strategies should be used for each customer segment?

---

## 📊 Dataset

The project uses the **Online Retail II** dataset containing e-commerce transactions.

### Original Dataset

| Metric | Value |
|---|---:|
| Transactions | 1,067,371 |
| Columns | 8 |
| Time Period | Dec 2009 – Dec 2011 |
| Countries | 41 |
| Unique Products | 4,631 |
| Unique Customers | 5,878 |

### Dataset Columns

| Column | Description |
|---|---|
| `Invoice` | Invoice / transaction identifier |
| `StockCode` | Product identifier |
| `Description` | Product description |
| `Quantity` | Number of units purchased |
| `InvoiceDate` | Transaction date and time |
| `Price` | Unit price |
| `Customer ID` | Customer identifier |
| `Country` | Customer's country |

---

# 🔧 Technology Stack

### Programming

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

### Development

- Jupyter Notebook
- VS Code
- Git
- GitHub

### Machine Learning

- K-Means Clustering
- StandardScaler
- Elbow Method

---

# 🧹 Data Cleaning

The raw dataset contained missing values and duplicate transactions.

## Initial Data Quality

The original dataset contained:

- **2,928 missing Description values**
- **107,927 missing Customer ID values**
- **6,865 duplicate rows**

These issues were identified using Pandas data-quality checks.

Example checks:

```python
df.info()

df.isnull().sum()

df.duplicated().sum()
