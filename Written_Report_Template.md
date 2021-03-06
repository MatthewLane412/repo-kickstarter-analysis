# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of this analysis is to help Louise run a successful kickstarter campaign to fund her theater project. Looking through historical data, we are able to determine insights that may help Louise run a successful campaign.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

By performing data analysis on thousands of crowdfunding projects, I was able to uncover trends on Launch date. To do this, I needed the powerful tool, **Excel**. First, I needed to over come the challenge of converting unix time stamps to a short date (easily readable) for the start and end date of campaigns. **Code** ```=(((Unix Time Stamp/60)/60)/24)+DATE(1970,1,1)```. Next I needed to use the **text to columns** function in Excel to break out catgegory and subcategory into two separate columns. Then I input the data into a **Pivot table** (a powerful summarizing tool). With the **Pivot Table** I was able to summarize the outcome by months while filtering on the parent category "Theater". Finally, I used a **Pivot Chart** to create an easily digestable visual of the analysis. 

![Theater_Outcomes_vs_Launch](/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

Outcomes based on Goals tells us the number of successful and failed campaigns based on a particular goal range. To complete this analysis, I broke out the goals into ranges. Then , performed the ```countifs``` function in excel to bring in the number of successful, failed and canceled campaigns. Then I used a ```sum``` function to add all three together (Total Projects). Next I divided the number of successful, failed and canceled one-by-one by Total Projects to get the percentage for each goal range. Finally, I created a line chart to show the trends by goal amounts. 

![Outcomes Based on Goals](/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
 - Converting unix timestamps to a short date.
   - This was a new challenge for me. I needed to read documentation on the web to learn about conversions.
 - Creating countifs statement.
   - At first, I created the countifs to have greater than or less than. Soon realizing, it needed to be 'greater than or equal to' or 'less than or equal to', to complete the assignment. 
 - Creating Pivot Tables and summarizing on the best information.
   - Figuring out which fields were the best to include in the pivot tables.


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  - Historically the most successful campaigns start in May and June. In addition, the least successful campaigns start in December. Most campaigns launch in late Spring to early Summer
   
- What can you conclude about the Outcomes based on Goals?
  - The most successful campaigns are less than $1,000. Historically, campaigns less than $10,000 have over a 50% chance of success. I would recommend keeping the kickstarter campaing under $10,000.   

- What are some limitations of this dataset?
  - The sample size is relatively small
  - Not all of the data set is for the nitch market Louise is getting into

- What are some other possible tables and/or graphs that we could create?
  - Pivot table utilizing the filter for Staff Pick. If staff pick is true the success rate is very high.
  - Pivot table utilizing the fileter for Spotlight. If spotlighted, the success rate is 100%!
