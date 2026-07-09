# Bellabeat Smart Device Usage Analysis
### Unlocking Growth Opportunities for Women's Wellness Marketing

![Python](https://img.shields.io/badge/tools-Python%20%7C%20Pandas%20%7C%20Matplotlib-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

---

## 📌 Business Task

Bellabeat is a high-tech manufacturer of health-focused products for women. The company wants to understand how consumers use **non-Bellabeat smart devices** in order to identify growth opportunities and inform its own marketing strategy.

This project analyzes FitBit fitness tracker data to answer:
1. What are the usage trends in smart device data?
2. How can these trends apply to Bellabeat customers?
3. How can these trends help shape Bellabeat's marketing strategy?

---

## 📂 Data Source

- **Dataset:** [FitBit Fitness Tracker Data](https://www.kaggle.com/datasets/arashnic/fitbit) (Kaggle, public domain via Mobius)
- **Scope:** Daily activity records from 33 Fitbit users
- **Time period:** April 12, 2016 – May 12, 2016 (31 days)
- **License note:** Data has limitations — small sample size, self-selected users, and data from 2016, which are acknowledged as constraints on generalizability.

---

## 🛠️ Tools & Tech Stack

| Stage | Tools |
|---|---|
| Data Cleaning & Processing | Python (Pandas) |
| Analysis | Pandas, Statistical correlation |
| Visualization | Matplotlib |
| Environment | Kaggle Notebooks |

---

## 🔍 Methodology

1. **Data Cleaning**
   - Checked for null values and duplicates (none found)
   - Validated date ranges and confirmed 31 unique logging days per user
   - Checked for invalid/negative values across numeric columns

2. **Feature Engineering**
   - Extracted `day_of_week` from `activity_date` for weekly pattern analysis
   - Created an `activity_level` segmentation (Sedentary / Active / Very Active) based on average daily steps per user

3. **Exploratory Data Analysis**
   - Descriptive statistics (`df.describe()`) across all activity metrics
   - Correlation analysis between steps and calories burned
   - Weekly trend analysis for steps, logging consistency, and active vs. sedentary minutes

---

## 📊 Key Insights

- **The 10,000-Steps Gap:** Average daily steps across users is ~7,637 — falling short of the widely recommended 10,000-step benchmark.
- **Steps Drive Calories:** A strong positive correlation exists between steps taken and calories burned (**Pearson's r = 0.59**), confirming that movement is a key driver of energy expenditure.
- **Weekly Activity Pattern:** Users are most active on **Saturdays (8,153 steps)** and **Tuesdays (8,125 steps)**, and least active on **Sundays (6,933 steps)**.
- **Logging Consistency:** Logging completion rate peaks on **Fridays (95.5%)** and dips on **Thursdays (89.1%)**, suggesting engagement fatigue mid-week.
- **A Sedentary Lifestyle:** Users spend an average of **~991 minutes/day (81.3%)** sedentary, compared to just 1.7% in very active minutes and 1.1% in fairly active minutes — highlighting a major behavioral gap.

---

## 💡 Business Recommendations

1. **Incentivize the 10K Goal (Smart Notifications):** Send encouraging push notifications mid-day when a user is falling behind on their step goal, paired with calorie-burn framing to boost motivation.

2. **Target Inactive Days:** Since activity consistently dips on Sundays, design targeted marketing campaigns and in-app challenges specifically to re-engage users on their least active day.

3. **Sedentary Alerts for Office Workers:** Given that over 80% of tracked time is sedentary, position Bellabeat's **Leaf** and **Time** trackers as stylish wellness companions that gently vibrate to remind women to stand and move after prolonged periods of inactivity.

---

## 📁 Repository Structure

```
bellabeat-marketing-data-analysis/
│
├── datasets/          # Raw FitBit dataset files
├── notebooks/         # Full analysis notebook (Kaggle/Jupyter)
└── README.md          # Project overview (this file)
```
---

## 👩‍💻 Author

**Safaa Mahmoud**
