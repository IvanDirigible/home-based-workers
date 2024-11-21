# home-based-workers
**Sources used **
U.S. Census Bureau. Data. U.S. Census Bureau, https://www.census.gov/data.html.
U.S. Census Bureau. American Community Survey. U.S. Census Bureau, https://www.census.gov/programs-surveys/acs.
OpenAI. *ChatGPT*. Version 4, OpenAI, 2024, https://openai.com/chatgpt. Accessed 17 Nov. 2024.
Used ChatGPT to help code create loop in order to grab work-at-home and median household income. ChatGPT also helped converted the data frame to numeric for easy to read format. 
OpenAI. *ChatGPT*. Version 4, OpenAI, 2024, https://openai.com/chatgpt. Accessed 19 Nov. 2024.
Used ChatGPT to help plot a scatter chart as I was having issues with the bar chart. The code used plt.annotate to add the state names to the scatter plot which I thought was helpful. 

*** Presentation Notes ***
Q: How does the percentage of remote workers relate to the median household income across different states in 2022?

Analysis: 

We pulled data from the census library (ACS 5-Year Estimates) and specifically looked at the variables `B08301_021E` containing work at home data and `B19013_001E` median household income. 

*** Websites to data ***
B08301: Means of Transportation ... - Census Bureau Table (Work at home data)
B19013: Median Household Income in ... - Census Bureau Table (Median household income)
*** The US median estimate was 74,755.00 - note to self ***
*** Work from home estimate for 2022 was 24,381,732.00 - note to self ***

Cleaning the data we converted median income and work-at-home data to numeric as some columns contain non-numeric values, those values are converted to NaN which is easier to use.  Assign state names to a separate column, Drop the 'NAME' column, then Append the data for the year to the all_data list.

We then created a scatter plot for a visual analysis in order to cross reference these two data sets. The result shows the percentage of the population in each state who completed the census working from home and the median income within those states. 

Note: We know that the median income by state is not solely linked to the income of home-based workers. But that doesn’t mean that home-based workers do not contribute to the median household income. 

Conclusion: Looking at the chart, there is a possibility that the annual gross income is less for remote workers residing in the states with less work-at-home percentage vs a state with a higher work-at-home percentage. And with that we can possibly conclude that states with higher median income may offer more remote jobs vs states with lower median income as they may have more resources and wealth to offer remote positions. 



