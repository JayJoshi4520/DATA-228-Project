# Analyzing Fashion Trends and Customer Preferences Using Big Data Technologies

This repository contains the code and documentation for the project **"Analyzing Fashion Trends and Customer Preferences Using Big Data Technologies"**, developed as part of the course project for DATA 228 at San Jose State University. The project leverages the **Fashion Product Images dataset from Kaggle** to uncover hidden insights into fashion trends and customer preferences using advanced big data technologies like Hadoop and Apache Spark.
## Introduction

The fashion industry is undergoing a digital transformation, with consumer behavior and preferences changing rapidly. This project addresses the challenges faced by fashion retailers in processing large, varied datasets and extracting actionable insights. By analyzing over **44,000 images** and metadata, the project aims to:
- Identify patterns in fashion trends across demographics and seasons.
- Predict product popularity and customer preferences based on attributes like color, material, and style.
- Optimize inventory and marketing strategies for fashion retailers.

---

## Dataset Overview

The **Fashion Product Images Dataset** consists of:
- **Images:** 44,400 high-resolution fashion product images in JPG format.
- **Metadata:** Product details stored in JSON files and CSV files, including attributes like categories, display names, and colors.

### Dataset Structure:
- **Directories:**
  - `images/`: Contains product images.
  - `styles/`: Contains metadata files in JSON format.
- **Files:**
  - `styles.csv`: Maps product IDs to attributes like categories, colors, and names.
  - `images.csv`: Provides supplementary image metadata.
- **Size:** Approximately 23.1 GB.

---

## Technologies Used

The project leverages the following technologies:
- **Apache Hadoop**: For distributed storage and resource management.
  - **HDFS**: Stores large datasets in a fault-tolerant manner.
  - **YARN**: Manages computational resources efficiently.
- **Apache Spark**: For distributed data processing and machine learning.
  - **Spark SQL**: For structured data analysis.
  - **Spark MLlib**: For implementing machine learning models.
- **PySpark**: For developing scalable data processing scripts.
- **Pandas** and **NumPy**: For exploratory data analysis (EDA).
- **Linear Regression**: For predictive modeling of product popularity.

---

## Project Workflow

### Data Pipeline:
1. **Data Storage**: Uploading data to HDFS using `hdfs dfs -put` command.
2. **Data Preprocessing**: Cleaning and transforming JSON and CSV files into structured formats.
3. **Exploratory Data Analysis (EDA)**:
   - Analyzing unique values, null values, and trends in the dataset.
   - Extracting metadata like image sizes, formats, and color modes.
4. **Machine Learning**:
   - Implementing a Linear Regression model using Spark MLlib to predict product popularity.
5. **Insights and Recommendations**:
   - Identifying popular colors, categories, and seasonal trends.
   - Optimizing inventory and marketing strategies based on data-driven insights.

---

## Setup and Installation

### Prerequisites:
- Hadoop (HDFS and YARN configured)
- Apache Spark
- Python 3.x
- PySpark
- Kaggle API (for downloading the dataset)

### Steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/JayJoshi4520/DATA-228-Project.git
   cd DATA-228-Project

Usage:

Running the Data Pipeline:
Start Hadoop and Spark services.
Execute the data preprocessing scripts to clean and structure the data:
spark-submit preprocessing.py
Run EDA scripts to analyze trends and insights:
spark-submit eda.py
Train and evaluate the Linear Regression model:
spark-submit regression_model.py
Results and Insights

Key Findings:
Popular Categories:
Topwear (15,405 entries) and Shoes (7,344 entries) dominate the dataset.
Color Trends:
Black and White are the most popular colors, reflecting a preference for neutral tones.
Seasonal Insights:
Summer products are the most represented, followed by Fall and Winter.
Revenue Optimization:
Low discounts (<10%) are most effective, generating maximum sales and revenue.
Customer Segmentation:
Strategies to move medium spenders to high spenders can increase profitability.
Model Performance:
Linear Regression Model:
R² Value: 0.999 (indicating high predictive accuracy).
Root Mean Square Error (RMSE): Very low, indicating precise predictions.

Contributors
Avirit Singh (avirit.singh@sjsu.edu)
Jay Joshi (jaynarendrabhai.joshi@sjsu.edu)
