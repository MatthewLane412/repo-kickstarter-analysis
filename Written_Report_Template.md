# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of this analysis is to help Louise run a successful kickstarter campaign to fund her theater project. Looking through historical data, we are able to determin insights that may help Louis run a successful campaign.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

Performing data analysis on thousands of crowdfunding projects we were able to uncover trends on Launch date. To do this, I needed the powerful tool, **Excel**. First, I needed to over come the challenge of converting unix time stamps to a short date (easily readable) for the start and end date of campaigns. **Code** ```=(((Unix Time Stamp/60)/60)/24)+DATE(1970,1,1)```. Next i needed to use the **text to columns** function in Excel to break out catgegory and subcategory into two separate columns. Then i input the data into a **Pivot table** (a powerful summarizing tool). With the **Pivot Table** i was able to summarize the outcome by months while filtering on the parent category "Theater". Finally, i used a **Pivot Chart** to create an easily digestable visual of the analysis. 

![Theater_Outcomes_vs_Launch](/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

Outcomes based on Goals tells us the number of successful and failed campaigns based on a particular goal range. To complete this analysis, I broke out the goals into ranges. Then , performed the ```countifs``` function in excel. to bring in the number of successful, failed and canceled campaigns. Then I used a ```sum``` function to add all three together (Total Projects). Next I divided the number of successful, failed and canceled one-by-one by Total Projects to get the percentage for each goal range. Finally, i created a line chart to show the trends by goal amounts. 

![Outcomes Based on Goals](/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered



## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  - Historically the most successful campains start in May and June. In addition, the least successful campaigns start in December. 

- What can you conclude about the Outcomes based on Goals?
  - The most successful campaigns are less than $1,000. Historically, campaigns less than $10,000 have over a 50% chance of success.     while the success rate between $35,000 and $44,999 is good,it is too small of a sample size to confiently say there is a high         success rate in that range


- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
