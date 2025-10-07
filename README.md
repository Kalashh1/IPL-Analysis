# **🏏 IPL 2025 Exploratory Data Analysis (EDA)**

## **Overview**

This project explores IPL 2025 player performance data to uncover batting & bowling trends, identify top performers, and extract fantasy cricket insights. The IPL has evolved into a fast-paced, high-strike-rate game where batsmen dominate with aggressive intent, while bowlers fight back with skill and precision.

### **Dataset**

* **Batting Dataset:**  
  * **File:** IPL2025Batters.csv  
  * **Rows:** 156 players  
  * **Columns:** 14 features (Runs, Matches, SR, AVG, 100s, 50s, 4s, 6s, etc.)  
* **Bowling Dataset:**  
  * **File:** IPL2025Bowlers.csv  
  * Covers bowling statistics from IPL 2025\.

## **Analysis Steps**

### **1\. Setup and Data Loading**

* **Libraries Imported:** pandas, numpy, matplotlib.pyplot, and seaborn were imported for data manipulation, numerical operations, and visualization.  
* **Data Loading:** The IPL2025Batters.csv and IPL2025Bowlers.csv files were loaded into pandas DataFrames.

### **2\. Data Cleaning and Preprocessing**

* **Visualization Styling:** Default styles for plots were set using seaborn.set() and plt.rcParams to ensure consistency and readability.  
* **Data Type Correction:**  
  * The HS (Highest Score) column in the batting dataset was cleaned by removing the '\*' character and converting it to an integer type.  
  * The AVG (Average) column was converted to a numeric type, with non-numeric values coerced into NaN.  
* **Index Reset:** The index for the bowlers' DataFrame was set to start from 1 for better readability.

### **3\. Batting Analysis**

A comprehensive analysis of the batting data was conducted to identify standout performances:

* **Highest Individual Score:** Identified the player with the most runs in a single match.  
* **Top Century Makers:** Extracted a list of players who scored 100 or more runs.  
* **Most Balls Faced:** Determined the top 10 players who faced the highest number of balls.  
* **Top Run Scorers:** Identified the top 10 players with the most runs in the tournament.  
* **Most Fifties:** Found the players who scored the most half-centuries.  
* **Most Sixes:** Analyzed which players and teams hit the most sixes.

### **4\. Bowling Analysis**

The bowling data was analyzed to find the top-performing bowlers:

* **Top Wicket Takers:** Identified the leading wicket-takers in the tournament.  
* **Most Economical Bowlers:** Found bowlers with the best economy rates (for those who have bowled more than 30 overs).  
* **Four and Five Wicket Hauls:** Identified players who have taken 4 or 5 wickets in a single match.

### **5\. Fantasy Cricket Insights**

* **Impact Score:** An Impact\_Score was calculated for batters using a weighted combination of runs, strike rate, 50s, and 100s to identify valuable players for fantasy leagues.  
* **Winning Team Analysis:** A case study on the winning team (RCB) was performed to analyze the run and wicket contributions of their key players.

### **6\. Visualizations**

Several visualizations were created to represent the findings:

* A bar plot of the **Top 10 Run Scorers**.  
* A histogram showing the **Distribution of Batting Average**.  
* A bar plot of the players with the **Most 50s**.  
* A scatter plot comparing **Runs vs. Strike Rate by Team**.  
* A scatter plot of **Highest Score vs. Total Runs by Team**.  
* A bar plot of the top **Impact Scores**.  
* A bar plot of the players with the **Most Sixes**.  
* A bar plot of the **Total Sixes Hit by Each Team**.  
* A pie chart showing the **Runs Distribution for the Winning Team (RCB)**.  
* A bar plot of the **Top 10 Wicket Takers**.  
* A bar plot comparing **Average vs. Economy Rate** for the most economical bowlers.  
* A scatter plot of **Wickets vs. Economy Rate by Team**.  
* A pie chart illustrating the **Wickets Distribution for the Winning Team (RCB)**.

Each visualization was saved as a PNG image for easy reference and reporting.