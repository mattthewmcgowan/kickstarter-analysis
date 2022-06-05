# Kickstarting with Excel

## Overview of Project
Analysis of Kickstarter data with an outcome based centralization.
### Purpose
To analyze the correlatoion between outcome and other variables. 
## Analysis and Challenges
The first analysis was taking a look at the correlation between the Category 'Theatre' and the success, failure, and cancelation rate based on 'Launch Date'. Although the data is collected over many years, for this analysis the 'Launch Date' referes to the specific month the Kickstarter campaign was launched. This analysis was performed by putting the data in a pivot table. From there I was able to narrow down the desired critera.


<img width="500" alt="Theater_Outcomes_vs_launch" src="https://user-images.githubusercontent.com/106042900/172065075-37b16f12-442c-4479-8c40-093bb2556aa1.png">


The second analysis performed took a look at the relationship between Outcomes, (successful, failed, and canceled) and Goal ranges. In the chart below you will see that 80% of Kickstarters succeeded when their goal pledge amount was less than $1,000. This analysis was performed by using the countifs function to count if a particular kickstarter was inside the desired goal range, if it had succeeded, failed, or canceled and lastly if it was under the subcategory of Play. 


<img width="500" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/106042900/172066031-6650ca5f-a86b-4f97-806b-58c5c75b6518.png">

The major challenge was utilizing the countifs function to seperate the data. I was having a hard time organizing the equation to pick the correct column I wanted it to search first, second, third. Eventually I was able to recongnize that I did not have one of the columns in the absolute status therefore anytime I copied my countifs formula over it would think I wanted to shift the cololmn over in my equation as well. 
### Analysis of Outcomes Based on 'Launch Date' is in monthly increments. 
This analysis started with creating a pivot table to better format the data. I was able to pull over the categories that I needed from there and filter down anything that was not useful. From there I inserted a stacked line chart to show the relationship between the theatre outcome based on launch date.
### Analysis of Outcomes Based on Goals
The analysis of Outcomes Based on Goals tells us that the overwhelming majority of Kickstarters have a goal range of $10,000 and below. It's also telling to see that play Kickstarters in the ranges $1,000 and below and $1,000 to $4,999 are both successfully funded over 70% of the time. This would be useful information to give to anyone wanting to raises for thier upcoming play. It would be wise to keep their production relatively small between this $4,999 or less. 
### Challenges and Difficulties Encountered
As stated above, the biggest technical challenged faced when analysing the data set was setting up the countifs funcion properly. Counting the first category or ranges was not difficult. It was adding multiple columns and variable to the already established equation that was difficult. I was able to overcome that hurdle whenver I realized that the column I was counting shifted right when I copied my equation to the two right cells. I made the Outcomes column an absolute useing the PF4 key and the equation counted without a problem. 
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. We can conclude that launching a Kickstarter in the summer months (May-Aug) has a higher probability of being successful.
2. We can conclude that more than half of all Kickstarters will fail or be canceled. 
- What can you conclude about the Outcomes based on Goals?
The conclusion would be that Kickstarter campaigns less than $5,000 are more successful than those over a $5,000 goal amount. 
- What are some limitations of this dataset?
During the analysis one thing that did come to mind was, "WHO did the funding?" One limitation of this data set is that it does not showing any pledger/donater information. In my opinion, that would give you a littme more insite into WHO these Kickstarters are for and who's essentially paying the bill. That is directly tied to the success rate just as much as the lauch date. 
- What are some other possible tables and/or graphs that we could create?

A simple bar chart reflecting the difference between number of Total Projects versus the Number of Successful campaigns. 

<img width="500" alt="OutcomeBasedOnGoal2" src="https://user-images.githubusercontent.com/106042900/172067600-ba31f8f3-1605-463d-97b6-fb2acc2b0591.png">
