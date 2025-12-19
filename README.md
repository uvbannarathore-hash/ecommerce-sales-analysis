# 🛒 E-Commerce Sales Analysis (EDA)

## 📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on real-world e-commerce transaction data to understand sales performance, customer behavior, product trends, and geographical revenue distribution.

Using Pandas, NumPy, Matplotlib, and Seaborn, the analysis provides business-oriented insights that can help improve:

Revenue growth

Product strategy

Customer retention

Market expansion

## 📂 Dataset

Source: Kaggle – Online Retail Dataset

File Used: data.csv

Data Type: Transaction-level e-commerce sales data

Encoding: latin1

Key Columns

InvoiceNo

InvoiceDate

CustomerID

Country

Description (Product)

Quantity

UnitPrice

Sales (engineered)

## 🛠️ Tools & Libraries Used

Python

Pandas – data cleaning & aggregation

NumPy – statistical analysis

Matplotlib – plotting

Seaborn – advanced visualizations

## 🔍 Project Workflow

### 1️⃣ Data Understanding

Inspected dataset structure using:

head(), info(), describe()

Analyzed shape, size, and datatypes

Identified missing values and anomalies

### 2️⃣ Data Cleaning & Preparation

Removed cancelled orders (InvoiceNo starting with C)

Dropped records with missing CustomerID

Converted InvoiceDate to datetime format

Created new time-based features:

Year

Month

Week

Day

Day of Week

Hour

### 3️⃣ Feature Engineering

Created key analytical columns:

Sales = Quantity × UnitPrice

Time-based features for trend analysis

### 4️⃣ Overall Sales Analysis

Calculated:

Total revenue

Number of transactions

Average order value

Analyzed:

Daily sales trend

Weekly sales trend

Monthly sales trend

Yearly sales trend

Identified month with maximum sales

### 5️⃣ Product Performance Analysis

Identified:

Top 10 selling products (by quantity)

Top revenue-generating products

Most frequently purchased products

Low-revenue products

Visualized:

Product demand distribution

Revenue contribution by product

### 6️⃣ Customer Behavior Analysis

Calculated:

Number of unique customers

Repeat vs one-time customers

Customer purchase frequency

Average order value per customer

Identified high-value customers

Visualized customer purchase distributions

### 7️⃣ Country-Wise Sales Analysis

Analyzed:

Country-wise revenue

Top countries by revenue

Top countries by number of orders


Created:

Sales heatmap (Country × Month)

Sales by Day of Week vs Hour heatmap

Monthly Sales vs Year heatmap

Calculated cumulative revenue contribution by country

## 📊 Visualizations Included

Sales distribution (Histogram + KDE)

Daily, weekly, monthly sales trends

Top products & low-revenue products

Customer frequency distributions

Country-wise revenue bar charts


Heatmaps for:

Country vs Month

Day of Week vs Hour

Year vs Month

Pairplot for multivariate analysis

## 💡 Key Insights

A small percentage of customers contribute a large share of total revenue

Sales show strong monthly and weekly seasonality

Certain products dominate both quantity and revenue

Repeat customers are critical for revenue stability

A few countries generate the majority of sales

Peak purchasing occurs during specific days and hours


## 📁 Project Structure
ecommerce-sales-analysis/
│
├── data/
│   └── data.csv
│
├── notebooks/
│   └── E-Commerce_Sales.ipynb
│
├── visuals/
│   └── sales_plots.png
│
├── requirements.txt
└── README.md

## 🚀 Future Enhancements

RFM (Recency, Frequency, Monetary) analysis

Customer segmentation

Sales forecasting

Churn risk identification

ML-based revenue prediction
