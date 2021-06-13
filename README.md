# kickstarter_analysis
Visualizing the success rate similar kickstarter campaigns are based on when they were greated and starting goal amount.

## Overview of Project

### Purpose
   The purpose of this project was to see which month had the most successful number of Kickstarter campaigns and the success percentage based on the desired goal to be raised. From this information one could estimate whether a Kickstarter for a similar project would be successful or not. One could aslo determine an optimal time of year to begin raising money and what a reasonable goal of money raised would be.
  
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
   By using pivot tables I could use the data sets for date created and outcome to create a graph that showed the number of specific outcomes by month. I filtered by category of Campaign project while counting number of outcomes per month.
  ![Theater_Outcomes_vs_Launch](https://github.com/Nifmoo/kickstarter_analysis/blob/main/Theater_Outcomes_VS_Launch.png)
  The challenge I encountered when using the pivot table was the Date Created values split into diiferent parts when selected for the pivot table. So i had to determine which part had the data i needed, the months, then filter accordingly.
  
### Analysis of Outcomes Based on Goals
   In order to determine success rate based on goal amount, I created a few arbitrary ranges that it could be included in and used a COUNTIFS() function to determine how many campaigns fell within the range and the outcome. I totaled the projects and then determine the percentage of successful and failed campaigns.
  ![Outcomes_vs_Goals](https://github.com/Nifmoo/kickstarter_analysis/blob/main/Outcomes_vs_Goals.png)
 
### Challenges and Difficulties Encountered
    The challenge I encountered when using the pivot table was the Date Created values split into diiferent parts when selected for the pivot table. So i had to determine which part had the data i needed, the months, then filter accordingly.
  
   The challenge I encountered creating this graph was actually creating the formulas using the COUNTIFS() function. It was a minor encounter, but at first I was not recieving the proper number of total projects. When i realized my mistake i realized I was not including the boundaries of the ranges. I changed the inside of my formulas to <= and >=, instead of < and > to fix my mistake.
  
## Results
  The best time to launch a theatrical Kickstarter campaign is the beginning of the summer, May and July. On contrast the worst time to start a campaign is in December.
  The campaigns raising the smaller amounts of money had a greater chance to be sucessful. The graph trended downward until a goal amount of $35000 where there was a relatively high success rate.
  The limitations of this data are how successful the project was once it got the necessary funds to help its completion. Also th amount one individual contributed to a fund is unknown. Other graphs that would be interesting to look at would be the average amount of time it took a successful campaign to reach its goal based on the amount needed to raise, or the amount of successful food truck kickstarter campaigns.
