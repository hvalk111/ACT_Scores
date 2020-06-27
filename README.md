# Project 1: SAT & ACT Analysis

## Problem Statement

### Of US States that underperform on the ACT, which are trending positively and why?
* Which states need the most help?
* Which of these states are on a positive path forward?
* What explains this positive trend? Are there policy ideas that could be exported to states in similar positions?

## Executive Summary

### Contents of final_code.ipynb:
- [2017 Data Import & Cleaning](#Data-Import-and-Cleaning)
- [2018 Data Import and Cleaning](#2018-Data-Import-and-Cleaning)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Data Visualization](#Visualize-the-data)
- [2019 Data Import & Cleaning](#2019-Data-Import-and-Cleaning)
- [Dataset Aggregation](#Dataset-Aggregation)
- [Underperforming States, Trending Positively](#Underperforming-States-Trending-Positively)
- [Choropleth Plots](#Choropleth-Plots)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

|Feature|Type|Datasets|Description|
|---|---|---|---|
|state|object|SAT 2017, SAT 2018, ACT 2017, ACT 2018|50 US states plus Washington D.C.| 
|participation_sat|float|SAT 2017, SAT 2018|percentage of eligible students who took the sat| 
|evidence_based_reading_and_writing_sat|int|SAT 2017, SAT 2018|mean score in range 200-800| 
|math_sat|int|SAT 2017, SAT 2018|mean score in range 200-800|
|total_sat|int|SAT 2017, SAT 2018|mean score in range 400-1600| 
|participation_act|float|ACT 2017, ACT 2018|percentage of eligible students who took the sat| 
|english_act|float|ACT 2017|mean score in range 0-36| 
|math_act|float|ACT 2017|mean score in range 0-36| 
|reading_act|float|ACT 2017|mean score in range 0-36| 
|science_act|float|ACT 2017|mean score in range 0-36| 
|composite_act|float|ACT 2017, ACT 2018|mean composite score of all 4 sections in range 0-36| 
|composite_mean|float|Aggregate of ACT 2017, ACT 2018, ACT 2019|mean composite score of 17, 18, 19 mean composite scores in range 0-36| 
|participation_mean|float|Aggregate of ACT 2017, ACT 2018, ACT 2019|mean participation rate of 17, 18, 19 participation rates|

## Conclusions and Recommendations

* Participations rates strongly influence ACT scores
* Few states are trending positively.
* Florida is the only underperforming state which does not require the ACT and has 3 consecutive years of ACT score improvement
<br />
<br />
* Consider variables other than standardized test scores
    * Are test scores the best reflection of a positive learning experience? Perhaps looks at graduation rates instead

* Determine if the relationship between participation rates and test scores is statistically significant

### Slide Deck
[Click Here](#../slides/Standardized_Testing_Trends.pptx)