# 📊 pj_9_mlb – Dodgers 2022 Attendance Analysis

## 🧾 Project Overview

This project explores attendance data for the 2022 Los Angeles Dodgers season. The primary goal is to identify key factors that influence game attendance and provide insights to help optimize fan turnout at future games.

## 📁 Dataset

**File:** `dodgers-2022 (1).csv`  
- **Rows:** 81  
- **Columns:** 12  
- **Attributes:**
  - `month`, `day`, `day_of_week`: Temporal information about the game
  - `attend`: Game attendance (target variable)
  - `opponent`: Opposing team
  - `temp`, `skies`, `day_night`: Weather and time conditions
  - `cap`, `shirt`, `fireworks`, `bobblehead`: Binary flags for promotional items

## 🔍 Exploratory Data Analysis (EDA)

- **Distribution of Attendance:** Shows variability, with some games reaching very high attendance.
- **Day of the Week:** Attendance is generally higher during weekends.
- **Promotions:** Promotional events (especially bobbleheads) significantly boost attendance.
- **Visualization Tools:** Matplotlib and Pandas used to generate histograms and bar charts.

## 📈 Key Insights

- **Weekends vs Weekdays:** Weekend games (Saturday/Sunday) are more attended.
- **Promotional Impact:** All four promotions increased attendance, with bobblehead giveaways having the largest impact.
- **Weather and Opponents:** Future steps include analyzing these variables more deeply.

## 🧠 Tools Used

- Python
  - `pandas` for data manipulation
  - `matplotlib` for visualization

## 📌 Future Recommendations

- Schedule more games with bobblehead promotions.
- Optimize game times for weekends.
- Further analyze the effects of weather, opponent team, and temperature.

## 📂 Project Files

- `dodgers-2022 (1).csv` – Raw dataset
- `Bobga-Herman Gwanvoma hw 3.2 DSC630.pdf` – Report with analysis and insights

## 👨‍💻 Author

Bobga-Herman Gwanvoma  
MS Data Science | 2025  
