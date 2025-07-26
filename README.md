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
<img width="627" height="387" alt="Screenshot 2025-07-26 105656" src="https://github.com/user-attachments/assets/d66b6c9e-2744-4381-8a13-cf0f97a77508" />
<img width="786" height="465" alt="Screenshot 2025-07-26 105648" src="https://github.com/user-attachments/assets/ae32caae-ecb9-4c9e-99e4-d80a984a746c" />
<img width="776" height="251" alt="Screenshot 2025-07-26 105638" src="https://github.com/user-attachments/assets/8db3ab65-2550-46b8-b441-36823e3c15e0" />
<img width="437" height="65" alt="Screenshot 2025-07-26 105632" src="https://github.com/user-attachments/assets/6d7d7e14-b876-4be5-967e-accceca5a929" />
<img width="808" height="166" alt="Screenshot 2025-07-26 105623" src="https://github.com/user-attachments/assets/2273725b-68e9-46de-8360-fae1333bde1f" />
<img width="875" height="292" alt="Screenshot 2025-07-26 105614" src="https://github.com/user-attachments/assets/b4725caa-dfde-44d3-921f-fc2e3d16c63b" />
<img width="871" height="259" alt="Screenshot 2025-07-26 105603" src="https://github.com/user-attachments/assets/6643a0e2-5a9e-4ee5-a3e4-8864bb1819b2" />


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

LINKEDIN : "www.linkedin.com/in/ritesh-paithankar-4b43a828a"
---
