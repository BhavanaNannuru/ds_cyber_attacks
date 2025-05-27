# 🛡️ Cybersecurity Attacks Dataset - EDA & Data Cleaning

This project performs data cleaning and exploratory data analysis (EDA) on a real-world cybersecurity dataset. The goal is to prepare the data for insights that support threat intelligence and incident response.

---

## 📄 Dataset Source

**Kaggle**: [Cyber Security Attacks Dataset](https://www.kaggle.com/datasets/teamincribo/cyber-security-attacks/data)

---

## 📌 Objective

To conduct a **visual-driven analysis** of cybersecurity logs, focusing on threat indicators such as:

- Malware detection
- Proxy usage
- Firewall activity
- IDS/IPS alerts

---

## 🔍 Steps Performed

### 1. Data Loading & Initial Overview

- Imported necessary libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`
- Loaded the dataset using `pd.read_csv()`
- Inspected data types and structure:
  - `.info()`
  - `.describe()`
  - `.head()`
- Extracted and reviewed column names

### 2. Data Cleaning & Preprocessing

- Converted the `Timestamp` column to datetime format using `pd.to_datetime()`
- Checked for missing values using `.isnull().sum()`
- Calculated missing value percentages
- Imputed missing values in key columns by replacing with `'No'`:
  - `Malware Indicators`
  - `Alerts/Warnings`
  - `Proxy Information`
  - `Firewall Logs`
  - `IDS/IPS Alerts`

---

## ✅ Observations from Cleaning

- Key threat-related columns had missing data.
- All missing values were filled with `'No'` to maintain consistency.
- Timestamp parsing was successful for enabling time-based insights.

---

## 🧰 Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

