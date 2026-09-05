# 🏏 IPL Matches Data Analysis

## 📌 Project Overview

This project is an exploratory data analysis of **950 IPL matches played from 2008 to 2022**.

The dataset contains match-level information such as teams, venues, cities, toss decisions, winners, winning margins, Player of the Match, umpires, and player lists.

The project focuses on cleaning the dataset, understanding its structure, analyzing match patterns, and extracting useful insights through Python visualizations.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Understand the structure and quality of IPL match data.
- Clean and prepare the dataset for analysis.
- Analyze IPL seasons and match distribution.
- Identify cities and venues where matches were played most frequently.
- Analyze toss decisions and their patterns.
- Study Super Over occurrences.
- Analyze how teams won matches — by runs, wickets, or Super Over.
- Explore venue-wise match outcomes.
- Analyze winning teams across seasons.
- Explore the relationship between toss winners and match winners.
- Identify the most frequent Player of the Match by season.
- Explore umpire information.

---

## 🛠️ Technologies Used

- **Python**
- **Pandas** – Data cleaning and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Jupyter Notebook** – Analysis environment

---

## 📂 Project Files

| File | Description |
|---|---|
| `ipl-matches.ipynb` | Jupyter Notebook containing data cleaning, exploratory analysis, visualizations, and conclusions |
| `ipl-matches.csv` | Original IPL matches dataset used for the analysis |
| `New_iplData.csv` | Cleaned dataset exported from the notebook |
| `README.md` | Project documentation |

---

## 📊 Dataset Summary

The dataset contains **950 IPL match records** covering the seasons **2008–2022**.

The dataset includes information about:

- Match ID
- City
- Date
- Season
- Match Number
- Team 1 and Team 2
- Venue
- Toss Winner
- Toss Decision
- Super Over
- Winning Team
- Winning Method
- Winning Margin
- Player of the Match
- Umpires
- Team player lists

---

## 🧹 Data Cleaning

The notebook performs several data-cleaning and transformation steps.

### Missing Values

The project checks missing values and handles important missing fields:

- Missing `WinningTeam` values are filled with `together`.
- Missing `Player_of_Match` values are filled with `Not Anyone`.
- Missing `SuperOver` values are filled with `No`.
- Missing `Margin` values are filled with `0`.
- Missing city values are filled using the corresponding venue for Sharjah and Dubai matches.

### Data Transformation

The notebook also:

- Removes the unused `method` column.
- Cleans venue names by keeping the main venue name before the comma.
- Standardizes `SuperOver` values from `Y/N` to `Yes/No`.
- Converts categorical columns to the `category` data type.
- Converts `Date` into a proper datetime format.
- Standardizes historical team names:
  - Delhi Daredevils → Delhi Capitals
  - Kings XI Punjab → Punjab Kings
  - Rising Pune Supergiant → Rising Pune Supergiants
- Recreates the `Season` value from the match date.

---

## 🔍 Exploratory Data Analysis

### 1. Season Analysis

The project analyzes the number of matches played in each IPL season.

There are **950 matches across 15 seasons**, from 2008 to 2022.

The highest number of matches in the dataset occurred in **2013 with 76 matches**.

### 2. City Analysis

The analysis identifies cities with the highest number of IPL matches.

**Mumbai** has the highest number of matches in the dataset, with **159 matches**.

Other frequently used cities include Kolkata, Delhi, Chennai, Bangalore, and Hyderabad.

### 3. Toss Decision Analysis

The project analyzes whether teams chose to **bat** or **field** after winning the toss.

- Field: **599 matches**
- Bat: **351 matches**

Therefore, choosing to field was more common in this dataset.

### 4. Super Over Analysis

The project studies the occurrence of Super Overs.

- No Super Over: **936 matches**
- Super Over: **14 matches**

This shows that Super Overs were relatively rare compared with normal match results.

### 5. Winning Method Analysis

The dataset is analyzed according to how matches were won:

- Wickets: **509 matches**
- Runs: **423 matches**
- Super Over: **14 matches**
- No Result: **4 matches**

Winning by wickets is the most frequent result type in this dataset.

### 6. Venue Analysis

The project uses cross-tabulation and heatmaps to analyze:

- Venue vs winning method
- Venue vs season
- Venue vs winning team

This helps understand match distribution and winning patterns across different venues.

### 7. Toss Winner vs Match Winner

The project compares the team that won the toss with the team that eventually won the match.

A pie chart is used to visualize the relationship between toss results and match results.

### 8. Season-wise Winning Teams

The project analyzes winning teams across different IPL seasons using counts and cross-tabulation.

### 9. Player of the Match Analysis

The notebook identifies the most frequent Player of the Match for each season and visualizes the result using a heatmap.

### 10. Umpire Analysis

The project explores umpire information from `Umpire1` and `Umpire2`.

The notebook also identifies the most frequently appearing first umpire in the dataset.

---

## 📈 Visualizations

The project uses several visualization techniques, including:

- Bar charts
- Histograms
- Box plots
- Pie charts
- Heatmaps
- Cross-tabulation visualizations

These visualizations are used to make IPL match patterns easier to understand.

---

## 💡 Key Insights

Based on the analysis performed in the notebook:

- The dataset contains **950 IPL matches from 2008 to 2022**.
- **2013** has the highest number of matches in the dataset with **76 matches**.
- **Mumbai** hosted the highest number of matches with **159 matches**.
- Teams chose to **field after winning the toss more often** than choosing to bat.
- Only **14 matches** went to a Super Over.
- Winning by **wickets** is the most common winning method.
- Venue, season, winning team, toss decision, and Player of the Match show useful patterns that can be explored further.

---

## 📌 Conclusion

This project demonstrates the complete process of performing exploratory data analysis on IPL match data using Python.

The workflow includes **dataset understanding, data-quality checking, data cleaning, data transformation, exploratory analysis, visualization, and insight generation**.

The analysis provides a useful overview of IPL match patterns across seasons, cities, venues, toss decisions, winning methods, teams, players, and umpires.

---

## 📊 Power BI Dashboard

An interactive Power BI dashboard was created to visualize Diwali sales performance.

### Dashboard Highlights
- Sales and order analysis
- Customer demographics
- State-wise sales performance
- Product category analysis
- Gender-wise sales insights
- Interactive filters and slicers

### Dashboard Preview

![Diwali Sales Dashboard](image.png)

### Power BI File

The complete Power BI dashboard is available here:

`Diwali Sales.pbix`


## 👨‍💻 Author

**Darshan Bagthariya**

MCA Student | Aspiring Data Analyst

### Skills Demonstrated

`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Data Cleaning` `EDA` `Data Visualization`
