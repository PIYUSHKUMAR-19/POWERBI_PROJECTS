# 🏦 BANK LOAN ANALYTICS DASHBOARD
### An Interactive Financial Analytics & Credit Risk Dashboard | Microsoft Power BI

<p align="center">
  <img src="https://img.shields.io/badge/POWER%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" />
  <img src="https://img.shields.io/badge/DAX-Analytics-512BD4?style=for-the-badge" />
  <img src="https://img.shields.io/badge/DOMAIN-Financial%20Analytics-168B75?style=for-the-badge" />
  <img src="https://img.shields.io/badge/PROJECT-Business%20Intelligence-2874A6?style=for-the-badge" />
</p>

---

## 📊 Dashboard Overview

The **Bank Loan Analytics Dashboard** is an interactive Business Intelligence project developed using Microsoft Power BI to analyze loan applications, financial performance, repayment behavior, and borrower characteristics.

The dashboard transforms loan-related data into meaningful financial insights through dynamic KPIs, interactive slicers, comparative visualizations, and geographical analysis.

It consists of two analytical views:

- **Summary:** Financial KPIs, loan quality, funding performance, repayment status, interest rates, and DTI analysis.
- **Overview:** Monthly application trends, loan term distribution, homeownership analysis, loan purposes, and geographical distribution.

## 🎯 Project Objectives

- Analyze overall loan application performance.
- Evaluate total funded and received amounts.
- Identify good loan and bad loan distributions.
- Examine repayment behavior across different loan statuses.
- Analyze average interest rates and debt-to-income ratios.
- Understand monthly loan application trends.
- Investigate loan distribution by grade and purpose.
- Explore borrower homeownership and geographical patterns.
- Build an interactive dashboard for data-driven financial analysis.

---

## 🖥️ Dashboard Preview

### 01 | Summary Dashboard

The Summary Dashboard provides a consolidated overview of the bank's loan portfolio, financial performance, and repayment quality.

#### Key Performance Indicators

| KPI | Overall Performance |
|:---|---:|
| 📄 Total Loan Applications | **39K** |
| 💰 Total Funded Amount | **₹435.8M** |
| 💵 Total Amount Received | **₹473.1M** |
| 📈 Average Interest Rate | **12.0%** |
| 📊 Average DTI Ratio | **13.3%** |

#### Good Loan vs. Bad Loan Analysis

The dashboard segments loan applications into good and bad loan categories to evaluate the overall quality of the loan portfolio.

| Performance Metric | Good Loans | Bad Loans |
|:---|---:|---:|
| Loan Applications | 33,243 | 5,333 |
| Funded Amount | ₹370.2M | ₹65.5M |
| Amount Received | ₹435.8M | ₹37.3M |
| Application Percentage | 86.18% | 13.82% |

#### 🔍 Key Observations

- **86.18% Good Loans:** The majority of loan applications fall under the good loan category.
- **13.82% Bad Loans:** A smaller but important portion of the portfolio is classified as bad loans.
- **Funding Distribution:** Good loans account for approximately ₹370.2M in funded amounts.
- **Recovery Performance:** The bad loan segment has a considerably lower received amount compared with its funded amount.
- **Portfolio Quality:** The distribution provides an overview of the overall lending performance and potential credit risk.

#### Loan Status Analysis

The dashboard examines loan applications across three major repayment statuses.

| Loan Status | Applications |
|:---|---:|
| Fully Paid | 32.1K |
| Charged Off | 5.3K |
| Current | 1.1K |

**Additional comparisons include:**

- Funded Amount vs. Received Amount by Loan Status.
- Loan Application Distribution by Status.
- Average Interest Rate by Loan Status.
- Average DTI Ratio by Loan Status.

These visualizations help evaluate repayment patterns and compare the financial characteristics of different loan segments.

---

### 02 | Overview Dashboard

The Overview Dashboard explores the distribution of loan applications across time, repayment periods, borrower housing arrangements, loan purposes, and geographical locations.

#### A. Monthly Loan Application Distribution

The line chart illustrates the monthly movement of loan applications.

**Analytical Focus:**
- Identify monthly changes in application volume.
- Observe periods of relatively higher application activity.
- Understand the overall application trend.
- Identify potential seasonal patterns in borrowing activity.

#### B. Loan Term Distribution

The dashboard compares loan applications based on repayment duration.

