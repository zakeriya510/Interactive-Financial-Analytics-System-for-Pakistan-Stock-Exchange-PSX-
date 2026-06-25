https://public.tableau.com/views/PSXDataAnalyticsPotralTableau/PSXProfileDashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
https://public.tableau.com/views/PSXSectorCompanyWisePerformanceRiskAnalysis/StockMarketSectorPerformanceRiskAnalysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
https://public.tableau.com/views/PSXSignalDashboard/SignalsDashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
https://public.tableau.com/views/PriceTrendsReturnsRiskDistribution/StockMarketAnalysisPriceTrendsReturnsRiskDistribution?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link





















Problem Statement:
Currently, thousands of investors operating within the PSX lack access to a fully-fledged investment-centric platform that can provide investment signals and evaluate the performance of a specific stock.  While the data of interest exists in silos and across different platforms and sources that lack an integrated platform that could leverage the power of data that these isolated platforms and sources offer. In a high-stakes, time-critical investment avenue like the PSX, the absence of data-led signals and insights can translate into a windfall profit or plummeting losses that have to be incurred by the investors just due to the lack of a centralized platform. 
The MVP that our team aspired to curate would serve the purpose of arming the investor base with the power of data analytics and enabling it to undertake decisions grounded in historical trends depicted by diverse stocks associated with multiple sectors of the industry. The project aims to intimate the investors regarding the financial health of stocks of interest and render buy or sell signals that could empower the investors to reap maximum profit upon their investments. 
The developed MVP can be deployed and can theoretically be integrated with live data feed and provide live buy, sell signals in addition to evaluating the financial health of the stocks in real-time, thus enabling the investors to rid their dependence off upon different platforms to obtain critical financial information.

















Dataset Description:
The dataset that has been used in our MVP has been sourced from Kaggle, and it encompasses 50 top-performing KSE-100 index heavy stocks in tandem with the 2021-2025 timeframe.  
The dataset has 50.5K rows and 10 columns. 
 
The data type of columns Symbol, Month, and Year are string datatype, the data type of  Date is DateTime, volume, opening, closing, high, low and volume are float datatype.
 
 












Data Preparation:
20 companies from 5 sectors of the dataset were filtered out to obtain a new data frame. 
 

These companies were mapped onto the respective sector, and a new column called sector was obtained.
 
The modified dataset was downloaded and subject to the data visualization process. 
There were no missing values in the dataset.












Dashboard Design Planning:
KPIS:
1.	Total Volumes Traded:
We have utilized this specific KPI to gauge the confidence of investors in the sector, which is usually depicted by the volume of shares traded during a specific timeframe. High volume trading depicts strong confidence of the investor base in the market and vice versa. 
2.	Average Return:
In order to gauge the financial health of the stocks, we created an average return metric KPI as return is one of the sole metrics that an investor factors in before opting for a decision. 
3.	Volatility:
Volatility demonstrates the variance existing between daily returns depicted by each trading day and the associated script and sector. Volatility is actually the measure of risk associated with specific sectors and scripts. 
Layout planning of dashboard:
Each dashboard has been reserved for a specific functionality of the portal. The first dashboard depicts the profile of the 20 companies and associated sectors, while the second dashboard demonstrates sector and script dashboard-wise performance, the third dashboard depicts signals that can be leveraged by investors, while the final dashboard depicts performance analysis.

Price Trend with 7-Day Moving Average
An area chart with a 7-day moving average was selected to visualize the overall trend of stock prices over time. The moving average smooths short-term fluctuations and reduces noise in the data, making long-term upward and downward trends easier to identify. The filled area also improves visual understanding of changes in price magnitude across the selected time period.
Volume Breakdown Per Company
A pie chart was used to represent the proportion of total trading volume contributed by each company in the dataset. This chart helps compare market participation among companies and provides a quick visual understanding of which stocks dominate trading activity in the Pakistan Stock Exchange.





