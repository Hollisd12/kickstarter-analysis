# An Analysis of Kickstarter Campaigns

## Overview of Project

### Purpose 
In this project, we evaluated data for crowdfunding campaigns from 2009 to 2017. Louise is an up-and-coming playwright who launched crowdfunding campaign to help fund her play *Fever*. Her campaign came close to its fundraising goal in a short amount time. She wants us to help her visualize how similar campaigns fared in relation to their launch dates and funding goals.

The purpose of this project is to examine global kickstarter campaigns, specifically Plays, to better determine whether there are specific factors that make a project's campaign successful. In our analysis, we hope to uncover if there are trends around successful campaigns and their launch dates and goals. Additionally, our analysis will help Louise determine how her campaign fared against other similar kickstarter campaigns.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In our first analysis, we investigated the outcomes of campaigns based on their launch date, specifically Theater campaigns. We created a Pivot chart to better analyze this data. First, we had to add a new column to the Kickstarter sheet labeled "Years." In this new column, we used the =Years() function in Excel to extract the year from the launch date of each campaign. Next, we created a pivot table from the Kickstarter sheet and added filters for the Parent Category and Years. Our Pivot table displayed the data below:

![Pivot Table](https://user-images.githubusercontent.com/112137694/190038580-113136c9-cf13-4fbd-8309-5800569ae6fa.png)

From that pivot table, we created the following line graph to visually display Theater outcomes based on launch date.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/112137694/190038498-e3615ed1-f2bb-4a00-a8a1-975a319bb710.png)

### Analysis of Outcomes Based on Goals
In our second analysis, we evaluated the outcomes of campaigns based on their fundraising goals, specifically, campaigns for Plays. We created a table in new sheet to and used the =Countifs() function in Excel to analyze the number of successful, failed, and canceled campaigns in the Play subcategory based on the goal amount. After pulling the data for the outcomes of the campaigns, we pulled the percentage of successful, failed, and canceled plays from the total number of projects. After creating the table, we were able to create the visualization of outcomes based on goals in the line graph below.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/112137694/190038918-bd07d472-7cc8-47a4-843c-390d42883603.png)

### Challenges and Difficulties Encountered
This analysis required the creation of additional columns to the original data set. For example, the launch date and end date data were in a format that may be difficult to comprehend at a glance. Two new columns were needed to convert the date created and date ended data into a standard date format that is easy to understand. To convert the date, we take the data in the launced_at column and divide by 60, divide by 60, divide by 24, and add the formulate DATE(1970,1,1).

Additionally, when creating the pivot table for the Outcomes Based on Launch Date analysis, setting the correct row field for the pivot table could prove to be challenging. For an effective analysis, the rows should be displayed as months. However, the data in the Kickstarter sheet is listed as a full date. When adding the Date Created Conversion field to the Row of the pivot table, you need to remove the Years and Quarters fields to clean up the data. 

## Results

- What are two conclusions you can draw about the Outcomes Based on Launch Date?
  - First, we can determine that May, June, and July, launched the highest number of successful campaigns in the Theater category. April through July appears to be ideal for launching campaigns as successful campaigns accounted for the highest percentage of total campaigns launched in this time frame while the percentage of failed campaigns remained relatively low.
  - Secondly, in our analysis we can conclude that May, June, July, August, and October all saw relatively the same amount of failures. The overlap of high successes and high failures could be due to the fact that during the months of May through August there were more total campaigns launched than any other time of year. 
- What can you conclude about the Outcomes based on Goals?
  - In our analysis of Outcomes Based on Goals, we can conclude that Plays with a goal of less than $14,999 and goals between $35,000 to $44,999 saw the highest percentage of successful campaigns. 
- What are some limitations of this dataset?
  - With this data set, it is difficult to determine if there are other factors outside of the launch date and goal that could be affecting the success of the campaign. Additionally, there isn't any data to determine why a campaign would be canceled as opposed to failed. We have to keep in mind that there could be other factors affecting outcome as we perform our analysis on this data set. 
- What are some other possible tables and/or graphs that we could create?
  - We could create a graph to compare how the length of the campaign affects the outcome. By visualizing the length of campaigns we could also determine how long a campaign with a high goal would need compared to a campaign with a low goal.  
  - We could create a graph or table to visualize is the campaign was spotlighted and how that affected the outcome. 
