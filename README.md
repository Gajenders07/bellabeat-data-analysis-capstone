## 🛠️ Tools Used
 
- **Python** — core analysis language
- **Pandas** — data manipulation and cleaning
- **NumPy** — numerical operations
- **Matplotlib** — data visualization
- **Jupyter Notebook** — interactive development environment
---
 
## 🔄 Process Summary
 
### Step 3: Process (Data Cleaning)
- Checked for null/missing values → **none found**
- Converted `ActivityDate` from `object` to `datetime64` format
- Created new columns: `day_of_the_week`, `total_mins`, `total_hours`
- Renamed all columns to `snake_case` for consistency
- Reordered and restructured columns for cleaner analysis
### Step 4: Analyze
Key statistics from `df_activity.describe()`:
 
| Metric | Value |
|--------|-------|
| Average daily steps | 7,637 (~5.4 km) |
| Recommended daily steps | 10,000 (~8 km) |
| Average calories burned | 2,303 |
| Average sedentary time | ~16.5 hours/day |
| Average active time | ~3.5 hours/day |
 
---
 
## 📊 Visualizations & Key Findings
 
### 1. App Usage Frequency Across the Week
> **Histogram** — frequency of FitBit app logins by day of week
 
- Users are **most active on weekdays** (Tuesday–Thursday)
- Activity tracking drops noticeably on **weekends**
- Suggests users track fitness alongside work/weekday routines
---
 
### 2. Calories Burned vs. Steps Taken
> **Scatter Plot** — relationship between daily steps and calories burned
 
- Clear **positive correlation** between steps and calories burned
- Median: **7,637 steps** and **2,303 calories**
- Users below the median steps line tend to burn fewer calories — reinforcing the value of step-based goals
---
 
### 3. Calories Burned vs. Hours Logged
> **Scatter Plot** — relationship between hours logged and calories burned
 
- **Weak positive correlation** between hours logged and calories burned
- Median sedentary time: ~16.5 hours (991 mins ÷ 60)
- High sedentary time does not significantly increase calorie burn — highlighting the need for active movement reminders
---
 
### 4. Activity Breakdown (Minutes)
> **Pie Chart** — proportion of activity types across all users
 
| Activity Type | Percentage |
|---------------|-----------|
| Sedentary | **81.3%** |
| Lightly Active | 15.8% |
| Fairly Active | 1.1% |
| Very Active | 1.7% |
 
- Over **81% of tracked time is sedentary** — users are primarily logging passive daily movement, not intentional fitness activity
---
 
## 💡 Recommendations
 
**1. Push Notifications for Activity Goals**
Since 81.3% of usage is sedentary, Bellabeat should implement smart nudges in their app — reminding users to hit step goals and move during long inactive periods. Target notifications especially on **weekends**, when engagement drops.
 
**2. Weekday-Focused Marketing Campaigns**
Since users are most active tracking on weekdays, Bellabeat should time their digital ad campaigns (Google Search, Instagram, Facebook) around **Tuesday–Thursday** for maximum engagement and click-through rates.
 
**3. Holistic Health Content Strategy**
Leverage the Bellabeat membership program to deliver personalized weekly health reports — showing users their sedentary vs. active split and nudging them toward healthier habits. This deepens app stickiness and differentiates Bellabeat from competitors.
 
---
 
## 📁 Repository Structure
 
```
bellabeat-data-analysis-capstone/
│
├── bellabeat_activity_analysis.ipynb   # Full analysis notebook
├── README.md                           # Project overview (this file)
└── datasets/
    └── dailyActivity_merged.csv        # Source data from Kaggle
```
 
---
 
## 🎓 Certificate
 
This project was completed as part of the:
 
**[Google Data Analytics Professional Certificate](https://www.coursera.org/professional-certificates/google-data-analytics)** — Coursera
 
The 8-course program covers: data cleaning, SQL, Tableau, R programming, data visualization, and real-world case studies.
 

 
*If you found this project helpful, feel free to ⭐ star the repository!*
