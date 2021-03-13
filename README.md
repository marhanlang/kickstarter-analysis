# kickstarter-analysis
Analysis on Kickstarter data to reveal trends 21.02.21

## Project Overview
Analysis of the results of campaigns depending on their launch dates and fundraising goals
### Purpose
The purpose of this analysis is to use the given data in order to determine the effect of launch dates and fundraiser goals on the overall success of a campaign.
## Analysis and Challenges

### Goal Outcomes
![Outcomes Based on Fundraiser Goal](https://github.com/marhanlang/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)
This Chart Can be used to visualize the percentage of Successful or Failed play campaigns.  To create this chart, the data had to be narrowed from all campaigns to exclusively theater/play data. After narrowing the dataset down to only necessary data, the individal pieces of data had to be counted (i.e. Number of success, failures, and total number of campaigns) and sorted.  With the sorted data, percentage of failures and successes can be calculated.
### Launch Date Outcomes
![Outcomes Based on Launch Date](https://github.com/marhanlang/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)
This chart is a visualization of outcomes of Theater campaigns based on the time of year they were launched.  Before being able to sort this data, the launch dates had to be converted from Unix timestamps to a standard date format. This was done by creating a conversion that multiplied the Launched_at number by dividing by 60, dividing the result of the first division by 60, dividing that by 24, then adding that to the date 1/1/1970 in this format : =(((J2/60)/60)/24)+DATE(1970,1,1). To create this chart, the data had to be filtered by the Parent Category, Theater, to narrow down the dataset to exclusively relevant data. The launch dates can then be sorted by month.
## Results

- Based on Outcomes by Fundraiser Goal, the most successful campaigns are the campaigns with goals below 1000 and next most successful group of campaigns are those with goals between 1000 and 4999. An ideal goal for a successful campaign would be less than 5000. 
- Based on the data from Theater Outcomes by Launch Date, May through July are the months with the highest number of successful campaigns. Therefore, the best months to launch would be between the start of May and end of July. 
- Alongside that, the same data shows that the month of December has the lowest number of successful campaigns. Thus, the worst month to launch a fundraising theater campaign would be in December.
### Limitations
This dataset does not detail how campaigns were advertised upon launch or the method backers used to donate that may provide further info on Fundraiser goal successes or failures.
### Suggestions for Further Analysis
This analysis does not account for the length of time a campaign was live. Length of campaign may account for some failures in campaigns achieving thier goals. Launch date analysis in combination with an analysis on Campaign length may provide a more comprehensive view on factors that make a successful campaign.
