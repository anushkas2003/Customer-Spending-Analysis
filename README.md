
# 📊 Customer Spending Analysis Project

This repository contains the code and analysis for a deep dive into customer spending and purchasing behavior. The goal is to identify high-value customers, understand purchase frequency, and analyze sales distribution across different product categories to inform strategic business decisions.

---

## 🎯 Project Goals

The primary objectives of this analysis were to:
1.  **Identify** the top customers based on their total monetary spend.
2.  **Analyze** the frequency of purchases across the customer base.
3.  **Determine** the sales contribution of different product categories.
4.  **Visualize** key findings for actionable insights.

---

## 🛠️ Technologies and Libraries

This project is built using Python for data analysis and visualization.

| Category | Tool/Library | Purpose |
| :--- | :--- | :--- |
| **Language** | Python | Core programming language |
| **Data Analysis** | Pandas | Data manipulation, grouping, and aggregation |
| **Visualization** | Matplotlib (pyplot) | Creating statistical plots (bar charts, pie charts) |

---

## 🔍 Key Analysis Steps and Findings

The analysis was executed in distinct phases, resulting in the following key insights:

### 1. Customer Purchase Frequency Analysis
* **Method:** Calculated the number of transactions per individual `Customer_ID`.
* **Result:** Provides a baseline understanding of how distributed purchases are, indicating whether sales are driven by a few frequent shoppers or many single-purchase customers.

### 2. Total Spend Per Customer
* **Method:** Aggregated the total `Spend` for every `Customer_ID`.

### 3. Top 5 High-Spending Customers (Monetary Value)

| Customer_ID | Spend | Rank |
| :--- | :--- | :--- |
| **1011** | **1700** | **1** |
| 1019 | 1600 | 2 |
| 1005 | 1500 | 3 |
| 1015 | 1400 | 4 |
| 1009 | 1300 | 5 |

* **Visualization:** A **pie chart** was used to illustrate the proportional contribution of these top 5 customers to the total spend (as shown in the code: `top_customers.plot(kind="pie", ...)`)

### 4. Sales by Product Category
* **Method:** Grouped sales data by `Product_Category` and summed the `Spend` to determine total revenue per category.
* **Key Finding:** **Clothing** is the leading product category by sales volume.

| Product_Category | Total Sales |
| :--- | :--- |
| **Clothing** | **7780** |
| Electronics | 5700 |
| Groceries | 5600 |

---

## 🚀 How to Run the Project

1.  **Clone the Repository:**
    ```bash
    git clone [YOUR_REPO_URL]
    cd customer-spending-analysis
    ```
2.  **Install Dependencies:**
    ```bash
    pip install pandas matplotlib
    ```
3.  **Execute the Analysis Script:**
    *(Assuming your main script is named `analysis.py`)*
    ```bash
    python analysis.py
    ```

---

## ✨ Future Enhancements

* Implement a full **RFM (Recency, Frequency, Monetary)** segmentation model.
* Conduct **Cohort Analysis** to track customer value over time.
* Integrate a machine learning model to predict **Customer Lifetime Value (CLV)**.
