# Pole to Victory: 20 Years of F1 Competitiveness

**Author:** Alison Carvajal Paulino  
**Student ID:** 70095663  

---

## Overview

Formula 1 is widely recognized as one of the most data-intensive sports in the world. A common saying in motorsport claims that *"the race is won on Saturday"* during qualifying. 

The primary goal of this project is to analyze historical F1 race data to examine whether starting grid position dictates the final race outcome, or if modern regulations and race strategies allow for meaningful comebacks from further back on the grid.

To evaluate this hypothesis, the project compares the **2005** and **2025** Formula 1 seasons, assessing whether two decades of technological and regulatory innovations have reshaped race competitiveness.

---
## Regulatory Context: 2005 vs. 2025

Two decades of rule changes shifted Formula 1 from a Saturday-dominated sport to a Sunday strategy battle:

- **Tires & Strategy**: In 2005, tire changes were banned during the race, forcing drivers to use a single set. In 2025, mandatory pit stops with compound changes allow strategic pit overtaking.
- **Qualifying Format**: In 2005, drivers qualified on heavy race fuel in a single-lap session. In 2025, a low-fuel knockout system (Q1-Q2-Q3) measures pure single-lap pace.
- **Engine & Aerodynamics**: 2005 V10 engines generated heavy dirty air, making following other cars extremely difficult. 2025 V6 turbo-hybrids use ground-effect aerodynamics and DRS to reduce turbulence and enable passing.
- **Race Decisiveness**: In 2005, difficult overtaking meant Saturday qualifying largely determined the winner. In 2025, strategy and easier passing allow for Sunday comebacks from further back on the grid.


## Project Structure & Methodology

First, I observed how the URLs changed while navigating statsf1.com and created two lists with the years and races to work with. Inside the for loops, the code constructs the specific URLs to access qualifying and race information, calling a function named `grid_position`  that returns a list of driver names ordered by position. I then created a dictionary with the key information from each race to use for comparison later, and converted it into a DataFrame to work with the results comfortably. 

The output displays a table showing the year, location, poleman name, winner name, whether the winner was the poleman, and if not, the winner's starting grid position. After that, I calculated the win percentages based on starting positions —pole position (P1), 2nd or 3rd (P2–P3), and 4th or lower (P4+)— separately for 2005 and 2025. These results were visualized using two pie charts, and finally, a direct comparison was made between the two years based on those starting grid positions.

## How to Run
1. **Clone the repository:**
   ```bash
   git clone https://github.com/aalicarvajal/F1-data-analysis.git
   cd F1-data-analysis
   ```

2. **Install dependencies:**
   ```bash
   pip install pandas beautifulsoup4 requests matplotlib
   ```

3. **Execute the Jupyter Notebook:**
   ```bash
   jupyter notebook F1_Grid_Analysis.ipynb
   ```

---

## Summary of Results

The comparative analysis reveals how changes in qualifying formats, tire regulations, and aerodynamic design (DRS & ground effect) over a 20-year span have affected the correlation between Saturday grid position and Sunday victory.

---
