# 🌾 Agricultural Risk Assessment & Scheme Recommendation System using FSVI

> A data-driven agricultural risk analytics system that calculates the **Farm Shock Vulnerability Index (FSVI)** and recommends suitable **Government schemes** for Indian farmers based on the dominant factor contributing to their financial vulnerability.

---

## 📖 Overview

Agriculture in India faces multiple interconnected risks, including **market price fluctuations, crop yield variability, weather uncertainty, and financial stress**. Traditional approaches often analyze these risks independently, making it difficult to assess the overall financial vulnerability of farmers.

This project proposes a **Farm Shock Vulnerability Index (FSVI)** that integrates multiple agricultural risk indicators into a single composite score. Based on the calculated FSVI and the dominant contributing risk, the system recommends **Central, State, and District Government schemes** to help farmers reduce financial losses and improve resilience.

The project uses **real government datasets** collected for **Sehore District, Madhya Pradesh**, covering both **Kharif** and **Rabi** seasons.

---

## 🎯 Objectives

- Assess farmers' financial vulnerability using multiple agricultural indicators.
- Integrate heterogeneous government datasets into a unified analytical framework.
- Calculate a normalized **Farm Shock Vulnerability Index (FSVI)**.
- Categorize agricultural seasons into different financial risk levels.
- Recommend suitable Government schemes based on the dominant risk factor.
- Generate automated policy-ready reports for decision-makers.

---

## 🚜 Problem Statement

Farmers frequently suffer financial losses due to the combined impact of:

- 🌧 Weather uncertainty
- 🌾 Crop yield fluctuations
- 💰 Market price volatility
- 📈 Rising cultivation costs

Although these factors are interconnected, they are generally analyzed independently. This project combines all four dimensions into a single vulnerability index, enabling a comprehensive assessment of agricultural financial risk and supporting targeted intervention strategies.

---

## 📂 Data Sources

| Dataset | Source |
|----------|--------|
| Market Price Data | Agmarknet |
| Crop Yield Data | DES Madhya Pradesh / UPAG |
| Weather Data | IMD / MOSDAC |
| Financial Stress Proxy | Consumer Price Index (CPI) |

---

## 🏗️ Project Workflow

### Pipeline

1. Data Collection
2. Data Integration
3. Missing Value Handling
4. Data Cleaning
5. Standardization
6. Min-Max Normalization
7. Risk Score Construction
8. Weight Assignment
9. FSVI Calculation
10. Risk Classification
11. Government Scheme Recommendation

---

## 📊 Risk Components

The FSVI is calculated using four normalized risk indicators.

### 📈 Price Risk (MPR)

Measures market instability using deviations between MSP and market realization.

### 🌾 Yield Risk (CYD)

Captures crop production variability using historical yield deviations.

### 🌧 Weather Risk (WSI)

Measures climatic stress using rainfall deviations and weather anomalies.

### 💸 Financial Stress (FSP)

Represents increasing cultivation costs using inflation (CPI) trends.

---

## 🧮 Farm Shock Vulnerability Index (FSVI)

The FSVI is calculated as the equal-weighted average of four normalized risk components.

```text
FSVI = (Price Risk + Yield Risk + Weather Risk + Financial Stress) / 4
```

Each component is normalized to a range of **0–1** using Min-Max Normalization.

---

## 🚦 Risk Classification

| FSVI Score | Risk Level |
|------------|------------|
| 0.00 – 0.30 | 🟢 Low Risk |
| 0.30 – 0.60 | 🟡 Moderate Risk |
| 0.60 – 1.00 | 🔴 High Risk |

---

## 🤖 Recommendation System

The recommendation engine identifies the **highest contributing risk factor** and suggests relevant Government interventions.

### Market Price Risk

- PM-AASHA
- MSP Procurement
- Bhavantar Bhugtan Yojana

### Weather Risk

- PMFBY Crop Insurance
- Irrigation Support
- Balram Talab Scheme

### Financial Stress

- Kisan Credit Card (KCC)
- Interest Subsidy Schemes
- District Cooperative Bank Assistance

### Yield Risk

- Krishi Vigyan Kendra (KVK) Programs
- Soil Health Card Scheme
- Seed Improvement Initiatives

---

## ✨ Features

- Multi-source Government data integration
- Composite Farm Shock Vulnerability Index (FSVI)
- Financial risk assessment
- Automated risk classification
- Rule-based Government scheme recommendation engine
- Excel dashboard generation
- Season-wise trend analysis
- Explainable decision support

---


## 📤 Output

The system generates:

- ✅ Farm Shock Vulnerability Index (FSVI)
- ✅ Risk Category
- ✅ Dominant Risk Factor
- ✅ Government Scheme Recommendations
- ✅ Excel Dashboard
- ✅ Season-wise Risk Trend Analysis

---

## 💻 Tech Stack

- Python
- Pandas
- NumPy
- OpenPyXL
- Excel
- Jupyter Notebook

---

## 🎯 Applications

- Agricultural Risk Assessment
- Government Policy Planning
- Farmer Decision Support
- Financial Vulnerability Analysis
- Climate Risk Monitoring
- Agricultural Research

---

## 🚀 Future Enhancements

- Machine Learning-based adaptive weight calculation
- GIS-based district risk visualization
- Satellite imagery integration
- Weather forecasting APIs
- Streamlit web application
- Real-time recommendation dashboard

---
