# An Analysis of Kickstarter Campaigns
## Performing analysis on Kickstarter data to uncover trends for decision making.
### Through an in-depth analysis of crowdfunding data, this project aims to help guide decision making for playwright Louise who is embarking on her first crowdfunding campaign for her play *Fever*.  

## Successful Kickstarter Campaigns Analysis & Challenges
### How does the Launch Date and Fundraising Goal of a campaign affect the outcome of a Play Production? 
This analysis focuses specifically on whether factors such as the **Launch Date** and **Fundraising Goals** can impact the success of a play.

### Theater Outcomes Based on Launch Date
For the first portion of this analysis, I condensed the larger dataset to focus on Theater productions as a whole.
Within this category of Kickstarters, I analyzed whether the specific calendar month in which a theater campaign was launched could predict one of three outcomes:
1. Successful
2. Failed
3. Canceled

Pictured below is a line chart of this data. 

<img width="356" alt="Theater_Outcomes_vs_Launch" src="https://user-images.githubusercontent.com/89872154/133945937-e12e205b-0db6-468e-b76f-a0193a5fd7f4.png">

One portion of this analyiss that could have presented a challenge would have been the Unix timstamps listed in Column I of the main Kickstarter Dataset. This is not my first time working with Unix Timestamps, however, I can foresee how this would have been challenging to convert if one was unaware of this date and time formatting within Excel. Another potential challenge could be inherent in the fact that Excel is an American programming tool with month-day-year formatting for dates. Many other countries utilize ISO date formatting which could have made it difficult or confusing to validate your work. With some research into the way time is formatted in Excel, I believe these challenges are still possible to overcome despite someone's prior knowledge.

### Analysis of Outcomes Based on Goals
The second portion of the analyiss evaluates whether the specific dollar amount of a fundraising goal could help predict the success specifically of Plays within the Theater category of kickstarter campaigns. To do this, I created several uniform ranges for the fundraising goals and calculated the percentages of the same three outcomes mentioned in the previous section within each Goal range. This is visible in the below image.

<img width="468" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/89872154/133946621-048bec56-1294-497c-9de9-abc7b014c447.png">

### Challenges and Difficulties Encountered
I experienced some difficulty in the syntax of the COUNTIFs Formula. I could quickly validate that the intended formula was not delivering the correct results by switching back to the main Kickstarer dataset and manually filtering the columns captured in the formula. My formula was resulting in 0 returns which did not match teh data. This led to some further research on how to properly write such equations given the version of excel I was working with which solved the issue. I also encountered another issue when validating my chart against the chart provided in the course materials. I came to find that I unintentionally omitted an entire range: 
```
35000-39999
``` 
## Results
-One conslusion I can draw about the Outcomes based on Launch Date is that campaigns kicked off in the Spring or around the month of May have the highest number of successful Theater Outcomes.  A second conslusion is that fewer Theater campaigns are kicked off in the winter months.
-I can conclude that based on this specific set of data, more plays are succesful when provided a fundraising goal of between $1000-$4900. When analyzing the rate of success relative to fundraising amount, the data shows a downward trend up until fundraising goals reach $35,000-$45,000. 
-A limitation of this dataset lies in the timeframe from which this data was collected. I would like to see additional data collected over a longer period of time for increased accuracy of the sample size. Another limitation lies in the selection of the categories of outcomes depicted in this analysis. Specifically, what is the relevance of canceled campaigns in this analysis and how is this information useful towards understanding the success of a campaign? 
-Another table that would have been useful to analyze in the context of this project is the percentage of the fundraising goal that is pledged for each project and how that compares to the rate of success and failure based on Fundraising Goals. This could help expand both the definition and scope of how we understand "success." Additionally, Louise could certainly benefit from a more in depth analysis of the outcomes of plays within her fundraising bracket seeing as the percentage of failed and successful are similar.

