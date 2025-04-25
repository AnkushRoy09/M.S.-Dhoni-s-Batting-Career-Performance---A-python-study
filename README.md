[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/RN_okVXh)

# Project Title: "Analyzing M.S. Dhoni's Batting Career Performance: A Python Data Analysis Project"

This project analyzes cricket performance data across different formats (IPL, ODI, T20, Test) to generate insights and visualizations. The analysis is implemented in a Jupyter Notebook and includes data preprocessing, visualization, and clustering to distinguish between aggressive and defensive innings. In this project, we focus on a comprehensive analysis of M.S. Dhoni’s batting career performance using Python-based data analysis techniques.

---

## Project Overview

- **Objective:**  
    To analyze the performance data of a prominent cricket player—M.S. Dhoni—across multiple match formats (ODI, Test, T20, and IPL) and generate various plots, statistical insights, and regression analyses. The project explores key metrics such as total runs, strike rates, career averages, and performance trends over time.

- **Key Analyses:**  
    - Average performance against major teams  
    - Match performance trends over years  
    - Best batting positions and impact on strike rate  
    - Boundary percentage and career average progression  
    - Clustering of innings (aggressive vs. defensive)  
    - Regression analysis on factors influencing strike rate  
    - Comparison of performance across different formats

---

## Directory Structure

Below is an overview of the main components of the project:

| Directory/File                                        | Description                                                    |
|-------------------------------------------------------|----------------------------------------------------------------|
| `final-project-AnkushRoy09/`                           | Root folder containing the project.                            |
| ├── `EPP_Final_Project.ipynb`                          | Main Jupyter Notebook with all analysis and visualizations.    |
| ├── `README.md`                                      | This file, which provides an overview, analysis details, and setup instructions. |
| ├── `data/`                                          | Contains all data files.                                       |
| │   ├── `raw_data/`                                  | CSV files with raw cricket data.                               |
| │   └── `filtered_data/`                             | Processed CSV files used in the analysis.                      |
| ├── `build/`                                         | Folder containing generated plots and visualizations.          |
| │   ├── `Average_against_Major_Teams/`               | Plots for average performance against major teams.             |
| │   ├── `Average_Performance_Plots/`                 | Visualizations of average match performance.                   |
| │   ├── `Best_Batting_Position/`                     | Analysis of the best batting positions.                        |
| │   ├── `Boundary_Percentage_Plots/`                 | Boundary percentage visualizations.                            |
| │   ├── `Career_Average_Progression/`                | Career progression of batting average over time.               |
| │   ├── `Clustering_Aggressive_vs_Defensive_Innings/`  | Clustering plots for innings analysis.                         |
| │   ├── `Matches_played_against_different_oppositions/` | Visualizations of matches played vs. different teams.        |
| │   ├── `Matches_played_by_Year/`                    | Year-wise breakdown of matches played.                         |
| │   ├── `Runs_scored_against_different_oppositions/` | Visualizations of runs scored vs. opposition.                  |
| │   ├── `Runs_scored_by_year/`                       | Year-wise analysis of runs scored.                              |
| │   └── `Strike_Rate_Moving_Average/`                | Trend analysis of strike rates over time.                        |
| └── `.git/`                                         | Git version control files.                                     |

---

## Setup Instructions

Follow these steps to set up the project on your local machine:

1. **Clone the Repository:**

     ```bash
     git clone https://github.com/yourusername/final-project-AnkushRoy09.git
     cd final-project-AnkushRoy09
     ```

2. **Install Dependencies:**

     It is recommended to use a virtual environment. For example, using venv:

     ```bash
     python -m venv venv
     source venv/bin/activate  # On Windows, use: venv\Scripts\activate
     pip install -r requirements.txt
     ```

     Note: If a requirements.txt file is not provided, ensure you have the following Python packages installed:

     - pandas
     - matplotlib
     - numpy
     - jupyter or jupyterlab

3. **Data Files:**

     The `data/` directory contains both raw and processed CSV files. Ensure these files are in place before running the analysis. If you need to update the dataset, place your CSV files into the appropriate folder.

4. **Running the Project**

     - **Launch the Notebook:**

         Start the Jupyter Notebook environment:

         ```bash
         jupyter notebook
         ```

     - **Open the Notebook:**

         In the browser interface, open the `EPP_Final_Project.ipynb` notebook.

     - **Execute the Notebook:**

         Run all cells to execute the analysis and generate visualizations. The notebook includes:

         - Data loading and preprocessing
         - Statistical analysis and visualization generation
         - Regression and clustering analyses
         - Detailed interpretations of various performance metrics

