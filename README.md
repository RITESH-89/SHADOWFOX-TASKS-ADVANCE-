# SHADOWFOX-TASKS-ADVANCED-
An advanced cricket fielding performance analysis tool built with Python (Jupyter Notebook). This project calculates player fielding performance scores using metrics like clean picks, good throws, catches, dropped catches, and runs saved. Visualizations highlight top performers, providing actionable insights for sports analytics.
# Cricket Fielding Analysis 🏏

## 📌 Project Overview
This project is an **advanced cricket fielding performance analysis tool** designed to evaluate player contributions during a T20 match. Using a dataset of fielding events (e.g., clean picks, catches, throws, dropped catches), it calculates a **Performance Score (PS)** for each player to assess their defensive impact on the game.

This project was developed as part of an **Advanced Task** during the **ShadowFox Internship**.

---

## ✨ Key Features
- **Comprehensive Fielding Metrics:** Automatically calculates clean picks, good throws, catches, dropped catches, and runs saved.
- **Performance Score (PS):** A weighted scoring system based on the effectiveness of fielding actions.
- **Data Cleaning:** Automatically removes fake or numeric player names (e.g., `1`, `0`, `2`) for accuracy.
- **Visualizations:** Generates bar plots for **all players' performance** and **Top 5 performers** using Matplotlib & Seaborn.
- **Export:** Saves a performance matrix to Excel for further analysis.
- **Beginner-Friendly Notebook:** A Jupyter Notebook with step-by-step analysis and comments.

---

## 🗂 Dataset Details
The dataset includes the following columns:

| Column Name       | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| **Match No.**     | Identifier for the match.                                                   |
| **Innings**       | Indicates which innings the data is recorded for.                          |
| **Team**          | Fielding team name.                                                         |
| **Player Name**   | Name of the fielder involved in the event.                                  |
| **Position**      | Fielding position of the player at the time of the ball.                    |
| **Pick**          | Fielding event (e.g., clean pick, good throw, catch, drop catch).           |
| **Throw**         | Throw outcome (e.g., run out, missed run out, stumping, missed stumping).   |
| **Runs**          | Runs saved (+) or conceded (-) due to fielding action.                      |
| **Overcount**     | Over number in which the fielding event occurred.                           |
| **Venue**         | Location of the match.                                                      |

---

## 🧮 Performance Score Formula
\[
PS = (CP \times WCP) + (GT \times WGT) + (C \times WC) + (DC \times WDC) + RS
\]

Where:  
- **CP** = Clean Picks  
- **GT** = Good Throws  
- **C** = Catches  
- **DC** = Dropped Catches  
- **RS** = Runs Saved (positive or negative)  

**Weights:**  
- `WCP = 2`  
- `WGT = 3`  
- `WC = 5`  
- `WDC = -3`  

---

## ⚙️ Tech Stack
- **Language:** Python 3  
- **Libraries:** Pandas, Matplotlib, Seaborn, OpenPyXL  
- **Environment:** Jupyter Notebook (via Anaconda)  

---

## 📊 Visualizations
1. **Fielding Performance Score (All Players):** Horizontal bar chart showing PS of all players.  
2. **Top 5 Performers:** Highlighting the top 5 players with the highest PS.  
<img width="995" height="280" alt="Screenshot 2025-07-26 101812" src="https://github.com/user-attachments/assets/fa2a79df-f27c-4569-8fea-a4c94a9a83e9" />
<img width="752" height="646" alt="Screenshot 2025-07-26 102044" src="https://github.com/user-attachments/assets/396d701c-a36b-426f-b5b8-8beb582a9579" />
<img width="989" height="498" alt="Screenshot 2025-07-26 102034" src="https://github.com/user-attachments/assets/06d0f371-908d-40b1-9959-027020175a1b" />
<img width="617" height="261" alt="Screenshot 2025-07-26 102027" src="https://github.com/user-attachments/assets/15ab2ce0-839d-4511-ac54-f75a05464d20" />
<img width="896" height="174" alt="Screenshot 2025-07-26 101827" src="https://github.com/user-attachments/assets/e4d9795d-b26d-430b-a05a-29abed178312" />
<img width="957" height="171" alt="Screenshot 2025-07-26 101820" src="https://github.com/user-attachments/assets/e7560b67-2082-45ae-a920-bf7ba1764b34" />

---

## 📁 Project Structure
cricket-fielding-analysis/
│
├── data/
│ └── IPL sample data.xlsx
│
├── analysis/
│ └── performance_matrix.xlsx
│
├── fielding_analysis.ipynb
└── README.md

---
##🔑 Outputs
Performance Matrix: Table of fielding metrics and performance scores for each player.

Graphs:

Bar chart of all players' performance scores.

Bar chart of Top 5 fielders.

Excel Export: analysis/performance_matrix.xlsx.

---

##📌 Future Enhancements
Add interactive dashboards using Plotly or Streamlit.

Include additional metrics like direct hits and missed run-outs.

Generate automated PDF reports for matches.

---

##👨‍💻 Author
Ritesh Paithankar

Role: ShadowFox Internship Trainee – Advanced Task (Sports Analytics)

Skills Used: Python, Data Analysis, Visualization, Sports Analytics

---