| Loan Term | Description |
|:---|:---|
| 36 Months | Shorter repayment duration |
| 60 Months | Longer repayment duration |

**Key Observation:** The 36-month loan category represents the larger share of applications in the displayed distribution.

#### C. Loan Applications by Homeownership

Borrowers are classified according to their homeownership status.

| Category | Description |
|:---|:---|
| Rent | Borrowers living in rented accommodation |
| Mortgage | Borrowers with mortgage arrangements |
| Own | Borrowers who own their homes |
| Other | Other housing arrangements |
| None | No specified homeownership category |

**Key Observation:** Rent and Mortgage represent the dominant categories in the displayed borrower distribution.

#### D. Loan Applications by Purpose

The treemap visualization highlights the distribution of loan applications across different borrowing purposes.

Major loan categories include:

| Loan Purpose | Analytical Perspective |
|:---|:---|
| Debt Consolidation | Managing existing debts |
| Credit Card | Credit-related financial requirements |
| Other | Miscellaneous borrowing needs |
| Home Improvement | Property improvement expenses |
| Small Business | Business-related financial requirements |
| Car | Vehicle financing |
| Major Purchase | Significant personal purchases |
| Wedding | Wedding-related expenses |
| Medical | Healthcare-related expenses |
| Moving | Relocation expenses |
| House | Housing-related requirements |
| Vacation | Travel-related expenses |
| Educational | Education-related expenses |
| Renewable Energy | Renewable energy-related expenses |

**Key Observation:** Debt Consolidation occupies the largest visible segment, followed by Credit Card and Other.

This indicates that debt management and credit-related requirements contribute substantially to the displayed loan application distribution.

#### E. Geographical Loan Distribution

The geographical visualization represents loan application distribution across different US states.

**Analytical Focus:**
- Identify geographical concentrations of loan applications.
- Compare lending activity across states.
- Explore regional variations in borrowing patterns.
- Identify locations contributing significantly to the loan portfolio.

---

## 🎛️ Interactive Slicers & Dynamic Analysis

One of the major features of this dashboard is its interactive filtering functionality.

Instead of restricting users to an overall portfolio view, the dashboard allows them to investigate specific loan segments using two major slicers.

### 01. Loan Purpose Filter

Users can filter the dashboard using the following loan categories:

`Car` · `Credit Card` · `Debt Consolidation` · `Educational` · `Home Improvement` · `House` · `Major Purchase` · `Medical` · `Moving` · `Other` · `Renewable Energy` · `Small Business` · `Vacation` · `Wedding`

**What can be analyzed?**

- Total applications for a selected loan purpose.
- Funded amount and received amount.
- Good loan and bad loan percentages.
- Average interest rate and DTI ratio.
- Repayment status distribution.
- Financial performance of individual loan categories.

**Example: Debt Consolidation**

Selecting Debt Consolidation filters the dashboard to investigate its contribution to the overall portfolio, including its application volume, funding performance, repayment behavior, and credit risk indicators.

### 02. Loan Grade Filter

The dashboard provides seven loan-grade categories:

<p align="center">
  <img src="https://img.shields.io/badge/Grade-A-2E8B57?style=flat-square" />
  <img src="https://img.shields.io/badge/Grade-B-4C9F70?style=flat-square" />
  <img src="https://img.shields.io/badge/Grade-C-73A942?style=flat-square" />
  <img src="https://img.shields.io/badge/Grade-D-C9A227?style=flat-square" />
  <img src="https://img.shields.io/badge/Grade-E-D88A32?style=flat-square" />
  <img src="https://img.shields.io/badge/Grade-F-D45B45?style=flat-square" />
  <img src="https://img.shields.io/badge/Grade-G-BB3E3E?style=flat-square" />
</p>

**What can be analyzed?**

- Application distribution across loan grades.
- Total funded and received amounts.
- Differences in average interest rates.
- Good loan and bad loan proportions.
- Repayment performance across different grades.
- Potential credit risk patterns.

**Example: Selecting Grade C**

The dashboard dynamically updates its KPIs and visualizations to show the financial and repayment characteristics of Grade C loans.

### 03. Combined Filter Analysis

The dashboard also supports combining loan purpose and loan grade filters.

**Example: Debt Consolidation + Grade C**

This combination allows users to investigate a specific loan segment through:

