# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of this analysis was to help our client, Louise, discover funding trends pertaining to Kickstarter campaigns for theatrical plays.  We used a large database of Kickstarter campaigns' information, such as goal amount, amount pledged, the date the kickstarter began and the date it ended, type of project the kickstarter was for, etc.  This information was used to determine the trends of successful kickstarter campaigns as well as failed kickstarter campaigns.  

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
The first step in the analysis was to take a look at our dataset.  It is important to know what the data in each column/row represents.  The first challenge to overcome was to convert the time stamps into readable dates by creating a new column.  We then used the data to creat a pivot table that sorted by the parent category (Theater) and the years.  By putting the months in the rows bin and the outcomes in the columns bin we were able to create a pivot table to show the outcome of the campaign based on the month the campaign was started in.  We used the data in the pivot table to creat the below chart that illlustrates the outcomes of campaigns based on the month they launched in. 
![Theater_Outcomes_vs_Launch.png](https://github.com/bwheeler98/kickstarter-analysis/blob/2828133ac7ada6b3e2c06d1145651cde5473e29a/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
To discover the trends of outcomes based on the goal amount we had to create a new sheet within the workbook.  On this new sheet we created a table of 8 columns and 12 rows.  The columns included the number of successful, failed, and canceled campaigns for each row as well as the total number of campaigns for each row.  We also included the percentage of each outcome for every row.  Each row was a range of the goal amount, i.g. $0-$999, $1000-$1,499, etc.  To calculate the data in each column we had to use the COUNTIFS formula to calculate the total number of outcomes based on the filters we used in the formula.  We then created a line chart based on the the ranges of goal amount and the percentage of each outcome for each range.
![Outcomes_vs_Goals.png](https://github.com/bwheeler98/kickstarter-analysis/blob/2828133ac7ada6b3e2c06d1145651cde5473e29a/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
There was not to many challenges that we encountered for this analysis.  The first challenge was to take the date created time stamp and convert it into a readable date.  Another challenge one may have when analyzing the outcomes based on goal amount is to properly filter the COUNTIFS formula.  There were mutliple filters that were required to get the right total count for each range.

## Results
The analysis concludes that the best time for Louise to start a kickstarter campaign would be May-June, for these two months had the highest successful campaigns.  Louise should avoid starting her Kickstarter campaign after September as there are less successful campaigns from September to Decemeber.  The successful kickstarter campaigns for plays tend to have lower goal amounts than the failed campaigns did.  Louise should aim to have her goal amount to be around $2k-$3k.  There are some limitations for the dataset.  For instance, the data can be sorted by country, but if it was sorted down to cities or regions Louise would have a better idea on if her campaign will succeed in her targeted area.  We could then create tables and charts to determine the best area in a country for her Louise to advertise her campaign.  The data could also be filtered down to the type/genre of the play Louise intends to put on.    
