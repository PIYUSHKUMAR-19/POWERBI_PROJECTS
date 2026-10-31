# 🏠 Airbnb Performance Dashboard (Power BI)

An end-to-end interactive Power BI analysis exploring Airbnb performance, host verification, listing growth lifecycles, and customer review behavior across key global cities.

---

## 📌 Executive Summary & Key Highlights

* **Total Listings Analyzed:** 279,712 listings across 10 global cities and 144 property types.
* **Host Reach:** 182,024 unique hosts generating 5.37M+ total reviews.
* **Top Market Contributor:** Paris accounts for **23%** of overall listings.
* **Geographic Concentration:** Paris, New York, Sydney, and Rome collectively account for nearly **60%** of total listings.
* **Host Trust & Verification:** Over **two-thirds ($>66.9\%$)** of Airbnb hosts are fully verified with profile pictures.

---

## 📊 Key Insights & Dashboard Breakdown

### 1. New Listing Growth Analysis (Lifecycle Model)
* **2015 Peak Point:** Airbnb reached its highest rate of new listing growth.
* **2016–2017 Restraint & Profitability:** Tightening local regulations led to lower growth rates; however, Airbnb achieved profitability in H2 2016, marking 2017 as its first full year of net income.
* **2018–2020 Impact:** Renewed growth in 2018–2019 was sharply interrupted by the COVID-19 pandemic in early 2020.

### 2. Market Share & Pricing Mechanics
* **Price vs. Verification:** The average price of verified listings is generally lower than non-verified listings, while average ratings for verified listings remain slightly higher.
* **Superhost Distribution:** Mexico City boasts the best ratio of Superhost vs. non-Superhost listings, whereas Sydney shows the lowest relative proportion.
* **Rating Champions:** Mexico City holds the highest average overall rating; Hong Kong scores lowest overall.

### 3. Review Frequency & Customer Loyalty
* **Single-Review Dominance:** Most customers submit a review **only once**.
* **Cumulative Frequency:** **98.8%** of customers submit **3 reviews or fewer**.
* **Seasonal Demand Shifts:**
  * **Paris & Rome:** Dominate review volume from **April to August** (European summer peak).
  * **New York:** Experiences notable review spikes in **November and December** (holiday season).

---

## 🛠️ Data Model & DAX Measures

Below are the core DAX measures created to support dynamic analysis across this dashboard:

### 1. Calculated Column: Reviews per Reviewer
```dax
Reviews per Reviewer = 
CALCULATE (
    COUNT ( Reviews[review_id] ),
    ALLEXCEPT ( Reviews, Reviews[reviewer_id] )
)
```

### 2. Cumulative Reviewers Count
```dax
Cumulative Reviewers = 
VAR CurrentReviews = 
    MAX ( Reviews[Reviews per Reviewer] )
RETURN
CALCULATE (
    DISTINCTCOUNT ( Reviews[reviewer_id] ),
    FILTER (
        ALL ( Reviews ),
        Reviews[Reviews per Reviewer] <= CurrentReviews
    )
)
```

### 3. Total Reviewers (Context-Unfiltered)
```dax
Total Reviewers = 
CALCULATE (
    DISTINCTCOUNT ( Reviews[reviewer_id] ),
    ALL ( Reviews )
)
```

### 4. Cumulative % Review Frequency
```dax
Cumulative % review frequency = 
DIVIDE ( [Cumulative Reviewers], [Total Reviewers] )
```

### 5. % of Total Reviewers (Distribution)
```dax
% of Total Reviewers = 
DIVIDE (
    [Reviewers],
    CALCULATE (
        [Reviewers],
        ALL ( Reviews[Reviews per Reviewer] )
    )
)
```

### 6. Verification Status Matrix
```dax
NotVerified_NoProfile = 
CALCULATE (
    [Hosts Total],
    Listings[host_identity_verified] = "f",
    Listings[host_has_profile_pic] = "f"
)

NotVerified_Profile = 
CALCULATE (
    [Hosts Total],
    Listings[host_identity_verified] = "f",
    Listings[host_has_profile_pic] = "t"
)
```

### 7. City Level Review Share
```dax
% of Monthly Reviews = 
DIVIDE (
    [Total Reviews],
    CALCULATE (
        [Total Reviews],
        ALLSELECTED ( Listings[city] )
    )
)
```

---

## 💻 Tech Stack & Tools

* **Business Intelligence:** Power BI Desktop
* **Data Modeling:** DAX (Data Analysis Expressions)
* **Data Transformation:** Power Query ETL

---

## 🚀 How to Run locally

1. Clone this repository:
   ```bash
   git clone https://github.com/PIYUSHKUMAR-19/AIRBNB.git
   ```
2. Open `AIRBNB.pbix` in **Power BI Desktop**.
3. Ensure the underlying dataset paths are updated if prompted by Power Query.
