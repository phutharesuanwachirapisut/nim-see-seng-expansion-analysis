# Logistics Branch Expansion Analysis: Phrae vs. Mae Hong Son

This repository contains the data analysis, preprocessing scripts, and findings for evaluating the investment feasibility of opening a new logistics branch for Nim See Seng 1988 Co., Ltd.[cite: 109]. The project compares two specific provinces in Northern Thailand: Phrae and Mae Hong Son[cite: 109]. 

## 📌 Project Overview
The objective of this study is to analyze economic data and delivery volumes to recommend the best location for a new branch expansion[cite: 113]. The analysis balances pure profitability metrics with the company's ESG (Environmental, Social, and Governance) policies[cite: 114].

The project utilizes logistics data spanning from January 1, 2024, to June 30, 2024, alongside regional economic indicators (such as GDP per capita)[cite: 113, 114].

## 🛠️ Data Preprocessing & Methodology
Data preparation was handled using Python and the `pandas` library[cite: 124]. 

Key steps in the preprocessing pipeline (`DS_Project.ipynb`) include:
* **Data Cleaning:** Removing irrelevant columns and handling null values in receiver data[cite: 124].
* **Machine Learning Imputation:** A K-Nearest Neighbors (KNN) Classifier was utilized to predict and fill missing values in the district column (`CONSIGNEE_AMPHUR`)[cite: 124].
* **Feature Engineering:** Utilizing the destination code (`DEST_CODE`) as a key variable to accurately map missing location data[cite: 124].
* **Data Filtering:** Isolating data strictly related to Phrae and Mae Hong Son provinces for targeted analysis[cite: 125, 126].

## 📊 Data Visualization & Analysis
Following the preprocessing in Python, the cleaned data was exported for visualization.
* **Power BI Dashboards:** Interactive dashboards were created to compare the proportion of goods transported and regional economic data across different districts[cite: 133].
* **Metrics Tracked:** Total order volume (`QTY`), average income vs. order quantity, and GDP growth by year[cite: 126, 128, 133].

## 💡 Key Findings & Conclusion
The analysis revealed a strategic trade-off between the two provinces:
* **Phrae (Profitability Focus):** Phrae has a larger population (approx. 430,000) and a significantly higher volume of received goods[cite: 172]. Opening a branch in Phrae has a higher likelihood of generating immediate profit due to higher average income and spending[cite: 172]. However, the data shows significant inequality, with goods highly concentrated in the capital district (Mueang Phrae)[cite: 172].
* **Mae Hong Son (ESG Focus):** While Mae Hong Son has a smaller population (approx. 290,000) and more volatile economic growth, order deliveries are much better distributed across its districts[cite: 172]. Opening a branch here strongly aligns with ESG concepts by creating non-agricultural jobs, actively reducing income inequality, and potentially helping to reduce seasonal agricultural burning[cite: 114, 172].

**Conclusion:** While Phrae represents a more stable economic investment, Mae Hong Son represents a strategic investment in social equity and ESG principles[cite: 114, 173].

## 📂 Repository Structure
* `DS_Project.ipynb`: The primary Jupyter Notebook containing the data cleaning and KNN imputation code.
* `Unserious BACON time_Poster.jpg`: A visual summary poster of the project's methodology and Power BI dashboards.
* `Unserious BACON Time.pdf`: The detailed research summary and conclusions.