# U of T Fin Tech BootCamp Class Unit 4 Assignment #

## Python and Pandas

By: Ivan Kin-Ngai Fung

Date: June 4, 2021

**Objective**

The objective of this assignment was to perform the portfolio analysis using the tools in Pandas.  By using the tools we learned from the class, we were required to perform the portfolio anaylsis including volatilty, risk vs return and Sharpe ratio calculation.
We should use the results from these important metrics to evaluate the performance of the each given portfolio and to select the best performance among 7 different portfolio.  In this assignment, three CSV files to perform our analysis.  These portfolios were analyzed against the market benchmark S&P TSX 60 to determine the performance of each portfolio against the market benchmark.  

In the second part of the assignment, we had to select three additional stocks to be assembled into our own portfolio.  Each stock was assigned to have an equal weight within my own portfolio.  We were then required to run the whole analyis again with our selected stocks' portfolio with the rest of the portfolios in part one of the assignement and to see if our portfolio were able to outperform the other ones in the combined dataframe.  
 


**Results and Discussion**

*Part I - Portfolio Analysis*

Performance Anaylsis

From the results and plot of cumulative returns for all portfolio, we can see that the Algo funds was outperforming the rest of the funds with cumulative returns exceeded over 100% over time from 2015 to 2019.  

Risk Analysis

The box plot was plotted to review the disperison of the rate of return for each portfolio.  The box plot shown that Tiger Global Management LLC has the greatest disperson of daily return among the portfolios in the dataframe while Paulson & Co. Inc has the lowest dispersion of daily return.  
From of the standard deviation calculation, we could see that Berkshire Hathaway Inc was the riskest investment among all of the portfolios while Paulson & Co. Inc. has the least standard deviation for its daily return.  With the S&P TSX60 as the market benchmark, the portfolios which were riskier than the market were Algo 1, Soros Fund Management LLC, Algo 2, Tiger Global Management LLC, and Berkshire Hathaway Inc.

Rolling Statistics

Tiger Global Management LLC and Berkshire Hathaway Inc seemed to be the portfolio with the higher values in 21-Day rolling standard deviation.

Using the corr() function in pandas, we were able to compute the correlation of each portfolio with each portfolio in the dataframe.  We could identify Algo 2 had a correlation of 0.74 which were the highest and close to 1 with the S&P TSX 60.  So, Algo may tried to mimick the S&P TSX 60 with a correlation close to 1.0.

Tiger Global Management LLC was chosen to calculate the 21 rolling beta with the S&P TSX 60, and the results shown that the portfolio had rolling beta values less than when comparing to the market benchmark. It reached the lowest in 2018, and then climbed back up to the level above 1.0 since 2019.

Sharpe Ratios

We had to make an assumption that Risk Free rate were close to zero in the recent low interest environment.   The Sharpe Ratio was computed for each of the portfolio, and the results shown that Algo 1 had the highest ratio among the portfolios in our analysis.  As a result, Algo 1 was far supreme over the rest of the other portfolios in the dataframe.

*Part II - Custom Portfolio*


Three stocks were selected in this part of the assignment.  
1) Royal Bank of Canada (RY.TO)
2) Sucor Energy (SU.TO)
3) Sqaure (SQ)

We assigned equal weight for each of the selected stocks in my own portfolio.  To calculate the overall return of my portfolio, we used the dot() function to cross multipying each stock return with its own weight in the portfolio.  We then concatenated the daily return results of my portfolio with the rest of portfolio in part one of the assignment into one combined dataframe to carry out the portfolio analysis.  

From the risk metric, my portfolio was the riskest among the portfolios in the dataframe with annual standard deviation of 0.2217.  

Morever, the correlation matrix among the portfolios shown that my portfolio had some correlation with Algo 2 and S&P TSX with values of 0.62 and 0.64 respectively.

To further understand the relationship with the market benchmark, we used my portfolio to compute 60 day rolling beta value.  The results shown that the beta was generally higher than one in the time horizon of our study.  The results stayed at the level over 2.0 after 2019.  This might attribute to the explosive growth of Square since 2019.  As a result, the rolling beta remains in such a high level.  

Finally, the Sharpe ratio of each portfolio was computed to compare the overall performance of each portfolio.  The assumption of Risk Free rate was equal to zero was made in our calculation.  The final results revealed that my portfolio was able to outperform the rest of other portfolios with Sharpe ratio 1.3535 which were even better than Algo 1 in our disccusion for part one of the assignment.







 


