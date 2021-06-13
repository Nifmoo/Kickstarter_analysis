# kickstarter_analysis
Visualizing the success rate similar kickstarter campaigns are based on when they were greated and starting goal amount.

## Overview of Project

### Purpose
  The purpose of this project was to see which month had the most successful number of Kickstarter campaigns and the success percentage based on the desired goal to be raised. From this information one could estimate whether a Kickstarter for a similar project would be successful or not. One could aslo determine an optimal time of year to begin raising money and what a reasonable goal of money raised would be.
  
## Analysis and Challenges

  By using pivot tables I could use the data sets for date created and outcome to create a graph that showed the number of specific outcomes by month. I filtered by category of Campaign project while counting number of outcomes per month.
  ![Theater_Outcomes_vs_Launch](https://github.com/Nifmoo/kickstarter_analysis/blob/main/Theater_Outcomes_VS_Launch.png)
  In order to determine success rate based on goal amount, I created a few arbitrary ranges that it could be included in and used a COUNTIFS() function to determine how many campaigns fell within the range and the outcome. I totaled the projects and then determine the percentage of successful and failed campaigns.
  ![
