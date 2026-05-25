# 🌿 Bellabeat Fitness Tracking App Analysis
### Google Data Analytics Professional Certificate — Capstone Project
 
![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-informational)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
 
---
 
## 📌 Overview
 
This repository contains my Capstone Project for the **Google Data Analytics Professional Certificate** on Coursera. The analysis follows the complete **6-step data analysis framework**: Ask → Prepare → Process → Analyze → Share → Act.
 
The goal is to analyze FitBit smart device usage data and extract actionable insights to guide **Bellabeat's** marketing strategy — a high-tech wellness company specializing in health-focused smart products for women.
 
---
 
## 🏢 About Bellabeat
 
Founded in 2013 by Urška Sršen and Sando Mur, Bellabeat designs elegantly crafted health-focused smart products that empower women with knowledge about their own health and habits. Their product lineup includes the **Bellabeat App**, **Leaf tracker**, **Time wellness watch**, and **Spring water bottle**.
 
---
## Step 1: Ask ❓
 
### Business Task
Analyze FitBit Fitness Tracker Data to extract actionable insights regarding consumer behavior, thereby informing Bellabeat's marketing strategy.
 
### Business Objectives
1. Identify prevailing trends within the FitBit user base
2. Assess the applicability of these trends to Bellabeat's customer demographic
3. Utilize identified trends to shape and optimize Bellabeat's marketing strategy
### Key Stakeholders
| Stakeholder | Role |
|-------------|------|
| Urška Sršen | Co-founder & Chief Creative Officer |
| Sando Mur | Co-founder & Executive Team |
| Marketing Analytics Team | Data analysts steering marketing strategy |
 
---
 
## Step 2: Prepare 📦
 
### Data Source
| Detail | Info |
|--------|------|
| **Source** | [FitBit Fitness Tracker Data — Kaggle](https://www.kaggle.com/arashnic/fitbit) |
| **License** | CC0: Public Domain |
| **Collection Method** | Amazon Mechanical Turk survey |
| **Period** | March 12, 2016 – May 12, 2016 |
| **Users** | 30 consented FitBit users |
| **Files Available** | 18 CSV files |
| **File Used** | `dailyActivity_merged.csv` |
 
### Data Limitations
1. Data from **2016** may not reflect current consumer behaviors
2. **Sample size of 30** users is not representative of the broader female population
3. Survey-sourced data — accuracy and integrity cannot be fully guaranteed
### ROCCC Assessment
| Criteria | Rating | Reason |
|----------|--------|--------|
| Reliable | 🔴 Low | Small sample of 30 respondents |
| Original | 🔴 Low | Sourced via third-party (Amazon Mechanical Turk) |
| Comprehensive | 🟡 Medium | Parameters moderately align with Bellabeat's products |
| Current | 🔴 Low | Dataset is nearly a decade old |
| Cited | 🔴 Low | Limited traceability from third-party platform |
 
 
## Step 3: Process 🔄
 
### Tools Used
- **Python** — core analysis language
- **Pandas** — data manipulation and cleaning
- **NumPy** — numerical operations
- **Matplotlib** — data visualization
- **Jupyter Notebook** — interactive development environment
### Data Cleaning Steps
- ✅ Checked for null/missing values → **none found**
- ✅ Dataset: **940 rows, 15 columns**
- ✅ Confirmed **33 unique user IDs**
- ✅ Converted `ActivityDate` from `object` → `datetime64`
- ✅ Created `day_of_the_week` column from date
- ✅ Created `total_mins` (sum of all activity minute columns)
- ✅ Created `total_hours` (total_mins ÷ 60)
- ✅ Renamed all columns to `snake_case` for consistency
- ✅ Reordered columns for cleaner structure
---
 
## Step 4: Analyze 🔍
 
Key statistics from `df_activity.describe()`:
 
| Metric | Value |
|--------|-------|
| Average daily steps | **7,637** (~5.4 km) |
| Recommended daily steps | 10,000 (~8 km) |
| Average calories burned | **2,303** |
| Median sedentary time | **~16.5 hours/day** (991 mins) |
| Average active time | **~3.5 hours/day** |
 
---
 
## Step 5: Share (Visualizations & Findings) 📊
 
### Chart 1 — App Usage Frequency Across the Week
> Histogram of FitBit login frequency by day of week
 
- Users are **most active on weekdays** (Tuesday–Thursday)
- Activity tracking drops noticeably on **weekends**
- Suggests users link fitness tracking to their work/weekday routine
---
 
### Chart 2 — Calories Burned vs. Steps Taken
> Scatter plot with median reference lines
 
- Clear **positive correlation** between steps and calories burned
- Median: **7,637 steps** and **2,303 calories**
- Users below median steps consistently burn fewer calories
---
 
### Chart 3 — Calories Burned vs. Hours Logged
> Scatter plot with median sedentary reference line
 
- **Weak positive correlation** between hours logged and calories burned
- High sedentary time does not significantly increase calorie burn
- Reinforces the need for active movement prompts in the app
---
 
### Chart 4 — Activity Breakdown by Minutes
> Pie chart of total activity type proportions
 
| Activity Type | Percentage |
|---------------|-----------|
| 😴 Sedentary | **81.3%** |
| 🚶 Lightly Active | 15.8% |
| 🏃 Fairly Active | 1.1% |
| 💪 Very Active | 1.7% |
 
- Over **81% of all tracked time is sedentary**
- Users are primarily logging passive daily movement, not intentional fitness
---
 
## Step 6: Act (Recommendations) 💡
 
### 1. 🔔 Smart Activity Notifications
Since 81.3% of usage is sedentary, Bellabeat should implement intelligent nudges in the app reminding users to hit step goals and move during long inactive periods. Weekend push notifications could help close the engagement gap seen on Saturdays and Sundays.
 
### 2. 📅 Weekday-Focused Marketing Campaigns
Users are most active tracking on weekdays. Bellabeat should time their digital campaigns (Google Search, Instagram, Facebook) around **Tuesday–Thursday** for maximum engagement and click-through rates.
 
### 3. 📈 Personalized Weekly Health Reports via Membership
Leverage the Bellabeat membership program to deliver personalized weekly summaries showing users their sedentary vs. active time split and nudging them toward improvement. This deepens app retention and differentiates Bellabeat from competitors.
 
---
 
## 📁 Repository Structure
 
```
bellabeat-data-analysis-capstone/
│
├── bellabeat_activity_analysis.ipynb   ← Full analysis notebook
├── README.md                           ← Project overview (this file)
└── datasets/
    └── dailyActivity_merged.csv        ← Source data from Kaggle
```
 
---
 
## 🎓 Certificate
 
Completed as part of the **[Google Data Analytics Professional Certificate](https://www.coursera.org/professional-certificates/google-data-analytics)** — Coursera
 
8-course program covering: data cleaning, SQL, Tableau, R programming, data visualization, and real-world case studies.
 
---
