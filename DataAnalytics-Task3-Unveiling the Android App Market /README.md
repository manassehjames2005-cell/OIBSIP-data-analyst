# Task 3 – Unveiling the Android App Market (Android App Market Analysis)

## 📌 Project Overview

This project focuses on analyzing the Google Play Store ecosystem using Python and data analysis techniques.

The analysis covers app categories, ratings, installations, app size, pricing, estimated revenue, and user review sentiment. The objective is to understand patterns in the Android app market and identify useful insights for developers planning to launch a new application.

---

## 🎯 Objective

The main objectives of this project are:

* Clean and preprocess real-world Google Play Store data.
* Analyze the distribution of apps across different categories.
* Study app ratings and average ratings by category.
* Analyze the relationship between app size and number of installs.
* Compare free and paid applications.
* Analyze pricing trends for paid applications.
* Estimate revenue across app categories.
* Perform sentiment analysis on user reviews.
* Analyze positive, negative, and neutral sentiment by category.
* Generate data-driven insights for app developers.

---

## 🛠️ Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* TextBlob
* Plotly
* Jupyter Notebook

---

## 📂 Datasets

Two publicly available Google Play Store datasets were used:

1. **Google Play Store Apps Dataset**

   * Contains information about applications, categories, ratings, installs, size, type, price, and other app details.

2. **Google Play Store User Reviews Dataset**

   * Contains user reviews and sentiment-related information for applications.

---

## 🔧 Data Cleaning

The datasets were cleaned and prepared for analysis by performing the following operations:

* Checked the dataset structure and data types.
* Identified missing values.
* Removed duplicate records.
* Converted the `Installs` column from text format into numeric format.
* Removed special characters such as `+` and `,` from the `Installs` column.
* Converted the `Price` column into numeric format.
* Converted application size values into MB.
* Removed reviews with missing review text.

---

## 📊 Exploratory Data Analysis

### 1. App Category Analysis

The number of applications in each category was analyzed to identify categories with a large number of applications.

A bar chart was created to visualize the distribution of applications across categories.

### 2. Ratings Analysis

The distribution of application ratings was analyzed using a histogram.

Average ratings were also calculated for different application categories to understand differences in user ratings.

### 3. Size and Install Analysis

A scatter plot was created to investigate the relationship between application size and number of installs.

Correlation analysis was also performed to understand whether a relationship exists between these two variables.

### 4. Pricing Analysis

Applications were divided into:

* Free applications
* Paid applications

The distribution of paid application prices was analyzed using a histogram.

### 5. Estimated Revenue Analysis

Estimated revenue was calculated using:

**Estimated Revenue = Price × Installs**

The estimated revenue was then aggregated by application category to identify categories with higher estimated revenue.

> Note: The revenue calculation is only an estimate because the dataset contains approximate installation figures and does not represent actual company revenue.

---

## 💬 Sentiment Analysis

User reviews were analyzed using **TextBlob**.

Each review was classified into one of three sentiment categories:

* Positive
* Negative
* Neutral

The sentiment distribution was visualized using a count plot.

Sentiment was also analyzed by application category to identify categories with more positive and negative user feedback.

---

## 📈 Visualizations

The project includes the following visualizations:

* App distribution by category
* App rating distribution
* Average rating by category
* App size vs installs scatter plot
* Free vs paid application distribution
* Paid app price distribution
* Estimated revenue by category
* User review sentiment distribution
* Positive sentiment by category
* Negative sentiment by category
* Interactive Plotly visualization

---

## 🔍 Key Insights

The analysis provides the following types of insights:

1. **Category Competition**
   Categories with a large number of applications may represent highly competitive and saturated areas of the Google Play Store.

2. **User Feedback**
   Ratings and sentiment analysis provide useful information about user satisfaction and areas where application quality can be improved.

3. **Monetization Opportunities**
   Pricing, installations, and estimated revenue analysis can help developers understand different monetization patterns across categories.

---

## 💡 Recommendations for App Developers

Based on the analysis, developers can:

* Study category competition before launching a new application.
* Analyze user ratings and reviews to identify common user expectations.
* Focus on improving application quality and user experience.
* Evaluate pricing strategies using market data.
* Consider both installation potential and monetization opportunities.
* Use negative feedback to identify areas for future improvements.

---

## 📁 Project Structure

```text
Task4-AndroidAppMarket/
│
├── googleplaystore.csv
├── googleplaystore_user_reviews.csv
├── Android_App_Market_Analysis.ipynb
└── README.md
```

---

## ▶️ How to Run

1. Download or clone this repository.
2. Open the project folder.
3. Open `Android_App_Market_Analysis.ipynb` using Jupyter Notebook.
4. Install the required Python libraries if necessary.
5. Run the notebook cells sequentially.
6. Review the generated visualizations and analysis results.

---

## 👨‍💻 Project Author

**Manasseh M**

Data Analytics Project – Task 3