---

## Project Components

### Data Analysis

- Processes data from multiple formats (ODI, Test, T20, IPL) to extract key performance metrics.
- Calculates career statistics such as total runs, balls faced, strike rates, averages, centuries, and fifties.
- Compares performance across different oppositions and match years.

### Visualization

- Generates multiple plots and graphs saved in the `build/` directory:
    - Average performance and batting averages against different teams.
    - Matches played and runs scored by year.
    - Career average progression and clustering of innings.
    - Regression plots showing the impact of balls faced and batting position on strike rate.

### Regression & Machine Learning Analysis

- **Impact of Balls Faced on Strike Rate:**
    - Regression analysis is performed across formats:
        - ODI: Negative correlation indicating a slight decrease in strike rate with additional balls faced.
        - Test: Positive correlation reflecting a steady increase in strike rate over longer innings.
        - T20: Significant negative correlation suggesting caution in aggressive T20 innings.
        - IPL: Positive correlation indicating acceleration in the fast-paced format.

- **Analysis of Batting Position:**
    - Examines how batting order affects strike rate:
        - In ODIs and Tests, lower batting positions correlate with reduced strike rates.
        - In T20s and IPL, lower positions often yield higher strike rates due to the need for quick scoring in the final overs.

### Reports and Insights

- Provides comprehensive insights into M.S. Dhoni’s batting career, including:
    - Performance trends over time and across formats.
    - Optimal batting positions for maximizing runs and strike rate.
    - Detailed breakdowns of matches played and runs scored against different oppositions.

---

## Detailed Analysis & Observations

### Introduction

M.S. Dhoni, one of the most successful and celebrated cricketers in history, has left an indelible mark on the game with his exceptional batting skills, strategic acumen, and leadership. This project uses Python data analysis techniques to evaluate his career performance across ODIs, Test Matches, T20 Internationals, and IPL. The analysis not only quantifies his contributions with key statistics but also explores performance trends using regression and clustering methods.

### Overview & Key Observations

- **Consistency Across Formats:**
    Dhoni's ODI career shows remarkable consistency with high averages and strike rates, while his Test performances underline his adaptability in various conditions.

- **Performance Trends:**
    The project examines fluctuations over the years, highlighting phases where Dhoni either accelerated or steadied his innings.

- **Role Adaptation:**
    In T20s and the IPL, Dhoni’s aggressive finishing ability is underscored by high strike rates, especially in the death overs.

### Data Cleaning & Career Statistics Calculation

- **Data Cleaning:**
    Functions process raw data by converting date formats, extracting years, and cleaning batting scores. Unnecessary columns are dropped, and missing values are handled to prepare datasets for analysis.

- **Career Statistics:**
    The analysis computes:
    - First and last match dates
    - Total matches, innings, runs, balls faced, and averages
    - Number of not outs, centuries, and fifties
    - Boundary counts (fours and sixes)

### Data Visualization & Results Analysis

- **Visualizations:**
    Bar charts and line plots illustrate:
    - Matches and runs scored by year
    - Average performance against different oppositions
    - Career average progression over time

- **Results Analysis:**
    Tables summarize:
    - Matches played and runs scored against various teams
    - Batting averages, best/worst averages per opposition
    - Year-wise performance highlights

### Regression Analysis (Using Linear Regression and Random Forest Regression)

- **Impact of Balls Faced on Strike Rate:**
    Regression coefficients reveal format-specific trends:
    - ODI: Slight negative impact
    - Test: Positive trend
    - T20: Strong negative impact
    - IPL: Positive impact

- **Batting Position & Strike Rate:**
    Analysis shows:
    - In ODIs and Tests, lower batting positions reduce strike rate.
    - In T20s and IPL, batting lower can boost strike rate, reflecting aggressive finishing roles.

### Conclusion

Through an in-depth statistical examination of M.S. Dhoni’s batting career, this project highlights key performance metrics, trends, and correlations across formats. The findings reinforce Dhoni’s reputation as a dynamic player—adept at both stabilizing and accelerating innings depending on match context. The use of Python for data analysis and visualization in this project underscores the power of data-driven insights in sports analytics.

---

## Citations

- ESPN Cricinfo. (n.d.). M.S. Dhoni Career Statistics. Retrieved from ESPN Cricinfo
- MS Dhoni Performance Data. Retrieved from CricMetric
- Python Data Science Handbook. (2017). O'Reilly Media.
- Seaborn and Matplotlib Documentation. (n.d.). Retrieved from Matplotlib & Seaborn

---
