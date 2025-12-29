# 📊 Amazon Sales Data Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Pandas%20%7C%20Seaborn%20%7C%20WordCloud-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)
![License](https://img.shields.io/badge/License-Apache%202.0-lightgrey)

## 📝 Project Overview

This project is an **Exploratory Data Analysis (EDA)** of the Amazon Sales Dataset. The goal was to clean messy real-world data and uncover insights into pricing strategies, discount effectiveness, and customer satisfaction.

The analysis answers key questions such as:
* Does a higher discount percentage actually lead to better ratings?
* Which product categories have the most consistent quality?
* What are customers actually saying in their reviews? (Sentiment Analysis)

## 📂 Dataset

The dataset contains information on 1,000+ Amazon products, including:
* **Product Details:** ID, Name, Category
* **Pricing:** Actual Price, Discounted Price, Discount Percentage
* **Customer Feedback:** Rating, Rating Count, Review Content

## 🛠️ Tech Stack

* **Python**
* **Pandas:** For data manipulation and cleaning (handling string anomalies, type conversion).
* **NumPy:** For numerical operations.
* **Seaborn & Matplotlib:** For statistical data visualization.
* **WordCloud:** For text analysis of customer reviews.

## 🔍 Key Analysis & Workflow

### 1. Data Cleaning (The Heavy Lifting)
* **Handling Nulls:** Imputed missing ratings using the **Median** strategy to maintain statistical integrity.
* **Data Type Conversion:** Cleaned currency symbols (`₹`) and percentage signs (`%`) to convert columns to numeric types.
* **String Manipulation:** Split complex `Category` strings (e.g., *"Computers|Accessories|Cables"*) to extract the **Main Category** for broader analysis.

### 2. Exploratory Data Analysis (EDA)
* **Univariate Analysis:** Analyzed the distribution of ratings and prices.
* **Bivariate Analysis:** Explored the correlation between `Discount Percentage` and `Rating`.
* **Multivariate Analysis:** Created a **Violin Plot** to visualize rating density across different product categories.



**Rating Distribution by Category (Violin Plot)**
### 3. Visualizations
<img width="1006" height="660" alt="download" src="https://github.com/user-attachments/assets/6bf021f1-04ac-4a1c-b619-9604445ad846" />

**Customer Sentiment WordCloud**
<img width="790" height="429" alt="download" src="https://github.com/user-attachments/assets/85014e52-d142-4bf4-9422-4c04c28df769" />


## 💡 Key Findings

* **Pricing vs. Satisfaction:** There is a **weak correlation** between Discount Percentage and Rating. Offering massive discounts does not guarantee a 5-star review; product quality remains the primary driver.
* **Customer Sentiment:** The WordCloud analysis highlighted that customers prioritize reliability. Words like **"Quality"**, **"Good"**, **"Working"**, and **"Cable"** were most frequent.
* **Category Performance:** "Computers" and "Electronics" generally maintain high ratings (4.0+), though outliers exist. "Office Products" showed a wider variance in customer satisfaction.

## 🚀 How to Run

1.  Clone the repository:
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  Install dependencies:
    ```bash
    pip install pandas seaborn matplotlib wordcloud
    ```
3.  Open the Jupyter Notebook:
    ```bash
    jupyter notebook "Eda-on-amazon-sales-data.ipynb"
    ```

## 📜 License
This project is licensed under the Apache 2.0 License.

---
*Created by Kunal Saini*


