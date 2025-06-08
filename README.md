
# NBA-Player-Data-Analysis

This project is an **NBA Player Data Analysis** implemented in Python using Jupyter Notebook. It analyzes a dataset of 458 NBA players, covering player distribution, position roles, age demographics, and salary trends. The project includes clean data, visual insights, and correlation metrics to understand the modern NBA roster composition and player value.

---

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Data Story](#data-story)  
3. [Visualizations](#visualizations)  
4. [Key Insights](#key-insights)  
5. [Repository Structure](#repository-structure)  
6. [How to Run](#how-to-run)  
7. [Requirements](#requirements)   

---

## Project Overview

The NBA Player Data Analysis project is designed to examine:

- **Team distributions** – number of players per team  
- **Positions** – role-wise player distribution (Guard, Forward, Center)  
- **Age demographics** – age group patterns and peak playing ages  
- **Salary analysis** – total salary by team, position, and age correlation  
- **Correlation metrics** – how age relates to player salary  

---

## Data Story

The dataset contains detailed information on 458 NBA players, including:

- Team representation across all 30 NBA franchises  
- Position roles and how modern basketball emphasizes guards  
- Age patterns highlighting the league’s preference for younger talent  
- Salary trends across positions and franchises  

---

## Visualizations

> 📷 All visualizations are stored in the `/images/` directory. Click images below to view.

- ![Player Distribution by Team]([Images/Player Distribution by Team.png](https://github.com/nikhillshanmukhan/NBA-Player-Analysis-Python/blob/5c5f3ef98d8fee41d7b229da1c9edd8d6f719787/Images/Player%20Distribution%20by%20Team.png))  
- ![Position Distribution](images/Player_Position_Distribution.png)  
- ![Age Distribution](images/Player_Age_Distribution.png)  
- ![Total Salary by Team](images/Total_Salary_by_Team.png)  
- ![Total Salary by Position](images/Total_Salary_by_Position.png)  
- ![Age vs Salary Correlation](images/Age_vs_Salary.png)  

---

## Key Insights

- Guards dominate the NBA, making up **43.2%** of players  
- Most players are between **22–28 years** old, with a peak at 25  
- **Small forwards** command the highest salaries due to star power and versatility  
- Salaries **peak around age 28–30** but some young stars earn big early  
- Salary structures show a strong shift toward **perimeter play** and **positional flexibility**

---

## Repository Structure

```
nba-player-analysis/
├── data/
│   ├── nba_players_raw.csv
│   └── nba_players_clean.csv
├── images/
│   ├── Age_vs_Salary.png
│   ├── Player_Age_Distribution.png
│   ├── Player_Distribution_by_Team.png
│   ├── Player_Position_Distribution.png
│   ├── Total_Salary_by_Position.png
│   └── Total_Salary_by_Team.png
├── NBA_Player_Analysis.ipynb
└── README.md
```

---

## How to Run

1. Clone the repository  
   ```bash
   git clone https://github.com/your-username/nba-player-analysis.git
   cd nba-player-analysis
   ```

2. Open the notebook:  
   `NBA_Player_Analysis.ipynb` using Jupyter Notebook

3. Run all cells to generate the analysis and visualizations

---

## Requirements

- Python 3.x  
- Jupyter Notebook  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  

You can install the required packages using:

```bash
pip install pandas numpy matplotlib seaborn
```

---

