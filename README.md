
# NBA-Player-Data-Analysis

This project is an **NBA Player Data Analysis** implemented in Python using Jupyter Notebook. It analyzes a dataset of 458 NBA players, covering player distribution, position roles, age demographics, and salary trends. The project includes clean data, visual insights, and correlation metrics to understand the modern NBA roster composition and player value.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Preprocessing Steps](#Preprocessing-steps)  
3. [Data Story](#data-story)  
4. [Visualizations](#visualizations)  
5. [Key Insights](#key-insights)  
6. [Repository Structure](#repository-structure)  
7. [How to Run](#how-to-run)  
8. [Requirements](#requirements)   

---

## Project Overview

The NBA Player Data Analysis project is designed to examine:

- **Team distributions** – number of players per team  
- **Positions** – role-wise player distribution (Guard, Forward, Center)  
- **Age demographics** – age group patterns and peak playing ages  
- **Salary analysis** – total salary by team, position, and age correlation  
- **Correlation metrics** – how age relates to player salary  

---
## 🔧 Preprocessing Steps

#### 📏 Fixed Height Column
Replaced inconsistent entries with random heights ranging from **150 cm to 180 cm** using the following code:

```python
df['Height'] = np.random.randint(150, 181, size=len(df))
```

#### 💰 Handled Missing Salaries
Filled missing salary values with `0` or used an appropriate imputation strategy based on data context.

#### 🧹 Cleaned Position Data
Standardized player positions for uniformity (e.g., used `"PG"` instead of `"Point Guard"`).

## Data Story

The dataset contains detailed information on 458 NBA players, including:

- Team representation across all 30 NBA franchises  
- Position roles and how modern basketball emphasizes guards  
- Age patterns highlighting the league’s preference for younger talent  
- Salary trends across positions and franchises  

---

## 📊 Analysis Tasks with Visualizations

---

### 1. Player Distribution Across Teams

#### 📝 Findings:
- The dataset contains players from **30 NBA teams**
- The **Boston Celtics** have the most players in the dataset (**15 players**, 3.28%)
- Several teams have **15 players**, which appears to be the standard roster size
- Distribution is relatively even across teams with minor variations

#### 📉 Visualization:
> ![Bar chart showing team distribution with percentages](images/Player_Distribution_by_Team.png)

---

### 2. Player Position Segregation

#### 📝 Findings:
- **Guards (PG/SG)** make up the largest portion (**43.2%**)
- **Forwards (SF/PF)** account for **38.6%**
- **Centers (C)** comprise **18.2%** of the dataset
- **Point Guard (PG)** is the most common position (**22.5%**)
- **Center (C)** is the least common (**18.2%**)

#### 📊 Visualization:
> ![Pie chart showing position distribution](images/Player_Position_Distribution.png)

---

### 3. Predominant Age Group

#### 📝 Findings:
- Majority of players (**62%**) are between **22–28 years** old
- **Peak age** is **25 years** (**12.4%** of players)
- Only **8%** of players are **30 or older**
- **Youngest player**: *Devin Booker (19)*
- **Oldest players**: *Tim Duncan & Andre Miller (40)*

#### 📈 Visualization:
> ![Histogram of age distribution](images/Player_Age_Distribution.png)

---

### 4. Team/Position with Highest Salary Expenditure

#### 📝 Findings:
- **Los Angeles Clippers** have the **highest total salary** ($128,543,069)
- **Small Forwards (SF)** have the highest total salary across positions
- **Shooting Guard (SG)** includes high-paid stars like *James Harden*
- Notable high salaries:
  - *Kobe Bryant* – $25M
  - *LeBron James* – $22.9M
  - *Dwight Howard* – $22.3M

#### 📊 Visualization:
> ![Stacked bar chart showing salary by team and position](images/Total_Salary_by_Team.png)  
> ![Salary by position](images/Total_Salary_by_Position.png)

---

### 5. Age-Salary Correlation

#### 📝 Findings:
- Moderate **Weak positive correlation (r=0.21)** between **age** and **salary**
- Salaries **peak at age 28–30**, then decline
- Significant **outliers** among younger players with high salaries (e.g., *young stars*)
- **Veterans (35+)** usually earn less unless they're **superstars**

#### 📈 Visualization:
> ![Scatter plot showing age vs salary](images/Age_vs_Salary.png)

---


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
   git clone https://github.com/nikhillshanmukhan/nba-player-analysis.git
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

