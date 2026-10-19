# 🐔 Poultry Farm Interactive Excel Dashboard System

![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX_Measures-0176D3?style=for-the-badge&logo=analytics&logoColor=white)
![Status](https://img.shields.io/badge/Project_Status-Completed-success?style=for-the-badge)

---
![Healthcare Data Cleaning and Quality Assessment](https://github.com/Molla-Adugna/poultry-farm-interactive-excel-dashboard-system/blob/main/Assets/MFIPF_Dashboard_Thumbnail_Updated_2.png?raw=true)
## 📊 Project Overview

**MFIPF Poultry Farm Interactive Excel Dashboard System** is a comprehensive Excel-based Business Intelligence (BI) solution developed for an agricultural enterprise owned by **Meseret Fekade**.

The system transforms raw operational, production, feed consumption, mortality, flock performance, and financial data into interactive, executive-ready dashboards designed to drive data-informed decision-making.

### 🛠️ Core Capabilities Demonstrated
- **ETL & Data Transformation:** Power Query
- **Data Modeling:** Power Pivot (Star-schema concepts)
- **Advanced Analytics:** DAX (Data Analysis Expressions)
- **Data Visualization:** Pivot Tables, Dynamic Pivot Charts & Interactive Slicers
- **UX/UI Design:** Custom navigation menu, user control safeguards, and modular layout

> 💡 **Client Consent Note:** Permission has been granted by the client to showcase this sanitized project as part of my professional data analytics portfolio.

---

## 🎯 Key Objectives

This solution separates raw data entry from analytics reporting to maximize workbook performance, data integrity, and end-user accessibility.

- 📝 **Streamlined Data Entry:** Simplified inputs for daily operational logs without disrupting analytics.
- ⚙️ **Automated Pipeline:** Self-contained Power Query transformation pipeline.
- 📈 **KPI & Trend Monitoring:** Real-time visibility into egg production lay rates, mortality percentages, and flock age trends.
- 🌾 **Feed Efficiency Tracking:** Correlation analysis between feed consumption costs and daily production yield.
- 💰 **Financial Performance Analytics:** Consolidated views of revenues, operational expenses, and net profit margins.

---

## 📁 Project Structure

```text
MFIPF_Dashboard_System/
│
├── Tables/
│   ├── MFIPF_CalendarTable_2026.xlsx   # Dedicated Date Dimension Table
│   └── MFIPF_Data_Table_2026.xlsx      # Daily Operational Data Entry Workbook
│
├── MFIPF_Dashboard.xlsx                # Primary Interactive Analytics Environment
└── መሰረትፈቃደ የተቀናጀ የዶሮ ሃብት ልማት.pdf    # Comprehensive User & Technical Guide
```

## 📂 File Breakdown & Data Workflow
```text
1️⃣ MFIPF_CalendarTable_2026.xlsx  
```  

Central date dimension within the Data Model used for Time Intelligence calculations, enabling seamlessly linked Monthly, Quarterly, and Yearly comparative analysis.

```text
2️⃣ MFIPF_Data_Table_2026.xlsx  
```
Dedicated client data-entry workbook. To avoid file bloat and reporting errors, no dashboard logic resides here.

- Tracked Metrics: Daily Egg Production, Feed Consumed (kg), Mortality Count, Sales Volume, Operational Expenses, and Flock Metadata.  

### 👤 User Workflow:
1. Open the Data Table file.
2. Enter daily records.
3. Save the workbook.
4. Close the workbook.

(No dashboard interaction occurs within this file.)
```text
3️⃣ MFIPF_Dashboard.xlsx  
```  
The core business intelligence suite housing transformed data, DAX models, and user dashboards:

  - Dashboards: Home Summary, Production Analytics, Feed Management, Financial Analytics.
  - Backend: Hidden & protected Analysis Sheet containing core dynamic pivot tables and query connections.
## 🔄 End-to-End System Architecture
The reporting workflow follows the architecture below:
```text
  Raw Data Entry
│
▼
MFIPF_Data_Table_2026
│
▼
Power Query
│
▼
Data Transformation
│
▼
Power Pivot Data Model
│
▼
DAX Measures & Calculated Columns
│
▼
Pivot Tables & Charts
│
▼
Interactive Dashboards
```  
## ⚙️ Development Highlights
### Step 1: Data Architecture & ETL
- Designed decoupled data entry sheets stored in a standardized directory structure.
- Utilized Power Query for automated cleaning, column standardizations, data type casting, and query folding/optimization.
### Step 2: Data Modeling & DAX Engine
- Established one-to-many relationship between Calendar Table and Main Data Table.
- Created robust DAX Measures for dynamic metrics:
   - Lay Rate Percentage (\%)
   - Feed Conversion Efficiency
   - Period-over-Period Revenue & Expense Growth
   - Flock Age & Mortality Tracking
  
  ```text
   Calendar Table [1] ─── (1:N) ───► [*] Main Data Table
  ```
  

### Step 3: Security & Usability Safeguards
- Analysis Layer Isolation: Hidden and protected backend sheet to prevent accidental formula overwrites.
- Controlled User Layer: Dashboards remain locked for layout stability while keeping Slicers and Navigation Hyperlinks fully functional.
## 📈 Interactive Dashboards Overview

| Dashboard | Core Metrics & Insights |
| :--- | :--- |
| **🏠 Home Dashboard** | Executive summary, high-level KPIs, operational snapshot, and high-priority alerts. |
| **🥚 Production Dashboard** | Daily egg yields, lay rate tracking curves, flock age distribution, and mortality rate monitoring. |
| **🌾 Feed Management** | Daily feed consumption volume (kg), feed cost variance, and feed efficiency ratios. |
| **💰 Financial Dashboard** | Gross revenue streams, categorical operational expenses, net profit, and financial trend comparisons. |

## 📸 Dashboard Screenshots

| View | Asset Preview |
| :--- | :--- |
| **Home Dashboard** | `![Home Dashboard](images/home_dashboard.png)` |
| **Production Dashboard** | `![Production Dashboard](images/production_dashboard.png)` |
| **Feed Management** | `![Feed Dashboard](images/feed_dashboard.png)` |
| **Financial Dashboard** | `![Financial Dashboard](images/financial_dashboard.png)` |

---
## 🔒 System Refresh & Maintenance

### Standard Data Refresh Instructions:
1. Open `MFIPF_Dashboard.xlsx`.
2. Navigate to the ribbon/button and select **Refresh All Data**.
3. Allow Power Query to execute background connections.

> 🛠️ **Troubleshooting Blank Visuals:**  
> *If KPI cards or charts display blank values after a refresh, an isolated slicer combination may still be active. Clear all filters by clicking the **Clear Filter (X)** button on top of each Slicer panel.*  

---


## 🛠 Technologies & Tools Used

| Domain | Technology / Tool |
| :--- | :--- |
| **Spreadsheet Engine** | Microsoft Excel |
| **Data Ingestion & ETL** | Power Query |
| **Data Modeling** | Power Pivot (Data Model) |
| **Analytics Engine** | DAX (Data Analysis Expressions) |
| **Visualization** | Pivot Tables, Dynamic Charts, Custom Slicers |
| **Navigation** | Form Controls & Hyperlink Logic |
| **Documentation** | PDF User Guide & Markdown Documentation |  

## 👨‍💻 About the Developer

**Molla Adugna**  
*Healthcare & Business Data Analyst*

Specializing in leveraging business intelligence tools to solve complex operational problems in healthcare, agriculture, and commercial enterprises.

* **GitHub:** https://github.com/Molla-Adugna
* **LinkedIn:** https://www.linkedin.com/in/molla-adugna

---

## 🚀 Future Roadmap & Enhancements

* [ ] **Power BI Migration:** Build a cloud-synced, mobile-responsive version of the dashboard.
* [ ] **Automated Data Quality Checks:** Implement VBA/Power Query rules to catch data entry anomalies.
* [ ] **Predictive Forecasting:** Incorporate time-series forecasting for production yields and feed inventory planning.    
  

⭐ *If you find this project or framework helpful, feel free to give this repository a star!*
