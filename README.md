# Project 1: SAT & ACT Analysis

## Problem Statement

### Of US States that underperform on the ACT, which are trending positively and why?
* Which states need the most help?
* Which of these states are on a positive path forward?
* What explains this positive trend? Are there policy ideas that could be exported to states in similar positions?

> Three datasets were examined for the purposes of answering these questions, ACT test results and participation rates 2017, ACT test results and participation rates 2018, and ACT test results and participation rates 2019. Each dataset contained an entry for each US State and Washington D.C. describing ACT averages across that state. After the data was loaded, cleaned, and properly reformmatted, an aggregate dataframe was created. Two grand average series were created, three year mean of ACT composite scores and the three year mean of ACT participation rates. Below you will find an executive summary of the analysis steps in the final_code.ipynb file and a data dictionary detailing more thoroughly the features in question.

## Executive Summary

### Contents of [final_code.ipynb](final_code.ipynb):
- 2017 Data Import & Cleaning
- 2018 Data Import and Cleaning
- Exploratory Data Analysis
- Data Visualization
- 2019 Data Import & Cleaning
- Dataset Aggregation
- Underperforming States, Trending Positively
- Choropleth Plots
- Conclusions and Recommendations

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

## Methods

> To better understand underperforming states that trending positively. I separated states that require students take the ACT from states that do not. States that require students take the ACT perform significantly worse on average, likely due to the much larger set of students taking the test. Thus to avoid an apples and oranges comparison, these states were excluded from analysis. Next a median split was performed to separate the remaining 31 states into high and low performing. 'Positively trending' was defining as improving composite ACT score for 3 consecutive years. Choropleth plots were used to visualize these relationships. Choropleth [shapefiles](usa_shapefiles) are from https://www.arcgis.com/home/item.html?id=f7f805eb65eb4ab787a0a3e1116ca7e5)

## Conclusions and Recommendations

> Of the low performing group, only one state met that criteria to be considered positively trending, Florida. This may be in part due to legislation passed in 2017, but is more likely due to the fact that Florida's ACT participation rate decreased over the same time period. The inverse relationship between participation rate and score was seen across tests and years.

#### Key Takeaways:
* Participations rates strongly influence ACT scores
* Few states are trending positively.
* Florida is the only underperforming state which does not require the ACT and has 3 consecutive years of ACT score improvement

#### Future Directions:
* Consider variables other than standardized test scores
    * Are test scores the best reflection of a positive learning experience? Perhaps looks at graduation rates, which have been shown to have a stronger relationship with positive life outcomes.

* Determine if the relationship between participation rates and test scores is statistically significant. Determine if the relationship between participation rate trends and test score trends is statisically significant.
* Expand analysis to more years of test data.

### Slide Deck
- [Click Here](Standardized_Testing_Trends.pptx)
