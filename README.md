# 🏏 IPL Analysis Dashboard (2008–2025) | Power BI

An interactive **Power BI dashboard** that analyzes Indian Premier League (IPL) data from **2008 to 2025**. The dashboard provides insights into team performance, player statistics, match results, toss decisions, batting and bowling performances, and season-wise trends using interactive visualizations and DAX-based analytics.

---

# 📖 Table of Contents

- [Project Overview](#-project-overview)
- [Purpose](#-purpose)
- [Tech Stack](#-tech-stack)
- [Data Source](#-data-source)
- [Features & Highlights](#-features--highlights)
- [Dashboard Preview](#-dashboard-preview)
- [Key Insights](#-key-insights)
- [Project Structure](#-project-structure)
- [How to Use](#-how-to-use)
- [Skills Demonstrated](#-skills-demonstrated)
- [Business Value](#-business-value)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

# 📌 Project Overview

The **IPL Analysis Dashboard** is an interactive Business Intelligence project developed using **Microsoft Power BI** to analyze IPL match and ball-by-ball data from **2008 to 2025**.

The dashboard transforms extensive IPL data into meaningful visual insights covering team performance, player statistics, match outcomes, toss decisions, batting performance, bowling performance, and season-wise trends.

Interactive slicers, KPIs, charts, and DAX measures allow users to explore IPL statistics across different seasons, teams, players, and match conditions.

---

# 🎯 Purpose

The primary objective of this project is to provide a comprehensive analytical view of the Indian Premier League and make complex cricket statistics easier to understand.

The dashboard helps users:

- Analyze IPL performance across seasons.
- Compare team performance over the years.
- Identify top-performing batsmen and bowlers.
- Analyze toss decisions and their impact on match results.
- Study batting and bowling trends.
- Analyze match outcomes and winning margins.
- Track season-wise team performance.
- Explore player-level statistics.
- Identify important trends and patterns in IPL matches.

---

# 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **Power BI Desktop** | Dashboard Development |
| **Power Query** | Data Cleaning & Transformation |
| **DAX** | Measures, KPIs & Calculations |
| **Microsoft Excel / CSV** | Data Storage & Processing |
| **Data Modeling** | Relationship Management |
| **Data Visualization** | Interactive Reports |

---

# 📂 Data Source

The **IPL Analysis Dashboard (2008–2025)** is built using multiple datasets containing match-level, ball-by-ball, player, team, and IPL century information.

### 📊 1. Ball-by-Ball Data

The ball-by-ball dataset contains detailed information about every delivery bowled during IPL matches.

Key fields include:

- `match_id`
- `season_id`
- `inning`
- `over_number`
- `batter`
- `non_striker`
- `bowler`
- `batter_runs`
- `extras`
- `total_runs`
- `bye_runs`
- `leg_bye_runs`
- `penalty_runs`
- `no_ball_runs`
- `is_wicket`
- `is_wide_ball`
- `is_no_ball`
- `is_leg_bye`
- `is_bye`
- `wicket_kind`
- `player_out`
- `team_batting`
- `team_bowling`
- `batsman_type`
- `bowler_type`

The dataset is also used to calculate metrics such as:

- Total Runs
- Total 4s
- Total 6s
- Total Century
- Total Half Century
- Total Matches
- Average Runs per Innings
- Average Runs per Match

---

### 🏏 2. IPL Centuries Data

The `ipl_centuries` dataset contains information about individual century performances in IPL matches.

Key fields include:

- `Balls`
- `City`
- `Date`
- `Innings`
- `No`
- `Opposition`
- `Player`
- `Result`
- `Score`
- `Season`
- `Strike Rate`
- `Team`
- `Venue`

This dataset is used for analyzing batting performances and century statistics.

---

### 🏆 3. IPL Matches Data

The `IPL_Matches` dataset contains match-level information covering IPL seasons from **2008 to 2025**.

Key fields include:

- `match_id`
- `match_date`
- `match_number`
- `match_type`
- `season`
- `IPL Season`
- `team1`
- `team2`
- `match_winner`
- `toss_winner`
- `toss_decision`
- `Toss Match Result`
- `result`
- `city`
- `venue`
- `event_name`
- `format`
- `stage`
- `team_type`
- `balls_per_over`
- `overs`
- `player_of_match`
- `Fours`
- `Six`
- `Six_count`
- `Fours_count`
- `OC Team`
- `PC Team`
- `PC wicket`
- `OC Run`
- `PC Image`
- `OC Image`
- `Winner Logo`
- `Season Winner`
- `Season RunnerUp`
- `Purple cap`
- `RunnerUp logo`
- `win_by_runs`
- `win_by_wickets`

This dataset is used for analyzing:

- Match results
- Toss analysis
- Team performance
- Season winners
- Season runners-up
- Winning margins
- Player of the Match
- Venue performance
- Batting and bowling statistics

---

### 👤 4. Players Data

The `players-data-updated` dataset contains player information.

Key fields include:

- `player_id`
- `player_full_name`
- `player_name`
- `bat_style`
- `bowl_style`
- `player_image`

This dataset is used to provide player-level information and support player performance analysis.

---

### 🏏 5. Teams Data

The `teams_data` dataset contains IPL team information.

Key fields include:

- `team_id`
- `team_name`
- `image_url`
- `team_count`

This dataset is used for team identification, team analysis, and displaying team information in the dashboard.

---

### 📌 Data Model

The datasets are integrated in Power BI to create relationships between:

```text
Ball-by-Ball Data
        │
        │ match_id
        ▼
   IPL Matches
        │
        ├── season
        ├── team
        ├── player
        └── match information
             │
       ┌─────┴─────┐
       ▼           ▼
    Players      Teams
```
> **Note:** The datasets are used for educational, analytical, and portfolio purposes.

---

# ✨ Features & Highlights

## 🏆 Overall IPL Analysis

- Total Matches
- Total Seasons
- Total Teams
- Total Runs
- Total Wickets
- Average Runs per Innings
- Season-wise Performance

---

## 📅 Season-wise Analysis

Users can select individual IPL seasons to analyze:

- Matches Played
- Team Performance
- Top Run Scorers
- Top Wicket Takers
- Total Runs
- Total Wickets
- Winning Teams

---

## 📊 Match Analysis

- Match Results
- Winning Margins
- Runs-based Wins
- Wickets-based Wins
- Tie Matches
- No Result Matches
- Venue-wise Performance

---

## 🎛️ Interactive Features

- Dynamic Season Slicers
- Team Filters
- Player Filters
- Venue Filters
- Interactive KPI Cards
- Cross Filtering
- Drill-down Analysis
- Dynamic Charts
- Season-wise Comparisons

---

# 📸 Dashboard Preview

## Dashboard Overview

<p align="center">
  <img src="IPL Dashboard- I.png" alt="IPL Analysis Dashboard - Page 1" width="100%">
</p>

<p align="center">
  <img src="IPL Dashboard- II.png" alt="IPL Analysis Dashboard - Page 2" width="100%">
</p>

---
---

---

# 📊 Key Insights

The dashboard can be used to identify several important IPL trends, including:

- Comparison of team performance across IPL seasons.
- Identification of consistently successful teams.
- Analysis of top-performing batsmen and bowlers.
- Relationship between toss decisions and match outcomes.
- Trends in batting and bowling performance.
- Comparison of teams based on win percentage.
- Analysis of match-winning margins.
- Identification of high-scoring seasons and matches.
- Season-wise analysis of player performances.

---

# 📁 Project Structure

```text
📦 IPL-Analysis-2008-2025
│
├── 📄 README.md
│
├── 📂 Raw dataset
│   ├── IPL_Matches.csv
│   └── ball_by_ball_data.csv
│   └── ipl_centuries.csv
│   └── players-data-updated.csv
│   └── teams_data.csv
│
├── 📂 Cleaned dataset
│   ├── IPL_Matches.csv
│   └── ball_by_ball_data.csv
│   └── ipl_centuries.csv
│   └── players-data-updated.csv
│   └── teams_data.csv
│
├── 📂 images
│   ├── ipl_dashboard.png
│   ├── team_analysis.png
│   ├── player_analysis.png
│   └── toss_analysis.png
│
├── 📄 Data_Preprocesssing.ipynb
├── 📄 Data_Visualization.ipynb
├── 📄 IPL_Dashboard.pbix

```

---

# 🚀 How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/Adiitya09/ipl-analysis-2008-2025.git
```

### 2. Open the Power BI File

Open:

```text
IPL Analysis.pbix
```

using **Power BI Desktop**.

### 3. Load the Dataset

If required, update the dataset source paths in Power Query.

### 4. Refresh the Dashboard

Click:

```text
Home → Refresh
```

to load the latest available data.

### 5. Explore the Dashboard

Use the available slicers and filters to analyze:

- Seasons
- Teams
- Players
- Venues
- Toss decisions
- Match results

---

# 🚀 Skills Demonstrated

- Data Cleaning
- Data Transformation
- Data Modeling
- Power Query
- DAX
- KPI Development
- Data Visualization
- Interactive Dashboard Design
- Sports Analytics
- Exploratory Data Analysis
- Business Intelligence
- Analytical Storytelling

---

# 📈 DAX & Analytical Techniques

The project demonstrates the use of DAX for creating dynamic analytical measures such as:

- Total Matches
- Total Runs
- Total Wickets
- Average Runs
- Win Percentage
- Batting Statistics
- Bowling Statistics
- Toss Decision Analysis
- Season-wise Metrics
- Player Rankings

The measures dynamically respond to selected seasons, teams, and other filters.

---

# ⭐ Business Value

Although IPL is a sports dataset, the project demonstrates important **Business Intelligence and Data Analytics concepts**.

The dashboard shows how large datasets can be transformed into interactive reports that help users:

- Monitor performance.
- Compare entities.
- Identify trends.
- Analyze historical patterns.
- Discover relationships between different variables.
- Make data-driven decisions.

These analytical techniques can also be applied to real-world business domains such as sales, marketing, finance, HR, and operations.

---

# 🔮 Future Improvements

Potential improvements include:

- 🤖 IPL Match Outcome Prediction
- 📈 Player Performance Prediction
- 🏆 Team Win Probability
- 🔮 Season Performance Forecasting
- 🗺️ Venue-based Performance Mapping
- 📊 Advanced Player Ranking System
- 🧠 Machine Learning-based Match Prediction
- 📱 Mobile-optimized Dashboard
- ⚡ Real-time IPL Data Integration

---



---

# 📬 Connect With Me

### 👨‍💻 Author

**Aditya Patil**

- GitHub:   https://github.com/Adiitya09
- LinkedIn: https://www.linkedin.com/in/2004-aditya-patil/

---

## ⭐ If you found this project useful, don't forget to give it a Star!
