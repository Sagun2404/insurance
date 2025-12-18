# 🏦 Insurance Analytics Power BI Dashboard

## 📌 Project Overview
This project is an **end-to-end Insurance Analytics dashboard** built using **Power BI**. The report provides a consolidated view of insurance policies, premiums, coverage amounts, and claims performance, enabling stakeholders to monitor operational efficiency and make data-driven decisions.

The dashboard is designed with **interactive filters**, **KPIs**, and **drill-through analysis** to explore policy-level details from a high-level summary.

---

## 🧩 Problem Statement

This project demonstrates the ability to translate **raw insurance data into actionable business insights** using Power BI. The dashboard is designed for business users, analysts, and decision-makers who need quick visibility into insurance performance without writing queries.

The report addresses common business problems such as:
Insurance companies deal with large volumes of policy and claims data spread across multiple dimensions such as **policy type, customer demographics, claim status, and policy activity**.

The key challenges addressed by this project are:
- Lack of **centralized visibility** into premiums, coverage, and claims
- Difficulty tracking **active vs inactive policies**
- Limited insight into **claim outcomes** (settled, rejected, pending)
- No easy way to analyze **claims by age group and policy type**

This dashboard solves these problems by presenting a **single analytical view** that allows stakeholders to:
- Track overall insurance performance
- Identify high-risk or high-claim segments
- Drill down from summary metrics to individual policy records

---

## 🎯 Project Objectives
- Monitor **total premium, coverage, and claim amounts**
- Analyze **premium distribution by policy type**
- Track **active vs inactive policies**
- Evaluate **claim status distribution**
- Understand **claim amounts by age group**
- Enable **policy-level drill-through analysis**

---

## 📈 Key Performance Indicators (KPIs)

| KPI | Description | Business Value |
|---|---|---|
| **Total Premium Amount** | Sum of all premiums collected | Measures revenue generation |
| **Total Coverage Amount** | Total insured coverage value | Indicates company risk exposure |
| **Total Claim Amount** | Sum of all claims raised | Helps assess claim liability |
| **Active Policies %** | Ratio of active to inactive policies | Indicates customer retention |
| **Claims by Status** | Count of settled, rejected, pending claims | Measures operational efficiency |
| **Premium by Policy Type** | Premium distribution across policy categories | Identifies top-performing products |
| **Claim Amount by Age Group** | Claim value by customer age group | Helps in risk profiling |

---

## 📊 Dashboard Pages

### 🔹 Page 1: Insurance Report (Overview)
Provides a high-level snapshot of the insurance business.

**Key Visuals:**
- KPI Cards: Premium Amount, Coverage Amount, Claim Amount
- Premium Amount by Policy Type (Bar Chart)
- Active vs Inactive Policies (Donut Chart)
- Number of Claims by Claim Status
- Claim Amount by Age Group
- Gender-wise customer distribution

**Filters Available:**
- Policy Number
- Customer ID
- Claim Number

---

### 🔹 Page 2: Policy-Level Drill Through
This page enables **detailed analysis at the individual policy level** and is accessed via **drill-through from the “Premium Amount by Policy Type” visual**.

**Details Included:**
- Policy Type & Policy Number
- Customer ID & Gender
- Active / Inactive status
- Coverage Amount
- Claim Number & Claim Status
- Claim Date

This allows analysts to move from **aggregated metrics to raw records** seamlessly.

---

## 💡 Key Insights & Findings

The dashboard reveals several **actionable business insights** that can help insurance stakeholders improve decision-making:

- **Travel insurance generates the highest premium**, making it the most profitable policy type and a key revenue driver.
- **Active policies account for ~73%** of the total portfolio, indicating healthy customer retention but also highlighting scope to re-engage inactive customers.
- A **significant number of claims are rejected**, suggesting potential issues in claim eligibility checks or documentation quality.
- **Adult customers contribute the highest claim amount**, indicating a higher risk exposure compared to young customers.
- **Pending claims represent operational backlog**, which can impact customer satisfaction if not resolved quickly.
- Claim settlements vary noticeably by **policy type**, helping identify products with higher claim ratios.

These insights enable management to:
- Optimize policy offerings
- Improve claim processing efficiency
- Focus risk management strategies on high-claim segments

---

## 🗂 Dataset Description

**Key Fields Used:**
- `PolicyType`
- `PolicyNumber`
- `CustomerID`
- `Gender`
- `Active / Inactive`
- `CoverageAmount`
- `ClaimNumber`
- `ClaimStatus`
- `ClaimDate`

The dataset represents **policy and claim transactions** across multiple insurance categories such as **Travel, Health, Auto, Life, and Home**.

---

## 🧹 Data Cleaning & Preparation Steps
The following data preparation steps were performed in **Power Query**:

1. **Data Type Validation**
   - Converted `ClaimDate` to Date format
   - Ensured monetary fields (`Premium`, `CoverageAmount`, `ClaimAmount`) were numeric

2. **Standardization**
   - Normalized categorical values such as `PolicyType`, `ClaimStatus`, and `Gender`
   - Ensured consistent naming for Active / Inactive status

3. **Missing Value Handling**
   - Checked for null values in critical columns
   - Replaced missing claim amounts with 0 where applicable

4. **Derived Columns**
   - Created **Age Group** buckets (Young, Adult, Old)
   - Created calculated measures for total premiums, claims, and coverage

5. **Model Optimization**
   - Removed duplicate records
   - Kept only analysis-relevant columns

---

## 🛠 Tools & Technologies Used
- **Power BI Desktop** – Data modeling & visualization
- **Power Query** – Data cleaning and transformation
- **DAX** – KPI calculations and measures
- **GitHub** – Version control and project sharing

---

## 🖼 Project Screenshots

### Dashboard Overview
![Insurance Dashboard Overview](Screenshot 2025-12-18 160003.png)

### Drill-Through Page (Policy-Level Details)
![Drill Through Page](Screenshot 2025-12-18 160056.png)



---

## 🚀 How to Use the Report
1. Open the `.pbix` file in Power BI Desktop
2. Use slicers to filter by Policy, Customer, or Claim
3. Click on any **Policy Type bar** to drill through to detailed records
4. Analyze trends and export insights as needed

---