Type of charts selected and reason
Sector-wise Volume Distribution
A treemap chart was selected to display trading volume distribution across sectors and companies. The treemap efficiently represents hierarchical data where rectangle size corresponds to trading volume. This makes it easy to identify sectors and companies with the highest contribution to total market activity.
Sector vs Average Return
A horizontal bar chart was used to compare average returns across different sectors. This visualization clearly highlights positive and negative sector performance and allows easy comparison between industries. The horizontal orientation improves readability when multiple sector categories are displayed together.
Decomposition Tree for Sector and Company Returns
A diverging bar chart was selected to analyze returns at both sector and company levels. Positive and negative bars help distinguish profitable and loss-making stocks, while the grouped structure enables comparison of company performance within each sector. This chart supports detailed performance decomposition and sector-based analysis.
Smoothed Daily Returns (30-Day Trend)
An area chart with a 30-day moving average was used to display smoothed daily returns over time. The moving average minimizes short-term volatility and reveals broader market behavior and momentum trends. This helps in understanding long-term return patterns more effectively.
Closing Stock Price
A line chart was chosen to visualize changes in stock closing prices over time. Line charts are highly suitable for time-series analysis because they clearly show continuity, fluctuations, and long-term price trends. This chart allows easy observation of stock market movements and overall growth patterns.
Volume vs Price Chart
A scatter plot was used to examine the relationship between trading volume and stock prices. Each point represents a stock observation, allowing identification of correlations, clusters, and outliers. This chart is useful for understanding whether heavily traded stocks also exhibit higher prices or unusual market activity.
Signal Chart
A multi-line signal chart was selected to visualize moving average crossover signals used in technical analysis. The chart helps identify bullish and bearish trends by comparing short-term and long-term moving averages. It is useful for detecting potential buy and sell signals in stock trading analysis.
Return Curve Chart
A line chart was used to display daily stock returns over time. This chart highlights sudden rises and falls in returns, making it useful for observing market shocks, price corrections, and return volatility. Different return categories also help classify market behavior more effectively.
Rolling Volatility Graph
A rolling volatility line chart was selected to monitor changes in market volatility over time. Rolling volatility measures fluctuations in returns within a moving time window, helping identify stable and unstable periods in the stock market. This chart is important for risk analysis and volatility forecasting.
Return vs Risk
A bubble chart was used to compare stock returns with associated risk levels. The horizontal axis represents average return, while the vertical axis represents risk measured using standard deviation. Bubble size reflects trading volume, allowing simultaneous analysis of return, risk, and market activity for different stocks.
Return Distribution by Stock
A box plot was selected to analyze the distribution of daily returns for each stock. Box plots effectively summarize median values, quartiles, spread, and outliers, making them useful for comparing variability and consistency among different stocks in the dataset.
Distribution of Daily Returns
A histogram was used to visualize the frequency distribution of daily stock returns. This chart helps identify the concentration of positive and negative returns, overall distribution shape, skewness, and the occurrence of extreme return values. It is useful for understanding market behavior statistically.
Volume vs Date
A time-series line chart was selected to analyze trading volume changes over time. The chart highlights trends, spikes, and unusual fluctuations in trading activity. It helps identify periods of high investor participation and increased market movement within the PSX dataset.









Visualizations Created:
 
PSX Profile Dashboard Explanation
The PSX Profile Dashboard provides an interactive overview of stock market activity in the Pakistan Stock Exchange (PSX). It combines multiple visualizations to analyze stock prices, trading volume, sector contribution, and company performance in a single interface. Filters for Sector and Symbol allow users to dynamically explore specific industries and companies.
The Time-series based opening price line chart shows how stock opening prices changed over time, helping identify overall market trends and price movements. The Volume Breakdown-Per Company pie chart displays the proportion of total trading volume contributed by each company, making it easy to identify heavily traded stocks.
The Treemap visualization represents trading volume by sector and company, where larger blocks indicate higher market activity. Similarly, the Pie Chart Volume summarizes sector-wise trading volume distribution, allowing quick comparison of major industries in the market.
The Volume vs Date line chart tracks changes in trading volume over time and helps identify spikes in market activity and periods of increased investor participation.
Overall, the dashboard provides a compact and interactive way to monitor PSX market behavior, compare sector performance, and analyze trading trends efficiently.







 
Stock Market Sector Performance & Risk Analysis Dashboard
The Stock Market Sector Performance & Risk Analysis Dashboard provides an interactive overview of sector-wise stock market performance in the Pakistan Stock Exchange (PSX). It combines multiple visualizations to analyze returns, trading activity, and investment risk across different sectors.
The Monthly Sector Performance (Average Returns) line chart shows how sector returns change over different months, helping identify performance trends and seasonal variations. The Volume vs Price Chart scatter plot analyzes the relationship between trading volume and stock prices, making it easier to detect highly traded and high-priced stocks.
The Sector Wise Return bar chart compares average returns across sectors and highlights industries with positive or negative performance. The Return vs Risk bubble chart evaluates stocks based on return and volatility, while bubble size represents trading volume, helping users analyze the balance between profitability and investment risk.
Overall, the dashboard helps users compare sector performance, study market behavior, and evaluate risk-return patterns in an efficient and interactive way.








 
Signals Dashboard
The Signals Dashboard was developed to analyze stock market trends, volatility, and trading signals in the Pakistan Stock Exchange (PSX). It combines technical analysis visualizations into a single interactive dashboard to help users understand market movements and identify possible trading opportunities.
The Signal Chart visualizes moving average crossover signals such as Golden Cross and Death Cross, along with bullish and bearish market trends. This chart helps identify potential buy and sell signals based on changes in price momentum over time.
The Rolling Volatility Graph displays changes in market volatility over different time periods. It highlights stable and unstable market conditions and helps identify periods of high uncertainty or sudden price fluctuations in the market.
The Return Curve Chart shows daily stock returns over time and classifies movements into normal behavior, sharp rises, and sharp falls. This visualization helps users analyze return patterns, sudden market changes, and periods of extreme price movement.
Overall, the dashboard provides a compact and interactive way to monitor technical indicators, market volatility, and return behavior for financial analysis and investment decision-making.








 
Stock Market Analysis: Price Trends, Returns & Risk Distribution Dashboard
The Stock Market Analysis: Price Trends, Returns & Risk Distribution Dashboard was designed to provide an overview of stock price behavior, return patterns, and risk distribution in the Pakistan Stock Exchange (PSX). The dashboard combines multiple visualizations to help analyze market trends, return consistency, and volatility in an interactive way.
The Smoothed Daily Returns (30-Day Trend) area chart displays moving average returns over time, helping reduce short-term fluctuations and highlight long-term market trends. The Price Trend with 7-Day Moving Average chart visualizes stock price movement while smoothing daily noise, making overall price direction easier to understand.
The Return Distribution by Stock box plot compares the spread and variability of returns for different companies. It helps identify outliers, consistency, and stocks with higher volatility. The Distribution of Daily Returns histogram shows the frequency distribution of positive and negative returns, helping analyze return concentration, market behavior, and the occurrence of extreme returns.
Overall, the dashboard provides a concise and interactive analysis of stock price trends, return behavior, and market risk, supporting financial analysis and investment evaluation.







