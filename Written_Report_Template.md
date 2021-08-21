# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of this analysis is to help Louise run a successful kickstarter campaign to fund her theater project. Looking through historical data, we are able to determin insights that may help Louis run a successful campaign.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

Performing data analysis on thousands of crowdfunding projects we were able to uncover trends on Launch date. To do this, I needed the powerful tool, **Excel**. First, I needed to over come the challenge of converting unix time stamps to a short date (easily readable) for the start and end date of campaigns. **Code** ```=(((Unix Time Stamp/60)/60)/24)+DATE(1970,1,1)```. Next i needed to use the **text to columns** function in Excel to break out catgegory and subcategory into two separate columns. Then i input the data into a **Pivot table** (a powerful summarizing tool). With the **Pivot Table** i was able to summarize the outcome by months while filtering on the parent category "Theater". Finally, i used a **Pivot Chart** to create an easily digestable visual of the analysis which shows: Historically the most successful campains start in May and June. In addition, the least successful campaigns start in December. 

![Theater_Outcomes_vs_Launch](/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals



### Challenges and Difficulties Encountered



## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
