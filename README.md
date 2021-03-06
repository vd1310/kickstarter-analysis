# kickstarter-analysis
Performing analysis on Kickstarter data to uncover trends
# Kickstarting with Excel
## Overview of Project
Louise’s wants to know how different campaigns fared in relation to their launch dates and their funding goals. We need to visualize campaign outcomes based on their launch dates and their funding goals.
### Purpose
The purpose of this challenge to analyse how different campaigns performed with respect to their launch dates and funding goals. By using the excel skills (formulas, charts & pivot tables) learned over the class sessions, we have to present campaign outcomes-based launch dates and goals. Pivot tables and charts helps in turning data in the excel sheet into meaningful information with visualization and that’s is what this exercise intends to perform.
## Analysis and Challenges
Objective of this analysis is to find out the performance of the funding campaign based on the launch date and the goal amounts. 
In order to perform this analysis, we have to massage the data slightly meaning that we have to either insert new columns and pivot tables. Once we gather the required fields and tables for analysis, we will insert the charts to visualize the data and make inference.
### Analysis of Outcomes Based on Launch Date
Objective is to find out successful and failed campaigns based on launch date across categories. To find the campaign outcome by launch date we have to perform the following tasks:
a. We need a year column to apply filters based on years. This column is not present and thus we will use the 'Date created column' to get this data with the help of year function.
note1: please refer to the 'data' tab/column U in the 'kick-starter' challenge sheet
note2: we also need to convert the raw date created and ended column to meaningful dates by applying formula as used in column S and T in Data tab
b. The category and subcategory column is split further to get sub category to filter campaigns based on television, plays etc.
note: please refer to the 'data' tab/column R in the 'kick-starter' challenge sheet
c. Now we have create a pivot table to get failed, successful or cancelled campaign bases on parent category and years. The table has to display results across the month and also provide an option to have filter for parent category and years. Group the "Row Labels" column to show the months of the year
refer to 'theater outcomes by launch date' tab in Kickstarter sheet. 
d. Applied filter on parent category to get results specifically for 'Theater' category
refer to 'theater outcomes by launch date' tab in Kickstarter sheet. Cell B2
e. Row labels sorted in descending order to see
refer to 'theater outcomes by launch date' tab in Kickstarter sheet
f. The line chart shows the number of successful, failed or cancelled projects by month.
refer to 'Theater_outcome_vs_launchdate.png'
### Analysis of Outcomes Based on Goals
Objective is to find out successful and failed campaigns based on funding goal.
To perform this analysis, we have to first create the required fields and populate data.
a. Created following columns:
Goal
Number Successful
Number Failed
Number Canceled
Total Projects
Percentage Successful
Percentage Failed
Percentage Cancelled
note: refer to 'Theater Outcomes by Goals' sheet
b. Used Countifs formula to populate "Number Successful," "Number Failed," and "Number Canceled" columns. The countifs had multiple filter based on the project "outcome," the "goal" amount using the goal ranges and the Subcategory "plays" 
c. To populate "Total Projects" column, add columns 'number of successful', 'number failed' and 'number cancelled'
note: refer to 'Theater Outcomes by Goals' sheet
d. Calculated percentages of successful, failed, and canceled projects are calculated based on the data from the "Total Projects," "Number Successful," "Number Failed," and "Number Canceled" columns. 
note: refer to 'Theater Outcomes by Goals' sheet
e. To understand the successful, cancelled or failed campaign, inserted a line chart across goal ranges.
refer to Theater_outcome_vs_goal.png 
### Challenges and Difficulties Encountered
It was challenging to use the countifs formula with multiple conditions across multiple functions.
TA office hours helped in understanding the formula for one row and then it was easy to apply the logic for all the ranges.
## Results
- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. Successful campaign peaked during May and were lowest during Dec period
So the campaign launched in the middle of the year were more successful versus the ones launched during the beginning or the ending periods
2. failed campaigns showed a fairly consistent trend across the months
- What can you conclude about the Outcomes based on Goals?
Plays based campaign based on funding goals showed inverse relationship across the ranges. Successful plays based campaign showed increasing trend up until 30000 mark, where they dipped but then started rising as soon the funding goal was greater than 50000. This trend was reverse for percentage failed campaigns. No play-based campaign was cancelled
- What are some limitations of this dataset?
The analysis is limited to launch date or funding amount, there could be other factor for the success / failure of the campaign. Eg country specific constraints etc.
- What are some other possible tables and/or graphs that we could create?
We could have created more charts find out the success of campaign based on amount pledged, countries
