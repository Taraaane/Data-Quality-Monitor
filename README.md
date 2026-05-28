# 🔍 Automated Data Quality Monitor

An automated Python utility for profiling and monitoring data quality in tabular datasets. This tool evaluates datasets against predefined rules and thresholds, generating a comprehensive and visually appealing HTML report to help Data Analysts and Data Scientists quickly identify data inconsistencies.

## 🚀 Key Features

* **Missing Value Detection:** Calculates null rates per column and flags violations based on customizable thresholds.
* **Duplicate Row Identification:** Detects identical records and provides samples of duplicated rows.
* **Outlier & Range Validation:** Uses Statistical methods (IQR or Z-Score) to find outliers and checks values against predefined logical minimums and maximums (e.g., negative blood pressure).
* **Categorical Validation:** Ensures categorical variables strictly match an allowed list of values (e.g., standardizing text inputs).
* **Automated HTML Reporting:** Uses `Jinja2` to generate a responsive, standalone HTML report with a clean UI, summarizing the overall data health score and detailed metrics.

## 🛠️ Tech Stack

* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`, `scipy`
* **Report Generation:** `Jinja2`, HTML/CSS

## 📊 About the Sample Data

This repository includes a data generation script within the notebook that creates a dummy `Healthcare Patient Records` dataset. Intentional errors (such as BMI = 999.0, negative blood pressure, and missing values) are injected into the dataset to demonstrate the script's detection capabilities.

## ⚙️ How to Use

1. Clone the repository.
2. Ensure you have the required libraries installed (`pandas`, `numpy`, `scipy`, `jinja2`).
3. Run the `Data_Quality.ipynb` Jupyter Notebook.
4. The notebook will automatically generate a timestamped `.html` report in the same directory.
