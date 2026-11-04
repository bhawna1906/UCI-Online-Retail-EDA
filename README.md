![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-red)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-purple)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)
# 🛍️ UCI Online Retail — Exploratory Data Analysis (EDA)

### 📊 Uncovering Sales Trends, Product Performance & Business Opportunities with Python

An exploratory data analysis project on retail transaction data using Python, Pandas, NumPy, Matplotlib, and Seaborn to identify sales patterns, evaluate product performance, understand customer markets, and generate actionable business insights.

---

## 📌 Table of Contents

- 🎯 [Project Overview](#-project-overview)
- 💼 [Business Objectives](#-business-objectives)
- 📂 [Dataset Information](#-dataset-information)
- 🛠️ [Tools and Technologies](#️-tools-and-technologies)
- 🔄 [Project Workflow](#-project-workflow)
- 📈 [Key Performance Indicators](#-key-performance-indicators)
- 🔍 [Business Questions Answered](#-business-questions-answered)
- 💡 [Key Business Insights](#-key-business-insights)
- 🚀 [Strategic Recommendations](#-strategic-recommendations)
- 🧠 [Sample Visualization](#-sample-visualization)
- ⚠️ [Limitations](#️-limitations)
- ⚙️ [How to Run the Project](#️-how-to-run-the-project)
- 🔮 [Future Improvements](#-future-improvements)
- 🧠 [Skills Demonstrated](#-skills-demonstrated)
- 👩‍💻 [Author](#-author)

---

## 🎯 Project Overview

Retail businesses generate large volumes of transactional data, but transforming this data into meaningful business decisions requires careful analysis.

This project explores the **UCI Online Retail Dataset**, containing transaction records from a UK-based online retailer, to understand revenue patterns, product demand, purchasing activity, and geographical sales distribution.

Using Python-based data cleaning, feature engineering, exploratory data analysis, and visualization, this project aims to uncover meaningful patterns in retail performance and translate them into actionable business insights.

The focus extends beyond visualizing data to understanding **what the findings mean for the business and how they can support better decision-making.**

## 💼 Business Objectives

The primary objectives of this analysis are to:

- 💰 Evaluate overall sales performance using key business metrics.
- 📦 Understand the distribution of transaction quantities, unit prices, and revenue.
- 🔄 Examine cancellation-related and negative-value transactions.
- 📅 Identify sales patterns across months, quarters, weekdays, and hours.
- 🌍 Determine the major revenue-generating countries.
- 🏆 Identify high-revenue and high-volume products.
- 💡 Develop data-driven recommendations for sales optimization and operational improvement.

---

## 📂 Dataset Information

**Dataset:** Online Retail

**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/352/online+retail)

**Original Dataset Size:** 541,909 transaction records

**Time Period:** December 2010 – December 2011

The dataset contains transactions from a UK-based online retailer that primarily sells unique all-occasion gifts. Many customers are wholesalers.

### 🧾 Dataset Features

| Column | Description |
|---|---|
| `InvoiceNo` | Invoice identifier; values beginning with `C` indicate cancellations. |
| `StockCode` | Product identifier. |
| `Description` | Product name or transaction description. |
| `Quantity` | Number of units recorded in a transaction line. |
| `InvoiceDate` | Transaction invoice date and time. |
| `UnitPrice` | Price per unit in GBP (£). |
| `CustomerID` | Customer identifier, when available. |
| `Country` | Customer's country. |

---

## 🛠️ Tools and Technologies

- 🐍 **Python** — Core programming language.
- 🐼 **Pandas** — Data cleaning, manipulation, and aggregation.
- 🔢 **NumPy** — Numerical operations.
- 📊 **Matplotlib** — Data visualization.
- 🎨 **Seaborn** — Statistical visualization.
- 📓 **Jupyter Notebook** — Interactive analysis and documentation.
- 🐙 **Git & GitHub** — Version control and project hosting.

---

## 🔄 Project Workflow

### 1️⃣ Data Understanding 🔍

- Examined the dataset's dimensions, data types, and summary statistics.
- Inspected missing values and duplicate records.
- Explored the structure and characteristics of the transaction data.

### 2️⃣ Data Cleaning 🧹

- Investigated missing and unusual values.
- Converted date columns into appropriate datetime formats.
- Identified cancellation invoices and negative-quantity transactions.
- Applied data filters to prepare the dataset for sales analysis.

### 3️⃣ Feature Engineering ⚙️

Created a revenue feature using:

```python
Revenue = Quantity * UnitPrice
```

This feature supports revenue calculations and comparisons across products, countries, and time periods.

### 4️⃣ Exploratory Data Analysis 📊

Performed distribution analysis, relationship analysis, product ranking, geographical comparisons, and time-based sales analysis.

### 5️⃣ Business Insight Generation 💡

Interpreted analytical results to identify sales patterns, investigate operational concerns, and formulate business recommendations.

---

## 📈 Key Performance Indicators

The analysis examines the following metrics using the filtered sales data:

| Metric | Business Purpose |
|---|---|
| 💰 Gross Sales Revenue | Measures revenue from qualifying positive sales transactions. |
| 💷 Net Revenue | Examines revenue after negative-value transaction lines under the notebook's calculation. |
| 📦 Units Sold | Measures total units recorded in the selected sales transactions. |
| 🧾 Sales Invoices | Measures unique invoices included in the sales analysis. |
| 🛒 Average Order Value | Measures average gross revenue per included sales invoice. |
| 👥 Identified Customers | Counts distinct available customer IDs. |
| 🔄 Cancellation Invoice Lines | Measures transaction lines associated with cancellation invoices. |
| ↩️ Negative/Return-Related Lines | Identifies selected lines with negative quantities or revenue. |

These metrics provide a foundation for evaluating sales performance and identifying areas requiring further investigation.

---

## 🔍 Business Questions Answered

### 📊 1. What does the distribution of transaction quantities reveal?

Analyzed the distribution of quantities to understand typical transaction sizes and identify unusually large or negative values.

**💡 Business Insight:** The distribution helps distinguish routine purchasing activity from bulk transactions that may require separate investigation.

### 💷 2. How are unit prices distributed?

Examined unit prices to understand the range of product prices and identify potential outliers.

**💡 Business Insight:** Understanding price variation can support product segmentation and more informed pricing analysis.

### 💰 3. What does the revenue distribution reveal?

Analyzed transaction revenue to understand how sales values vary across transaction lines.

**💡 Business Insight:** A highly skewed distribution may indicate that a relatively small number of transactions contribute disproportionately to revenue.

### 🔗 4. What is the relationship between unit price and quantity?

Used a scatter plot to examine the relationship between product price and transaction quantity, with revenue represented through color.

**💡 Business Insight:** This analysis helps distinguish high-value transactions associated with higher prices from those driven by larger quantities.

### 🔄 5. How significant are cancellation-related transactions?

Examined invoice lines associated with cancellation invoices.

**💡 Business Insight:** Cancellation activity should be monitored to understand its potential impact on revenue reporting, inventory availability, and operational efficiency.

### 📅 6. How does sales revenue change over time?

Analyzed revenue by year, month, and quarter.

**💡 Business Insight:** Time-based analysis helps identify periods of stronger recorded sales activity and supports further investigation into demand patterns.

### 🕒 7. Which hours record the highest sales revenue?

Compared revenue across hours of the day.

**💡 Business Insight:** Stronger recorded sales periods can guide further investigation into order-processing workloads and operational planning.

### 📆 8. How does revenue vary by day of the week?

Compared revenue across weekdays to identify differences in recorded sales activity.

**💡 Business Insight:** Day-of-week patterns can help identify when additional operational attention may be needed, once differences in observation coverage are validated.

### 🌍 9. Which countries generate the highest revenue?

Ranked countries according to gross sales revenue.

**💡 Business Insight:** Identifying the leading markets helps businesses understand geographical revenue concentration and evaluate potential international opportunities.

### 🏆 10. Which products generate the highest revenue?

Ranked product descriptions based on recorded sales revenue.

**💡 Business Insight:** High-revenue products deserve further evaluation using sales frequency, costs, and profitability before inventory or investment decisions are made.

### 📦 11. Which products sell the highest number of units?

Examined products by total units sold.

**💡 Business Insight:** High-volume products may require closer inventory monitoring, but their commercial importance should also be evaluated using revenue, order frequency, and margins.

---

## 💡 Key Business Insights

The following findings are based on the calculated metrics and aggregations in the analysis. Figures should be interpreted in the context of the notebook's filtering rules.

- 💰 **Gross Sales Revenue:** The filtered sales transactions generated approximately **£10.64 million** in gross sales revenue.
- 📦 **Units Sold:** Approximately **5.57 million units** were recorded in the selected sales transactions.
- 🧾 **Sales Activity:** Approximately **19,960 unique sales invoices** were included in the analysis.
- 🛒 **Average Order Value:** The calculated average order value was approximately **£533.17**.
- 🇬🇧 **Geographical Concentration:** The United Kingdom contributed approximately **£9.00 million**, or 84.6% of analyzed gross sales revenue.
- 📈 **Quarterly Performance:** Recorded revenue was highest in Q4 2011, at approximately **£3.29 million**. However, comparisons with Q4 2010 are affected by the incomplete 2010 observation period.
- 🕙 **Hourly Patterns:** Recorded hourly revenue was highest at 10:00, followed by 12:00 and 15:00.
- 🏆 **Product Performance:** High-revenue products and high-volume products are not necessarily the same, highlighting the importance of using multiple performance measures.
- 🔄 **Transaction Monitoring:** Cancellation and negative-value transactions require separate analysis to understand their impact on net revenue and operational performance.

---

## 🚀 Strategic Recommendations

### 🌍 1. Strengthen the Core Market and Explore International Expansion

- Maintain product availability and customer satisfaction in the UK.
- Evaluate international markets based on demand, shipping costs, and contribution margins.
- Test targeted marketing campaigns before expanding into new markets at scale.

### 📦 2. Optimize Inventory Management

- Monitor high-volume and frequently purchased products.
- Investigate bulk purchases and demand variability.
- Establish replenishment policies based on demand patterns and supplier lead times.
- Evaluate inventory decisions using revenue, volume, and profitability together.

### 🛒 3. Improve Average Order Value

- Test product bundles and complementary-product recommendations.
- Explore volume-based offers where commercially appropriate.
- Compare order value across customer groups and countries.
- Evaluate promotional effectiveness using profit per order, not revenue alone.

### 📅 4. Improve Sales and Operational Planning

- Investigate hourly, weekly, and monthly sales patterns.
- Compare revenue with order counts and average order value.
- Align operational capacity with validated demand patterns.
- Use additional years of data before concluding that seasonal patterns recur.

### 🔄 5. Monitor Cancellations and Negative Transactions

- Calculate cancellation and return rates using clearly defined invoice-level metrics.
- Investigate products and periods with unusual cancellation activity.
- Identify recurring transaction issues.
- Reconcile gross sales, refunds, and net revenue.

### 👥 6. Strengthen Customer Retention

- Analyze customer purchase histories where customer IDs are available.
- Identify repeat customers and potentially inactive customers.
- Explore RFM segmentation using Recency, Frequency, and Monetary value.
- Test targeted retention campaigns and relevant product recommendations.

### 🏆 7. Improve Product Performance Analysis

- Separate physical products from postage and other non-merchandise descriptions.
- Rank products independently by revenue and units sold.
- Evaluate order frequency and profitability where cost data is available.
- Use these measures to support product and inventory decisions.

### 📊 8. Adopt Data-Driven Decision-Making

- Monitor revenue, average order value, sales volume, and cancellation rates.
- Track country-wise and product-wise performance.
- Consider developing an interactive dashboard using Power BI or Streamlit.
- Review KPIs regularly and investigate significant changes.

---

## 🧠 Sample Visualization

<img width="1190" height="490" alt="image" src="https://github.com/user-attachments/assets/fd8d2f58-b91d-4746-a2c6-187b86da32d8" />
<img width="1090" height="490" alt="image" src="https://github.com/user-attachments/assets/9cc07671-b569-4425-9c94-16f2a6c6a898" />
<img width="990" height="490" alt="image" src="https://github.com/user-attachments/assets/40e3160d-daf9-4fab-8ed0-aa570881b7c8" />
<img width="1190" height="490" alt="image" src="https://github.com/user-attachments/assets/24d32070-bd6c-4257-a2ed-55287d9c6b8c" />

---

## ⚠️ Limitations

- 📅 The dataset covers a limited historical period, restricting long-term trend and seasonality analysis.
- 📉 The 2010 and 2011 observation periods are not equally complete.
- 👤 Missing customer IDs limit customer-level analysis.
- 🔄 Cancellation invoice lines are not equivalent to unique cancelled orders.
- ↩️ Negative transaction quantities may represent returns or other adjustments and require contextual validation.
- 💷 Revenue does not equal profit because product costs and operating expenses are unavailable.
- 🕒 Invoice timestamps do not necessarily represent website browsing or order-placement times.
- 🔍 The analysis is descriptive and does not establish causal relationships.

---

## ⚙️ How to Run the Project

### 📋 Prerequisites

Install Python and Jupyter Notebook, JupyterLab, or use an environment such as Visual Studio Code.

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/bhawna1906/UCI-Online-Retail-EDA.git
cd UCI-Online-Retail-EDA
```

### 2️⃣ Install Dependencies

If a `requirements.txt` file is available:

```bash
pip install -r requirements.txt
```

Otherwise, install the libraries used by the notebook:

```bash
pip install pandas numpy matplotlib seaborn jupyter openpyxl
```

### 3️⃣ Download the Dataset

Download the Online Retail dataset from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/352/online+retail).

Place the dataset in the location expected by the notebook and update the file path if necessary.

### 4️⃣ Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the project's `.ipynb` file and run the cells sequentially.

**Note:** Ensure that the dataset filename, file path, and dependencies match the actual notebook configuration.

---

## 🔮 Future Improvements

- 👥 Perform customer segmentation using RFM analysis.
- 🔄 Analyze cancellation and return patterns at invoice and product levels.
- 💹 Incorporate product costs to evaluate profitability.
- 📊 Develop an interactive dashboard using Power BI or Streamlit.
- 📅 Extend the analysis with additional years of data to validate seasonal patterns.
- 🎯 Explore customer retention and product recommendation strategies.

---

## 🧠 Skills Demonstrated

- 🐍 Python Programming
- 🧹 Data Cleaning and Preprocessing
- 🐼 Data Manipulation with Pandas
- ⚙️ Feature Engineering
- 📊 Exploratory Data Analysis
- 📈 Data Visualization
- 📅 Time-Based Analysis
- 🌍 Geographical Sales Analysis
- 🏆 Product Performance Analysis
- 💼 Business Insight Generation
- 🎯 Data-Driven Decision-Making

---

## 👩‍💻 Author

**Bhawna**

Data Scientist

Feel free to connect with me on LinkedIn and see more of my projects!
