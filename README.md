# 📊 Mobile App User Interaction Analysis

## 🔍 Project Overview

This project analyzes user interaction data from a mobile application to understand user behavior, session patterns, and engagement drivers.

The analysis includes **data cleaning, exploratory data analysis (EDA), and statistical hypothesis testing** to evaluate whether features like subscription status and push notifications impact user engagement.

---

## 🎯 Objectives

* Clean and preprocess raw dataset
* Perform exploratory data analysis (EDA)
* Identify user behavior patterns
* Test the impact of:

  * Subscription status
  * Push notifications
    on session duration

---

## 🗂️ Dataset

* **Name:** Mobile App Interactions Dataset
* **File:** `mobile_app_interactions_csv.csv`
* **Description:**
  Contains user session data including:

  * User ID
  * Session ID
  * Device OS
  * Event Type (click, scroll, swipe, etc.)
  * Session Duration
  * Subscription Status
  * Push Notification Preference
  * User Age

---

## 🛠️ Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy

---

## 🧹 Data Cleaning & Preprocessing

* Removed unnecessary column: `Unnamed: 9`
* Handled missing values:

  * Dropped critical null rows
  * Filled categorical values with `"Unknown"`
  * Imputed `user_age` with median
  * Filled boolean values with `False`
* Standardized categorical columns:

  * Cleaned `device_os` (android / ios / unknown)
  * Cleaned `event_type` (click, scroll, tap, etc.)
* Removed outliers:

  * Session duration ≥ 10,000 seconds

---

## 📊 Exploratory Data Analysis (EDA)

### 🔹 Session Duration Distribution

* Average session duration ≈ **30 minutes**
* High variability observed
* Presence of **power users** with very high engagement

### 🔹 Event Type Analysis

* Most common interactions:

  * Click
  * Scroll
  * Share
* Slightly higher engagement in:

  * Scroll
  * Zoom

---

### 🔹 Feature Impact Analysis

* Compared session duration across:

  * Subscription status
  * Push notification settings

👉 No major visible differences found

---

## 📈 Hypothesis Testing

### Test 1: Subscription vs Session Duration

* **p-value:** 0.485
* ❌ No statistically significant impact

---

### Test 2: Push Notifications vs Session Duration

* **p-value:** 0.934
* ❌ No statistically significant impact

---

## 📌 Key Insights

* User activity is dominated by **click, scroll, and share events**
* Majority users are on **Android devices**
* Average session duration is around **30 minutes**
* **Power users** contribute to high engagement outliers
* Subscription and push notifications do **not significantly influence session duration**

---

## 🧠 Conclusion

User engagement is not significantly affected by subscription plans or push notification settings.

### 🚀 Recommendations

To improve engagement:

* Enhance **content quality**
* Focus on **personalization**
* Improve overall **user experience (UX)**

---

## 📷 Project Screenshots


* Dataset preview (`df.head()`)
* Data info (`df.info()`)
* Histogram & Boxplot
* Event type bar chart
* Hypothesis testing results

---

## 📁 Project Structure

```
├── data/
│   └── mobile_app_interactions_csv.csv
├── notebook/
│   └── analysis.ipynb
├── images/
│   └── (plots & screenshots)
├── report/
│   └── project_report.pdf
└── README.md
```

---

## 🙋‍♀️ Author

**Payal Dadhwal**
Aspiring Data Analyst

---

## ⭐ If you found this project useful

Give it a ⭐ on GitHub!