| Analytical Metric | Purpose |
|:---|:---|
| Loan Applications | Measure application volume |
| Funded Amount | Evaluate funding distribution |
| Amount Received | Examine repayment collections |
| Average Interest Rate | Understand borrowing costs |
| Average DTI Ratio | Evaluate borrower debt burden |
| Good Loan Percentage | Analyze loan quality |
| Bad Loan Percentage | Identify potential risk |
| Loan Status | Examine repayment distribution |

*Note: The values generated by these filters are dynamic. The overall KPI figures shown above represent the unfiltered dashboard snapshot.*

---

## 💡 Key Business Insights

The following insights are based on the overall dashboard figures and displayed visualizations.

| Analytical Area | Key Finding | Business Implication |
|:---|:---|:---|
| Loan Volume | Approximately 39K applications | Indicates the scale of lending activity |
| Good Loans | 86.18% of applications | Majority of the portfolio falls under the good loan category |
| Bad Loans | 13.82% of applications | Highlights the importance of credit risk monitoring |
| Funded Amount | ₹435.8M | Represents the total funding volume |
| Amount Received | ₹473.1M | Indicates the total amount collected |
| Loan Purpose | Debt Consolidation leads | Identifies a major borrowing requirement |
| Loan Term | 36-month loans dominate | Highlights the larger share of shorter-term applications |
| Homeownership | Rent and Mortgage dominate | Reveals the major housing categories among applicants |

### 🏢 Business Recommendations

**1. Credit Risk Monitoring**

Monitor the bad loan segment and investigate borrower characteristics associated with charged-off loans.

**2. Loan Recovery Optimization**

Evaluate differences between funded and received amounts to identify segments requiring stronger recovery strategies.

**3. Grade-Wise Performance Evaluation**

Compare loan grades A–G to understand differences in interest rates, repayment patterns, and loan quality.

**4. Customer-Centric Loan Products**

Use loan-purpose analysis to identify major borrowing requirements and develop suitable financial products.

**5. Monthly Trend Monitoring**

Analyze application trends to support lending capacity planning and resource allocation.

**6. Geographical Performance Analysis**

Explore state-wise application distribution to identify regional lending opportunities.

---

## 📐 Key Performance Indicators

The dashboard focuses on the following financial and operational KPIs:

| KPI Category | Metrics |
|:---|:---|
| Loan Volume | Total Loan Applications |
| Funding Performance | Total Funded Amount |
| Collection Performance | Total Amount Received |
| Borrowing Cost | Average Interest Rate |
| Borrower Financial Health | Average DTI Ratio |
| Loan Quality | Good Loan Percentage, Bad Loan Percentage |
| Repayment Performance | Fully Paid, Charged Off, Current |
| Comparative Analysis | Funded vs. Received Amount |

---

## 🛠️ Tools & Technologies

<p align="left">
  <img src="https://img.shields.io/badge/Microsoft-Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" />
  <img src="https://img.shields.io/badge/DAX-Data%20Analysis-512BD4?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Power%20Query-Data%20Transformation-168B75?style=for-the-badge" />
</p>

| Technology | Application |
|:---|:---|
| Microsoft Power BI | Interactive dashboard development |
| Power Query | Data transformation and preparation |
| DAX | KPI calculations and analytical measures |
| Data Modeling | Organizing data for analytical reporting |
| Slicers | Interactive filtering and segmentation |

---

## 🧠 Skills Demonstrated

- Business Intelligence
- Financial Data Analysis
- Data Visualization
- Interactive Dashboard Development
- DAX Measures and Calculations
- Power Query
- Data Modeling
- KPI Development
- Credit Risk Analysis
- Loan Portfolio Analysis
- Comparative and Trend Analysis
- Business Insight Generation

---

## 🚀 How to Explore the Dashboard

1. Download the Power BI `.pbix` file from this repository.
2. Install and open Microsoft Power BI Desktop.
3. Open `BANK_LOAN_ANALYTICS.pbix`.
4. Navigate between the Summary and Overview pages.
5. Select different loan purposes using the left-side slicer.
6. Explore loan grades A–G using the top slicer.
7. Combine filters to analyze specific loan segments.
8. Observe how the dashboard visualizations and KPIs respond dynamically.

---

## 👨‍💻 Author

**PIYUSH KUMAR**

 

 
