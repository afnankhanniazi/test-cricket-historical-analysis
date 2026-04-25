# 121 Years of Test Cricket History: BI & Exploratory Data Analysis

## Project Overview
[cite_start]This repository contains a comprehensive Business Intelligence (BI) project analyzing over a century of Test Cricket match data from 1898 to 2020[cite: 133]. [cite_start]Utilizing Microsoft Power BI, raw historical data was transformed into an interactive dashboard to visualize team dominance, scoring evolution, and geographical spread[cite: 138]. [cite_start]The analysis uncovers deep statistical trends, including the "Home Advantage" phenomenon and the historical dominance of key nations[cite: 139].

## Data Source
* [cite_start]**Source:** Kaggle[cite: 7].
* [cite_start]**Volume:** Over 2,000 records representing individual team innings[cite: 8, 152].
* [cite_start]**Key Features:** Teams, Scores, Wickets, Results, and Host Country[cite: 9].

## Methodology: ETL & Data Modeling
[cite_start]The data underwent rigorous preprocessing within Power BI's Power Query Editor[cite: 155]:
* [cite_start]**Data Type Standardization:** Columns like Score and Wickets were converted from text to Whole Numbers for mathematical aggregation[cite: 156].
* [cite_start]**Date Parsing:** The StartDate column was parsed to extract the Year, enabling time-series trend lines[cite: 157].
* [cite_start]**Duplicate Handling:** Applied a "Count (Distinct)" function to the MatchKey column to fix inflated match counts caused by multiple innings[cite: 158, 159].
* [cite_start]**Metric Creation:** Built custom measures for "Total Score," "Total Wickets," and "Average Score"[cite: 160].

## Dashboard Architecture

### 1. Executive Overview
[cite_start]A high-level command center providing visibility into historical global trends[cite: 163].
* [cite_start]**KPIs:** Over 2 million runs scored and 71,000 wickets taken in history[cite: 11, 221].
* [cite_start]**Geographical Map:** Shows Test cricket is heavily concentrated in Commonwealth nations[cite: 12, 165].
* [cite_start]**Trend Line:** Reveals a massive spike in scoring starting from the 1970s, correlating with the commercialization of the sport[cite: 14, 166].

*(Note: Add screenshot of Page 1 here)*

### 2. Deep Dive Analysis
[cite_start]Engineered for exploratory analysis of performance nuances and head-to-head records[cite: 169].
* [cite_start]**Rivalry Matrix:** A heatmap grid cross-referencing every Batting Team against their Opposition to reveal runs scored in every matchup[cite: 18]. 
* [cite_start]**Fortress Analysis:** A side-by-side comparison of Home vs. Away wins, proving the "Home Advantage" across teams[cite: 16, 171].
* [cite_start]**The Funnel:** Ranks the top distinct wicket-taking nations to honor the bowlers[cite: 17, 172].

*(Note: Add screenshot of Page 2 here)*

## Key Insights
* [cite_start]**The "Big Two":** England and Australia account for 40% of all historical runs and wickets[cite: 20, 356].
* [cite_start]**Home Dominance:** Teams are incredibly difficult to beat at home; for example, India's home wins are almost double their away wins[cite: 23].
* [cite_start]**The Pakistan Anomaly:** Pakistan is the unique exception, standing as the only nation with more "Away" wins than "Home" wins[cite: 22].
* [cite_start]**The Draw Rate:** 35% of all matches end without a winner[cite: 21].

## Analytical Limitations
* [cite_start]**Historical Bias:** The 1898 start date heavily skews total runs/wickets in favor of older teams compared to the number of matches played by newer nations[cite: 27, 372].
* [cite_start]**Missing Environmental Variables:** The dataset lacks information on rain and pitch conditions, which heavily influence match outcomes[cite: 375, 376, 379, 380].
* [cite_start]**Era Differences:** The analysis treats a 1900 match the same as a 2020 match, despite significant changes in rules and playing conditions over time[cite: 382, 383].
* [cite_start]**No Player Details:** The data tracks team totals rather than individual player statistics[cite: 377, 378].

## How to View
1. Clone this repository to your local machine.
2. Open the `Cricket_Dashboard_Project.pbix` file using Microsoft Power BI Desktop.
3. Utilize the slicer panels to interact with the visual data.
