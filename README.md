# Stock-Trend-Analysis
GameStop vs Tesla Stock Analysis : Analyzed short selling using Tesla and GameStop as Case studies. Extracted and visualized stock price and hedge fund profit data,building dashboard to compare performance and highlight the risks and outcomes of short positions.

# Objective
To Analyze the impact of short selling on Tesla and GameStop by extracting and visualizing stock price and hedge fund profit data and develop a dashboard that compares market performance with hedge fund outcomes.

# Key Insight
->Highlighted how short selling strategies can backfire when stock prices rise unexpectedly
-> Demostrated the contrast between Tesla's growth-driven rise and GameStop's Demand-driven surge
-> Built an interactive dashboard to compare stock price movements with hedge fund profit trends.
-> Provided insights into market behaviour,risk and investment strategies

# Introduction
Short Selling has played a significant role in recent stock market events, particularly with Tesla and GameStop. This project explores how hedge funds were impacted, highlightling both the risks and opportunities of short position

# Data
-> Sources : Stock Price Data (Tesla and GameStop), hedge fund profit/loss data
-> Format : python yfinance library ,  https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/revenue.htm , https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/stock.html 

# METHODS
-> General
1. I installed the relevant python library for the analysis using the pip install method which include yfinance , bs4 , nbformat , plotly
2. I imported the relevant modules which are yfinance, pandas, BeautifulSoup, plotly , make_subplot
3. I also imported the warning module to ignore all warnings
4. The function make_graph was also defined
-> Using the python yfinace library
5. I used the Ticker method from the yfinance to create a ticker object for the Tesla stock which is represented as **TSLA**
6. The ticker object and the function library history and setting the period to max to dsiplay the data in a dataFrame
7. I used the head function to dsiplayed the first five rows
8. Step 5-7 was repeated for GameStop. The symbol for GameStop in the yfinance library is **GME**
-> Using Web Scrapping
9. I used the request library to download the web page for the Tesla Stock data using the url :  https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/revenue.htm
10. I used beautifulSoup to parse the html data
11. The parsed data was stored in a DataFrame extracting only the **Quarterly revenue data**.
12. I used python basic lines of code to remove all commas , dollar sign and empty string from the revenue data
13. I displayed the last five(5) rows using the tail function
14. I repeated steps 9 - 13 for the GameStop Quarterly revenue data Using the url :  https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/stock.html

# Dashbord 
The interactive dashboard allows users to :
1. Compare Tesla and GameStop stock price Trends
2. Visualize hedge funds profit/loss over time
3. Explore relationship between stock movements and hedge fund performance

# Results
-> Clear Correlation between hedge fund losses and rapid stock price increases.
-> Tesla : Steady long-term growth affecting hedge fund short positions.
-> GameStop : Rapid short squeeze leading to massive losses for hedge funds.
