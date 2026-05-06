# 📊 Mobile App User Interaction Analysis

## 🔍 Project Overview

This project analyzes user interaction data from a mobile application to understand user behavior and engagement patterns.

---

## 🎯 Objectives

* Clean and preprocess raw dataset
* Perform exploratory data analysis (EDA)
* Test impact of subscription and push notifications

---

## 🗂️ Dataset

Dataset includes:

* User ID, Session ID
* Device OS
* Event Type
* Session Duration
* Subscription Status
* Push Notification Status

---

# 🧹 Data Cleaning & Preparation

## 🔹 Initial Data Inspection

### Dataset Preview (Before Cleaning)

![Dataset Preview](https://github.com/payaldadhwal/Mobile_AppUser_Interaction_Analysis/blob/main/images/head().png
)

👉 Shows raw, uncleaned dataset structure

---

### Data Information

![Data Info](https://github.com/payaldadhwal/Mobile_AppUser_Interaction_Analysis/blob/main/images/df.info.png
)

👉 Displays column types and non-null counts

---

## 🔹 Handling Missing Values

### Missing Values Check (After Cleaning)

![Missing Values](https://github.com/payaldadhwal/Mobile_AppUser_Interaction_Analysis/blob/main/images/df_isnull.png
)

👉 Confirms dataset has no null values after preprocessing

---

## 🔹 Data Cleaning Steps

* Removed unnecessary column (`Unnamed: 9`)
* Handled missing values
* Standardized categorical columns
* Converted data types

---

# 📊 Exploratory Data Analysis (EDA)

## 🔹 Session Duration Distribution

### Histogram

![Histogram](https://github.com/payaldadhwal/Mobile_AppUser_Interaction_Analysis/blob/main/images/hist.session.png
)

👉 Shows distribution of session duration across users

---

### Boxplot

![Boxplot](https://github.com/payaldadhwal/Mobile_AppUser_Interaction_Analysis/blob/main/images/boxplot.png
)

👉 Highlights spread and presence of outliers (power users)

---

## 🔹 Key Insights from EDA

* Average session duration ≈ 30 minutes
* High variability in user engagement
* Presence of power users

---

# 📈 Hypothesis Testing

## 🔹 Test 1: Subscription vs Session Duration

![Subscription Test](https://github.com/payaldadhwal/Mobile_AppUser_Interaction_Analysis/blob/main/images/ttest_sub.png
)

👉 Result: No statistically significant impact

---

## 🔹 Test 2: Push Notifications vs Session Duration

![Push Test](https://github.com/payaldadhwal/Mobile_AppUser_Interaction_Analysis/blob/main/images/pushenabled.png)

👉 Result: No statistically significant impact

---

# 📌 Key Findings

* Click, Scroll, Share are dominant interactions
* Android users form majority
* Session duration is not affected by:

  * Subscription
  * Push notifications

---

# 🧠 Conclusion

User engagement is driven more by:

* Content quality
* Personalization
* User experience

---

# 📁 Project Structure

```
Mobile_AppUser_Interaction_Analysis/
│
├── images/
│   ├── head().png
│   ├── df.info.png
│   ├── df_isnull.png
│   ├── hist.session.png
│   ├── boxplot.png
│   ├── ttest_sub.png
│   ├── pushenabled.png

│
└── README.md

├── data/
│   └── mobile_app_interactions_csv.csv
│
├── notebook/
│   └── mobileuser_interaction.ipynb
│
├── report/
│   └── project_report.pdf

---

## 🙋‍♀️ Author

Payal Dadhwal
