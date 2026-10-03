# TASK 2 · Customer Segmentation Analysis

## 📌 Project Overview

This project focuses on segmenting e-commerce customers based on their purchasing behaviour using **RFM Analysis** and the **K-Means Clustering** algorithm.

The objective is to identify different groups of customers based on their **Recency, Frequency, and Monetary value** and provide suitable marketing recommendations for each customer segment.

---

## 🎯 Objective

To apply clustering techniques to an e-commerce customer dataset and identify distinct customer segments based on purchasing behaviour.

The analysis helps businesses understand their customers and develop targeted marketing strategies.

---

## 🛠️ Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

## 📊 Dataset

**Dataset:** Online Retail Dataset

The dataset contains transaction-level information from an online retail store.

### Important Features

| Column      | Description                  |
| ----------- | ---------------------------- |
| InvoiceNo   | Unique invoice number        |
| StockCode   | Product code                 |
| Description | Product description          |
| Quantity    | Number of products purchased |
| InvoiceDate | Date and time of transaction |
| UnitPrice   | Price per unit               |
| CustomerID  | Unique customer identifier   |
| Country     | Customer's country           |

---

## 🔍 Project Workflow

The project follows these steps:

1. Load and inspect the dataset
2. Check missing values and duplicate records
3. Handle inconsistent and invalid data
4. Calculate total purchase amount
5. Perform descriptive statistics
6. Perform RFM analysis
7. Select Recency, Frequency and Monetary features
8. Standardize the features using StandardScaler
9. Apply the Elbow Method
10. Determine the suitable number of clusters
11. Apply K-Means clustering
12. Visualize customer segments
13. Profile each customer cluster
14. Analyze customer distribution
15. Provide marketing recommendations

---

## 🧹 Data Cleaning

The dataset was inspected for missing values, duplicate records and inconsistent transactions.

The following cleaning operations were performed:

* Removed records with missing `CustomerID`
* Removed cancelled transactions
* Removed transactions with zero or negative quantity
* Removed transactions with zero or negative unit price
* Removed duplicate records

---

## 💰 Total Purchase Value

A new feature called `TotalAmount` was created using:

**TotalAmount = Quantity × UnitPrice**

This value represents the total amount spent in each transaction.

---

## 📈 RFM Analysis

RFM analysis was used to understand customer purchasing behaviour.

### Recency

Measures how recently a customer made a purchase.

A lower Recency value indicates a more recent purchase.

### Frequency

Measures how frequently a customer made purchases.

A higher Frequency value indicates more frequent purchases.

### Monetary

Measures the total amount spent by a customer.

A higher Monetary value indicates higher customer spending.

The three RFM features were used as the main behavioural features for clustering.

---

## ⚙️ Feature Standardization

Since the RFM features have different numerical scales, **StandardScaler** from Scikit-learn was used to standardize the features before applying K-Means clustering.

The standardized features were:

* Recency
* Frequency
* Monetary

---

## 📉 Elbow Method

The **Elbow Method** was used to determine an appropriate number of clusters for the K-Means algorithm.

The method compares the number of clusters with the model's inertia and identifies the point where adding additional clusters provides less improvement.

The selected K value was then used for the final K-Means model.

### Elbow Method

![Elbow Method](screenshots/04-elbow-method.png)

---

## 🤖 K-Means Clustering

The K-Means algorithm was applied to the standardized RFM features.

Each customer was assigned to a cluster based on similarities in their purchasing behaviour.

The resulting clusters represent different types of customers.

---

## 📊 Customer Segment Visualizations

### Recency vs Monetary

![Recency vs Monetary](screenshots/07-recency-monetary.png)

### Frequency vs Monetary

![Frequency vs Monetary](screenshots/08-frequency-monetary.png)

These visualizations show how customers are distributed across the identified segments.

---

## 👥 Cluster Distribution

The number of customers in each cluster was visualized using a bar chart.

![Cluster Distribution](screenshots/05-cluster-distribution.png)

This helps identify the size of each customer segment.

---

## 📋 Cluster Profiling

The mean Recency, Frequency and Monetary values were calculated for each cluster to understand the characteristics of different customer groups.

![Cluster Profile](screenshots/06-cluster-profile.png)

The clusters were interpreted based on their purchasing behaviour.

For example:

* Customers with low Recency and high Monetary value may represent highly engaged and valuable customers.
* Customers with high Recency and low purchasing activity may require re-engagement campaigns.
* Customers with moderate purchasing behaviour may respond to cross-selling and promotional campaigns.

---

## 💡 Marketing Recommendations

Based on the customer segments, different marketing strategies can be applied.

### High Value Customers

* Provide loyalty rewards
* Offer premium products
* Provide exclusive offers
* Use personalized recommendations

### Loyal Customers

* Introduce loyalty programs
* Provide repeat-purchase offers
* Send personalized promotions

### Regular Customers

* Use cross-selling strategies
* Recommend related products
* Provide promotional discounts

### At-Risk Customers

* Launch customer win-back campaigns
* Provide limited-time discounts
* Send personalized re-engagement offers

> The exact segment names and recommendations are based on the characteristics observed in the final cluster profile.

---

## 📌 Key Insights

The analysis helps identify customer groups based on their purchasing behaviour.

RFM analysis provides three important behavioural measures:

* **Recency** helps identify recently active and inactive customers.
* **Frequency** identifies customers who purchase more frequently.
* **Monetary** identifies customers who contribute higher revenue.

K-Means clustering groups customers with similar purchasing patterns, making it easier to design targeted marketing strategies.

---

## 📁 Project Structure

```text
Task2-CustomerSegmentation/
│
├── Task2-CustomerSegmentation.ipynb
├── Online Retail.xlsx
├── README.md
│
└── screenshots/

---

## 🏁 Conclusion

This project demonstrates how **RFM analysis and K-Means clustering** can be used to segment e-commerce customers based on purchasing behaviour.

The identified customer segments provide useful insights for targeted marketing, customer retention, loyalty programs, personalized recommendations and customer re-engagement strategies.

---

