# Kickstarting with Excel - An Analysis of Kickstarter Campaigns
- - -
## Overview of Project
Our friend, Louise, needs to raise $10,000 for the performance she is organizing, *Fever*.  In this Module, we were tasked with sorting through a relatively large data set which included informaiton about past kickstarter campaigns in the hopes of revealing trends that would help Louise determine if her monetary goal is reasonable and establish when during the year she should launch her campaign to optimize her efforts.
- - -
### Purpose
While completing this module students were introduced to some of the automated features that Excel has to offer such as:
 - formatting cells,
 - Sorting and filtering mass amounts of data,
 - Creating new sheets within a workbook,
 - Using formulas to perform calculations using data spanning multiple sheets,
 - Creating easily manipulated pivot tables,
 - Generating visually appealing charts to display our data quickly to the user.

In addition to the functions of Excel, students were introduced to commonly used statistical methods such as; the mean, median, mode, and quartiles, to help our client, Louise, determine what an appropriate goal would be for her fundraiser based on the success of failures of others.  After reviewing our initial data, Louise's kickstarter campaign began and she quickly approached her goal, but now she wants to see how her campaign measures up to similar fundraisers!

- - -
## Analysis and Challenges
To generate this analysis the first thing we needed to do was create an easily manipulated pivot table.  In our pivot table we included the number of successful, failed, and canceled kickstarter projects and filtered the results to only include those related to theater productions.  We also sorted this data to display which months of the year had the most campaigns in each of the aforementioned categories.  [See source file](kickstarter_challenge_COPY.zip).

### Results:  Outcomes Based on Launch Date

![Outcomes based on launch date](https://github.com/murphyk2021/kickstarter-analysis/blob/4ef50dc63bad0f72920e3418cfb52275bbced9d5/Theater_outcomes_vs_Launch.png)


From the graph above, we can clearly see that the greatest number of successful campaigns were luanched during the month of May.  However, it is important to note that the highest total number of campaigns (166) were launched during the same month. To confirm that we have not accidentally come to the false conclusion that May has the best chance of success, it might be interesting to take this one step further and look at the *percentage* of successful campaigns launched in each month. 

![Percentage of Successful, Failed, of Canceled Kickstarters based on Launch date](https://github.com/murphyk2021/kickstarter-analysis/blob/4f5b13f948bb4e31eff157e442898b7778bf40c7/Theater_outcomes_vs_Launch_Percentage.png)

From this adjusted graph we can confirm that historically May does have the greatest number of launched campaigns but it also has the greatest success rate of the entire year at 67%.  May also had the lowest fail rate(31%).  This is likely the reason May is a popular month for campaigns to be launched! However, if Louise wanted to hold off on beginning her campaign until June, there wouldn't be a significant difference in her chances of success (based on the launch date alone).

**Challenges with this analysis**
Making this additional graph was a helpful step for me as I had to reference Google for guidance on changing the calculation for the outcomes column. It turned out to be failry simple: Add a second count of the "outcomes" and adjust the field category to "% of the row total".  See image below.  To create the graph I referenced [this forum](https://superuser.com/questions/1327704/excel-pivot-with-percentage-and-count-on-bar-graph) to help me create a "combo" graph with a secondary Y-axis.

![Adjusting the Pivot Table to show Percentages instead of total counts](https://github.com/murphyk2021/kickstarter-analysis/blob/4ef50dc63bad0f72920e3418cfb52275bbced9d5/making%20a%20percentage%20of%20the%20s_f_c%20kickstarters%20by%20launch%20date.png)

- - -
### Results Outcomes Based on Goals
To determine the relative success of fundraisers for plays with regard to their goals, we needed to create another worksheet in our workbook that would automatically look through our original data set and identify how many play campaigns had goals within a certain range and how many of those campaigns were successful.  We used a "CountIf" to achieve this goal.  See the set up below.
![Using the "CountIf" Statement](https://github.com/murphyk2021/kickstarter-analysis/blob/31442fdc34979290fa8711ff26d7995c47a23e5b/countif.png)

From this data we can easily create a line graph which shows the percentage of campaigns which were successful or not.  
![Outcomes based on Goal](https://github.com/murphyk2021/kickstarter-analysis/blob/38326a69ed9dadaf2704cb7424691956f6252e47/resources/Outcomes_vs_Goals.png)

From this data there appears to be some important monetary brackets to avoid.  For example, campaigns that set their goals between $5,000 and $35,000 are generally less successful than those set <$5,000.  However, we do see some increase in success in the range of $35,000 and $45,000. 

If we also include the number of total campaigns within each financial bracket we can also see that most of our campaigns had goals on the lower end of our data. See grah below.
![Outcomes based on goal with total number](https://github.com/murphyk2021/kickstarter-analysis/blob/8d3060f189b68bf852797e1dee835832e53f7db0/resources/Outcomes_vs_Goals_with_totals.png)

###Additional Information Needed
Other information that might be interesting to present to Louise would be how many of these successful campaigns exceeded their goals and by how much.  It is possible that some of these underestimated their potential success! Additionally, how unsuccessful were the failed campaigns.  This data might give a little more insight into the trends of pledges.    

Additionally, we may want to include an analysis of how long each campaign was live.  This will help ensure that her audience is motivated to pledge quickly but also allows enough time to get the word out and push the campaign.

###In Conclusion
Based off of these 2 parameters alone, Louise is doing quite well if she is close to her goal of $10,000!  


- - -

