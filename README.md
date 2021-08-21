# Kickstarting with Excel

## Overview of Project

### The purpose of this analysis is to help Louise with her play *Fever* campaign. Her campaign has successfully come close to its fundraising goal in a short time, and now we want to help her analyze how well her campaign went compared to others based on their launch dates and funding goals.

## Analysis and Challenges

### I first started my analysis by creating a pivot table filtered by parent category *theater* and years to see the trend over time. The values I analyzed were 3 categories of outcomes; **successful**, **failed**, or **canceled**. From the pivot table I then created a line chart to display a visual to see the trend in outcomes over time breaking it down by months.
![Theater_Outcomes_vs_Launch](C:\Users\marav\Documents\Columbia Data Analytics Bootcamp\Module 1\Challenge 1\Resources\Theater_Outcomes_vs_Launch.png)

### Next, I created another line chart showing *outcomes based on goal*. To create this chart I first created a table with goal ranges, ranging from *less than 1000* up to *greater than 50000*. From here I used the **COUNTIFS** function to pull together the total number of **successful**, **failed**, or **canceled** plays in relation to the goal amount. Once I captured all these values I found the percentage values of each category by comparing the total number of each outcome category of plays by the total number of projects. From this point I created the line chart (below) which shows **success**, **failure**, or **canceled** play trends depending on the fundraising goals.
![Outcomes_vs_Goals](C:\Users\marav\Documents\Columbia Data Analytics Bootcamp\Module 1\Challenge 1\Resources\Outcomes_vs_Goals.png)

### During my analysis I faced a few challenges while developing both line charts. The first challenge I faced was while putting together the pivot table for the *Theater Outcomes Based on Launch Date*, was breaking down the years to months. To overcome this challenge I referred back to a previous module 1 exercise for guidance. By doing so I found that I needed to add another field into rows which was the *Date Created Conversion* dataset.
### The second challenge I faced was when performing the **COUNTIFS* function to calculate the number of *successful*, *failed*, or *canceled* plays. It was a challenge when there was a range to look up (e.g. 20000 to 24999). To overcome this challenge I watched the hint tutorial provided in the module and learned how to account for a multiple conditions using the countifs function.

## Results

### -Two conclusions I can draw about the Outcomes based on Launch Date:
	1. There is a lot more successful theater campaigns than there are failed or canceled. 
	2. Campaigns seem to have spiked more success in the summer months. For example in May/June the number of successful theater campaigns were over 100.

### -My conclusion about the Outcomes based on Goals is the higher the fundraising goal the less successful the campaign is. However, based on our dataset there seems to have been a spike in success rates for fundraising goals set around 35000 to 40000 which may indicate our dataset may have some limitations of extreme outliers that are impacting our analysis.

### -Some limitations of this dataset specifically if we look at the *Outcomes Based on Goals* chart is that the percentage of **successful**, **failed**, or **canceled** plays may not be the best comparison to do with this data given that the number of plays based on the fundraising goal are not similar in number. There are far fewer play campaigns with high fundraising goals compared to those with lower goals and therefore the population measuring each category may be skewed. 

### -Some other possible tables and/or graphs that we could create for our analysis is a **Box and Whiskers Plot**, which could show us the common range for where more theater/play campaigns fundraising goals are set to. It also will show any extreme outliers that may impact out analysis. We could also create a **Box Chart** to better visualize the volume of *successful*, *failed*, or *canceled* plays compared to each other. 
