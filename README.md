# Kickstarting with Excel

## Overview of Project

The purpose of this project was to help Louise determine how other kickstarter campaigns did in relation to when they were launched, and what their initial funding goals were.  This will allow her to compare her campaign for her play *Fever* to other plays that have raised money through Kickstarter.  

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date: 
To evaluate the outcomes of the theater campaigns based on their launch date I aggregated the total number of successful, failed, and canceled campaigns by generating a pivot table from the initial dataset. The pivot table also enabled me to organize the data specific to theater campaigns by month for these three categories.  With the relevant data organized and filtered correctly within the pivot table I was then able to create a line chart (INSERT LINE CHART LINK) that provided a visual for all theater campaigns over time, based on their outcome and launch date.

### Analysis of Outcomes Based on Goals: 
To evaluate the outcomes of each theater campaign based on their goal I created a table (INSERT TABLE IMAGE LINK) that aggregated the total number of campaigns in each outcome category (successful, failed, or canceled) by various dollar ranges.  With this aggregated information I was also able to calculate how many campaigns are successful, how many fail, and how many are canceled based on their initial goal amount.  

### Challenges and Difficulties Encountered: 
I did not encounter any challenges with regard to the Outcome by Launch Date analysis, but recognize that it could be very difficult to complete this analysis if the data was not properly filtered, or if a pivot table could not be created.  The pivot table is very helpful in synthesizing the data and making it more visually digestible. With regard to the Outcome Based on Goal analysis I leveraged the countifs() function and ran into a small snag when trying to reference values within a cell that defined my dollar ranges.  After leveraging Google I was able to learn the proper syntax for referencing the cell that held my dollar range so that I could then copy the formula to all other ranges and have it be dynamic.  Example: Originally I tried to end the function statement by writing (…,”<A1”) where cell A1 held a value of 1000 for my first range. I learned that in order for it to work you have to write (…,”<” & A1).  Without that knowledge I would have had to manually add the top and bottom dollar amounts for each range by typing the numeric values into the function on each row.           


## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?  
The first conclusion you can draw is that May seems to be the best time to launch a campaign. Roughly 67% of the campaigns launched in May succeed versus an average success rate of approximately 60% across the other months of the year.  It also appears that December is the worst time to try and launch a campaign since nearly 50% of the campaigns fail during this month.    

### What can you conclude about the Outcomes based on Goals?  
Based on the line graph it appears that as campaigns increase in goal size their likelihood of failing increases.  This is true up to a dollar amount of about $25,000.  Above $25,000 the number of campaigns in each range starts to dramatically decrease in sample size which makes it difficult to establish a trend since the result of each campaign carries so much weight.  It also should be mentioned that not a single campaign for a play has been canceled over this time period, which would suggest that there is generally a lot of support for play campaigns, but perhaps some campaigns just set a goal that is to high; launch at the wrong time; or miss their goal for other reasons.    

### What are some limitations of this dataset?  
One limitation of this dataset is that there is no genre information for the various campaigns.  The “blurb” section is helpful in describing the topic of each campaign, but if there was genre information that would provide a nice data point for being able to determine which topics or styles tend to garner the most interest when it comes to meeting their funding goals.     

### What are some other possible tables and/or graphs that we could create?  
One possible pivot table that could be created would be to include the the “pledged” information to illustrate how campaigns perform by category. From this pivot table you could generate a stacked bar chart that could show how much money has been contributed to each category versus the combined goals for the category.  With this information you could tell if certain categories tend to make their goals; miss by a little; or miss by a lot.  Categories that miss by a lot may need to make only minor changes to hit their goals, but categories that miss by a lot may need to rethink their entire campaign.