Calculated Fields / Measures
List of calculated fields or DAX measures created
Average Return
The Average Return calculated field was created using AVG([Return]). Its purpose is to calculate the mean return of stocks over a selected period. This measure helps evaluate the overall performance of a stock, company, or sector and is widely used in return comparison analysis.
 
Correlation Daily Return
The Correlation Daily Return field was calculated using ([Close] - [Open]) / [Open]. This formula measures the percentage change between opening and closing prices for a trading day. It is used to analyze day-to-day stock price movement and market behavior.
 
Correlation
The Correlation measure was created using CORR([Volume], [Correlation Daily Return]). Its purpose is to determine the relationship between trading volume and daily stock returns. This helps identify whether higher trading activity is associated with stronger price movement.
 
Cross Over
The Cross Over calculation uses moving average comparisons with WINDOW_AVG() and LOOKUP() functions. It identifies technical trading signals such as Golden Cross and Death Cross by comparing short-term and long-term moving averages. This field is used for trend reversal detection and technical analysis.
 
Cumulative Return
The Cumulative Return field was created using EXP(RUNNING_SUM(LOG(1 + SUM([Return])))) - 1. Its purpose is to calculate compounded investment returns over time. This measure helps analyze total portfolio or stock growth across a selected period.
 
Cumulative Growth
The Cumulative Growth measure was calculated using EXP([Cumulative Return]). It converts cumulative returns into a growth representation, helping visualize long-term investment growth and market expansion.
 
Daily Return
The Daily Return field was created using (AVG([Close]) - LOOKUP(AVG([Close]), -1)) / LOOKUP(AVG([Close]), -1). This formula calculates the percentage change in stock closing price compared to the previous day. It is mainly used for return analysis, volatility measurement, and trend evaluation.
 
MA 7-D Return
The MA 7-D Return calculation uses WINDOW_AVG(SUM([Close]), -6, 0). Its purpose is to compute the 7-day moving average of stock prices. This smooths short-term fluctuations and helps identify short-term market trends.
 
Moving Average 30 Days
The Moving Average 30 Days field was calculated using WINDOW_AVG(AVG([Return]), -29, 0). It calculates the average return over the previous 30 days and is used to analyze long-term market behavior while reducing daily noise.
 
Moving Average 7 Days
The Moving Average 7 Days measure was created using WINDOW_AVG(SUM([Close]), -6, 0). This calculation smooths stock price movement over a weekly period and helps visualize short-term price trends more clearly.
 
Price Moving 7 Days Average
The Price Moving 7 Days Average field was created using WINDOW_AVG(AVG([Close]), -6, 0). Its purpose is to generate a smoothed trend line of stock prices over seven days, making it easier to observe market direction and price movement patterns.
Moving Average 30 Days (Price)
The Moving Average 30 Days (Price) calculation uses WINDOW_AVG(AVG([Close]), -29, 0). It calculates the long-term moving average of stock prices and helps identify broader market trends and price direction.
 
Rolling Volatility 10 D
The Rolling Volatility 10 D measure was created using WINDOW_STDEV([Daily Return], -10, 0). This field calculates rolling standard deviation over a 10-day window and is used to measure short-term market volatility and investment risk.
 
Sharpe Ratio
The Sharpe Ratio calculation uses AVG([Return]) / STDEV([Return]). Its purpose is to measure risk-adjusted return by comparing returns with volatility. It helps evaluate how efficiently a stock generates return relative to its risk.
 
Trend Signal
The Trend Signal field was created using a conditional comparison between short-term and long-term moving averages. If the 7-day moving average is greater than the 30-day moving average, the signal becomes Bullish; otherwise, it becomes Bearish. This measure is used for market trend identification and trading signal generation.
 
Volatility
The Volatility measure was calculated using STDEV([Return]). It measures the variability of stock returns over time and is used as an indicator of market uncertainty and investment risk.

 

Insights from Dashboard:
•	Oil & Gas sector depicts a large market share in terms of volume of shares traded.
•	Fauji Cement has depicted maximum shares traded company wise segregation. 
•	Maximum volume of shares traded was depicted on 30th-December 2021.
•	Fertilizer sector depicted maximum returns.


