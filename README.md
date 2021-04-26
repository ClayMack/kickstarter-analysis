# Kickstarter Analysis Results and Conclusions

## Overview of Project

> The purpose of this assessment is to analyze kickstarter data to find trends that provide the client a better understanding of various kickstarter theater campains and their success rates. 

## Analysis and Challenges

> We can study how various theater campaigns fared in relation to their launch dates and their funding goals to get an understading of the key variables that are controlling success rates. 
>> 1. Outcomes Based on Launch Date:

> This analysis was built utilizing a pivot table to seperate out campain success as a function of the launch date (i.e. month). From the table a line chart was created to see if there is a pattern in the success of a play based off of when it was launched. I did not have any challenges with this, but one could encounter a problem if the date was not converted from from UNIX time to standard date. 

>![Graph ploting theater outcomes based on the launch date.](https://github.com/ClayMack/kickstarter-analysis/blob/main/Resources/Theature_Outcomes_vs_Lauch.png
"This is a sample image.")


>> 2. Outcomes Based on Goals: 

> This analysis was performed using the COUNTIFS() statement in the kickstarter play data to bin goal size based on size. A table was created that seperated out campain goals in $5,000 increaments and whether or not a goal was successful, failed, or canceled. Lastly the percentates of success, failed, or canceled outcomes  were calculated by bin using the =sum() function then dividing the sum of each case by the total. This was done in order to see if there was a trend with the size of the goal and wether or not the campain was successful, failed, or canceled. This workflow was completed with no diffuculty, but the results could be biased due to the sample size of the larger goal amounts. There were numerous small goals but very limited number of higher goals. The effects can be seen between $35,000 to $50,000. The success percentages were really high but only acounted for a small number. This could give a false impression that campain goals of this size are realativly successful, when in reality they are likely less likely to be successful than smaller goals. 

![Graph ploting theater outcomes based on goal amount.](https://github.com/ClayMack/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)



## Results

> When looking at success of a kickstarter campain based on the month the campain launch, we see a couple of trends. In May/June we see a large spike in successful theater campains that begins to trail off in July. There also seems to be substantial drop in success from November to December.

>Taking a look at how successful plays are based on the size of the goal, you can see a clear pattern. Goals with lower amounts tend to be very successful and the success rate tends to drop as the size of the campain goal increases. 

> As mentioned in the analysis, there could be some limitations with the dataset due the distrubtion of goal size (sample bias). This could lead to an underrepresentation of larger campain goals and could be misleading. My recommendation is to look at the line graph and plot a trendline of the data and not fixate on individual goal size outcomes.

![Graph ploting theater outcomes based on goal amount with added trendlines.](https://github.com/ClayMack/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals_trendlines.png)
