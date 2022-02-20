# kickstarter-analysis
Module 1 - Performing analysis on Kickstarter data to uncover trends
# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of this analysis is to help Louise meet her crowdfunding campaign goal to fund her play, Fever, by identifying any trends in successful funding campaigns in relation to their launch dates and funding goals from data collected from almost 4,000 theater campaigns. With a budget estimated of over $10,000, this analysis aims to help Louise mimic other successful campaigns to meet her goal. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
A pivot table was generated, and a line graph created to display the total number of outcomes based on the month that the campaigns were launched. As seen in the graph below, May had the highest number of successful theater campaigns launched, whereas December had the lowest number of successful campaigns.

![image_name](https://github.com/lucymccanna/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png) 

### Analysis of Outcomes Based on Goals

In this part of the analysis, the data was catered to Louise by looking only at campaigns for plays. The total number of successful, failed, and cancelled play campaigns were summed using the COUNTIFS excel function, and the percentages of each outcome were calculated across 12 ranges in 5,000-dollar intervals. As displayed in the graph below, campaigns with goals under $5,000 had the highest success rates. Campaigns with goals from $15,000 to $35,000 and greater than $45,000 had more failed campaigns than successful.

![image_name](https://github.com/lucymccanna/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

When generating the pivot table and line graph for Theater Outcomes Based on Launch Date, the fields in the Filters, Columns, Rows, and Values must be correctly entered in order for the table to be valuable to the analysis. In this case, evaluating the campaigns based on month launched was more relevant. To view the outcomes based on months, the analyst must remove Years and Quarters from the Rows/Axis. Without understanding how to utilize the PivotTable fields, it would be challenging to create a table or graph that is beneficial to the analysis.

Challenges may also arise when automating excel functions, such as the COUNTIFS function used to generate the Outcomes Based on Goals sheet. If the COUNTIFS function entered contains a relative reference (for example, D:D) and the function is copied into the next cell to the right, the reference within the equation will shift over one column in the equation (in this example, to E:E). To avoid the reference shifting, the dollar sign ($) character is used to indicate that the range is an absolute reference, meaning when the formula is copied to another cell the absolute reference will not change.


## Results

Based on the data collected, May is the best month of the year to launch a campaign for plays. The plays launched during this month were 66.9% successful and contained the highest number of successful outcomes, at 111 campaigns. Campaigns launched in December were the least successful, with only 27 out of 75 plays having a successful outcome (or 49.3%). 

Looking at the data for all theater campaigns, those with goals under $5,000 had the highest success rates. Campaigns with goals from $15,000 to $35,000 and greater than $45,000 had more failed campaigns than successful. 

A limitation of the dataset is that the currency for the goal and pledge dollar amounts vary across each campaign. To accurately analyze the outcomes based on goals, the dollar amounts should be converted to a single currency. Another limitation is that the plays are not identified by genre. If Louise could analyze the data for plays with the same genre as her play, Fever, she may be able to identify different trends in the successful campaigns most similar to hers to help maximize her crowdfunding.  

Another Pivot Table/graph we could create to support our analysis is one that shows the total number of outcomes based on the duration of the campaign. 


