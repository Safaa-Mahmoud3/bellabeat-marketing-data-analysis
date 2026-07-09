# Bellabeat Smart Device Data Analysis


**Prepared by:** Safaa Mahmoud

---

## 1. Business Scenario
Bellabeat is a high-tech manufacturer of health-focused products for women. The goal of this project is to analyze smart device fitness data from non-Bellabeat users (FitBit) to identify consumer usage trends and provide high-level, data-driven marketing strategies for Bellabeat's executive team to unlock new growth opportunities.

---

## 2. Data Source Description
To understand consumer habits, this analysis utilizes public-domain smart device datasets. A quick overview of the dataset structure is summarized below:

| Attribute | Value |
| :--- | :--- |
| **Data Source** | Kaggle FitBit Fitness Tracker Data (via Mobius) |
| **Sample Size** | 33 Unique Users  |
| **Tracking Period** | March 2016 – May 2016 |
| **Licensing** | CC0: Public Domain |
| **Core Files Used** | `dailyActivity_merged.csv` |

### 2.1 Dataset Context & Content
* **Comprehensive Tracking:** The dataset contains personal fitness tracking data from eligible Fitbit users who consented to share minute-level output. This includes physical activity, heart rate, and sleep monitoring.

---

## 3. Technologies Used
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib
* **Environment:** Jupyter Notebook / Kaggle Notebook

---

## 4. Crucial Insight: The Friday Paradox (Adherence vs. Activity)
A fascinating contrast was discovered when comparing **User Adherence (Logging Rate)** and **Actual Activity (Average Steps)**:

* **Friday Behavior:** Friday recorded the **highest logging completion rate (95.5%)**, meaning users almost never take off their smart devices on this day. However, it showed one of the **lowest average step counts (7,448 steps)**. 
* **The Takeaway:** This indicates that on Fridays, users are highly committed to wearing their trackers, but their lifestyle becomes significantly more **sedentary** (low movement/rest days).
* **Tuesday/Saturday Behavior:** Conversely, days like Tuesday and Saturday show a slightly lower adherence frequency but experience huge spikes in physical movement, beating the 8,000 steps mark.

---
## 5. Marketing & Product Recommendations

* **Contextual Friday Push Notifications (The Friday Paradox):** Since data shows women wear their Bellabeat devices faithfully on Fridays (95.5% adherence) but move the least, the Bellabeat App should trigger tailored, friendly notifications on Friday afternoons. Instead of an aggressive "Go run" alert, send a wellness-focused reminder like: *"We notice you're enjoying a relaxing Friday! How about a quick 10-minute evening walk to hit your step goal while keeping your streak alive?"*
* **Incentivize the 10k Goal:** The Bellabeat app can send encouraging, smart push notifications around mid-day if a user is far from reaching the 10,000 steps threshold, reminding them of the personal health and calorie-burning benefits.
* **Target Inactive Days (Sunday Challenges):** Since data shows activity drops significantly on Sundays, marketing campaigns and app notifications can introduce "Sunday Fun-Walk" challenges or community badges to motivate users on typically lazy days.
* **Sedentary Alerts for Office Workers:** Because users spend a massive portion of their day being sedentary, Bellabeat can heavily market its **Leaf** or **Time** trackers as fashionable wellness assistants. The app can feature a custom setting that gently vibrates to remind women to stand up and stretch after 1 hour of continuous sitting.
