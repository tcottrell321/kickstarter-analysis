# An Analysis of Kickstarter Campaigns
# NOTE TO GRADERS - Complete Analysis with imbedded graphics is contained in the pdf file in this repository titled "An Analysis of Kickstarter Campaigns." 

## Purpose of the Analysis
Our Client, Louise, wants to create a Kickstarter Campaign to fund her new US Based Theatre Play. She estimates she will need to raise $10-12K.  In order to ensure success with this campaign, she requested an analysis of past Kickstarter Campaigns to determine if there were any common attributes or trends leading to success. Using data from over 4000 campaigns, the data was filtered, sorted, augmented with calculated columns, and statistically analyzed for any findings that might be useful to Louise. This report contains both the analysis as well as Final Recommendations

## Methodology
We followed the standard Data Science Methodology shown below. We were able to skip step one as the original data file (Excel) – which had been previously Extracted from the Kickstarter website API – was provided to us. It was stored locally in Excel format while we did our wrangling and data analysis.

## Exploratory Data Analysis
In exploring the data file, we discovered that we had over 4000 Kickstarter Campaigns from multiple countries – with fundraising goals ranging from a small ($1) to very large Campaigns of $100,000,000. However, as you can see from the plot below, only a small percentage of the campaigns sought these very large amounts of funds. 

To perform a meaningful analysis for the Client, this indicated that we would most likely need to filter the data down to a more relevant set of data – possibly excluding the very large Campaigns which were not relevant to Louise goal of $10-12K. We would filter by  by Category and SubCategory of the Campaign, plus Geography, Outcome, and Timing of Campaign Launch to look for any correlation to Success of the Campaigns.

Looking at U.S. Only Data across all Categories, we see the following results. What stands out for Louise, is that the Categories with the highest percentage of Success were Theater, Music, and Films.  This is good news for Louise who will launch a Campaign in the Theatre Category. Further drill down to the “Play” SubCategory will be needed.   

In order to perform meaningful analysis, we added additional columns of data for:  
1) Percentage Funded
2) Average Donation (with error handling)
3) Category and Subcategory as separate columns
4) Conversion of Unix timecodes to universal dates
5) We also added a Statistical Analysis Summary Table to include Averages, Mean, Std Deviation, and IRQ for both the Goal and Pledged Columns of data.  
 
## Final Conclusions
1. To be successful, individual Theatre Play Campaigns should not exceed $2000. Louise's Proposed Campaign of $20,000 exceeded that threshold significantly, therefore has little chance of success unless the target is lowered. 
2. Seasonality affected the success of Theatre Play Campaigns and are best launched in May of each year. 
3. Theatre Play Campaigns in Great Britian had a higher success rate when adhering to the limit, therefore, Lousie might consider running her play and Campaign in Great Britain if she has that flexibility. 

## Research Questions
1) Would timing of the Kickstarter Campaigns affect the Outcomes 
2) Would the Goal Amount affect the Outcome.   
3) Within the Play Category, how did Campaigns compare to other Subcategories.  
4) Might there be some logical Incentives based on the size of do

## Data Wrangling
There was no need to do a lot of Data Wrangling of the data as it was provided in reasonably complete excel spreadsheet format. However, we needed to add some additional columns of “calculated” data in order to complete our analysis. We added additional columns of data for:  
• Percentage Funded 
• Average Donation (with error handling)  
• Category and Subcategory as separate columns 
• Conversion of Unix timecodes to universal dates 

In addition, we created a Summary Table with 12 Histogram Bars to see if there was any correlation between the $ Goal of the campaign and its success. Further statistical analysis was performed on this data to show Mean, Median, and Std Dev along with IRQ.

## Data Analysis 
Focusing only on the SubCategory for Play Campaigns, we created the 2 Tabular Summary Tables below followed by 3 additional graphs to continue our analysis.  From the Summary Tables we can see that Play Campaigns varied in their success from: 
• 0% - 76% with an Average Success Rate of 66% (See Tabular Data and Pie Chart). 
• Campaign Goals Less than $5K had the highest success ratings. (See Line Chart).  

We then reduced our filtering of the Data from just “Plays” to all SubCategories of the Theatre Parent group and created a chart showing Outcome Based on Launch Date. From this graph below, you can see there is a significant correlation between Launch Data and Trend with the highest success achieved in May-June Launches. 

We then drilled down further creating a Summary Table for the Theatre Campaigns of the Mean, Mediian, Standard Deviation and IQR ending with a Box chart to graphically represent this data. 

From the final chart, we can see that Louise goal of raising $10-12K will be challenging and is in fact an outlier of Success with only a single Theatre Campaign getting $10K Pledged. The Mean was closer to $1000. To be successful, Louise will have to lower her goal significantly, or think of ways to build more awareness and preference to contributing to her campaign, possibly through Donation Incentives.  
 
## Recap of Final Conclusions
1) To be successful, individual Theatre Play Campaigns should not exceed $5000. Louise's Proposed Campaign of $12,000 exceeded that threshold significantly, therefore has little chance of success unless the target is lowered or donation incentives increased. 
2. In general, as the Campaign Goal amount increased, Success percentage dropped and Failure Rates increased. Campaigns below $5K had a much higher chance of success.  
3. There is an anomaly in the data at the $25-35K level. We see that success peaks back up to the 73-80%. This is unexplained and may be for Theatre Building projects, not just Plays.  
4. Seasonality affected the success of Theatre Play Campaigns and had the greatest success when launched in the May-June timeframe of each year. Louise might consider launching during this timeframe to increase chances of success.  
 
 ## Edinburgh Research/Additional Recommendations 
 The Client was also interested in doing a future project – specially a play for the market in Great Britain. She had 5 specific plays that she was interested in. We pulled the data on those 5 Plays and we pulled data on all US Campaigns, then more specifically GB Play Campaigns –  with the results shown below.   
• From the data we can see that in general, GB Plays had a Success Rate about 75% versus US of 65%. For the 5 specific Plays, goals were kept to $4K.  
• In addition, Louse wanted data run on GB Musicals shown in the last chart. Again we see a high success rate when Goals were kept modest of below $2K with $10K being an outlier.   
 
## Supporting Data and Graphs
See PDF File  "An Analysis of Kickstarter Campaigns" or the individual graphs in this Repository. 
