# CMSE-202-Project
Project: Finance and Economics 3 

Question: 3.  What factors have the most impact on the stock prices of supermarkets and their sales?

Group 14

Member Names:

1. Megha Chaudhari
2. Paige Tourangeau
3. Long Nguyen
4. Andrew Chisholm


Contributions of each member:

Megha Chaudhari: Worked on the unemployment rates code and the general compilation of the notebook. Worked on the abstract and added it to the README file. Helped create the presentation. 

Paige: Worked on the fuel prices code and helped get the data set. Helped create the presentation 

Long: Worked on the CPI and general stock market coding. Helped with creating the presentation. 

Andrew: Worked on the CPI a little and helped change the question.



### Abstract

Goal:
In this project, the main question we sought to answer was: What factors have the most impact on the stock prices of supermarkets and their sales? 
On a deeper level, this involved examining the features stored in our dataset and their relationship to both stock prices and store sales. 

Methodology:
We employed various methods throughout our project to address the research question. Initially, we acquired two datasets from Kaggle: one encompassing sales, fuel prices, local employment rates, CPI, and more for forty-five Walmart stores; the other containing weekly high and low stock prices, along with opening, closing, adjusted closing prices, and volume. After merging and filtering the datasets to focus on the 2010-2013 timeframe, we conducted detailed analyses on each variable, employing a range of techniques.

CPI:
Consumer Price Index (CPI) is a measure of the average change overtime in the prices paid by consumers. For this parameter, 4 separate line graphs were produced to visualize the comparison between CPI against, Opening, Closing, High and Low stock prices. The graph is also formatted in a way to host two axes, where the left side of the Y-axis shows CPI and the right side would display the Opening, Closing, High, and Low prices. This was done this way in order to make visible and easy to read graphs that would help with analysis. The correlation coefficient was found through using a code function called ‘.corr’. Essentially, through specifying the data frame and indexing the variables from the merged data frame, the correlation coefficient can be calculated between CPI and the different stock prices.

Unemployment Rates:
We examined the relationship between average unemployment rates and stock prices, including Open, Close, High, and Low. Graphing unemployment rates against Open and Close revealed an inverse relationship, with an R^2 value of approximately 0.5 for both, indicating moderate correlation. The correlation between unemployment and High, Low, Open, and Close hovered around -0.219, indicating a low negative correlation. Similarly, the correlation between unemployment and Weekly Sales was approximately -0.0265, suggesting an even weaker negative correlation. These findings were derived using the .corr() function and LinearRegression and OLS regression models.

Fuel Price:
Another feature we chose to analyze was the average weekly fuel price for each time period vs. the opening and closing stock price as well as against the average weekly sales amount for 2010-2013. Scatter plots demonstrating the relationship were created using the pandas library and the correlation coefficient was calculated using the .corr() function also in the pandas library. The correlation coefficient for fuel price vs. opening stock price was 0.356, while the same value for fuel price vs. closing price was 0.352. The relationships have a similar strength between them, although it looks to be low from examining the correlation values of each of them. Lastly, the correlation value for fuel prices vs. weekly sales was calculated to be -0.057. Of course, this is an extremely low value and shows that there is basically no correlation between the variables. 

Conclusion:
The final results of our project showed that there was a very low correlation between average fuel price and stock prices as well as an even lower correlation value between average fuel price and average weekly sales. These results tell us that fuel price is not an accurate predictor of either stock price or store sales. The results for unemployment rates were also the same. Both had a really low correlation the only major difference was the unemployment rate had only a negative correlation. Most significantly, we did find a relationship between the CPI feature and the different stock prices. Through deeper analysis and the use of  ‘.corr’ to derive the correlation coefficient, all the results came out to be higher than 0.86, where CPI with 'Open' at 0.8666361035581457, CPI with 'Close' at 0.8682166699472663, CPI with 'High' at 0.8681510050491542, and CPI with 'Low' at 0.8673277775293707. These values suggest that there is a very strong correlation between CPI and the stock prices, which tells us that CPI is a strong indicator of stock prices. And also the best indicator out of all the features we chose to examine in this project. 