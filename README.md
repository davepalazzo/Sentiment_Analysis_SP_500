
**Summary** - This repository explores the relationship between the sentiment of annual 10-K filings for the companies that make up the S&P 500 and their predictive capabilities for annual growth rate percentage of U.S. gross domestic product. Refer to the notebook Economic_Forecasting. 

[Final_Report](https://mybinder.org/v2/gh/davepalazzo/Sentiment_Analysis_SP_500/master?filepath=Sentiment_Analysis_Project%2FEconomic_Forecasting.ipynb)

**Motivation** - Economic indicators, particularly recessions are notoriously difficult to predict. Of the 469 downturns since 1988, the International Monetary Fund (IMF) had correctly predicted four by the spring of the preceding year.
https://www.fathom-consulting.com/the-economist-who-cried-wolf/

Our goal is to use sentiment analysis on the 10-K fillings of companies in the S&P500 for modeling fluctuations in US annual GDP to better predict economic volatility.

**Libraries** - The code in this repository is written in Python, utilizing the following libraries:
   -      Numpy
   -      Pandas
   -      Edgar – used to scrape the SEC website for 10-k documents
   -      Genism
   -      Sklearn
   -      TextBlob

**Data Collection** - We will scrape the SEC website for 10-K fillings of companies in the S&P500 utilizing the Edgar package in python to facilitate this process. Refer to the following notebook for the code used in to gather our data. 

[Data Gathering](https://mybinder.org/v2/gh/davepalazzo/Sentiment_Analysis_SP_500/master?filepath=Sentiment_Analysis_Project/scrape_top10_MDA.ipynb)

**Literature Review** - Through our review of academic papers we found several using sentiment analysis on various corpora to predict stock prices and company metrics, however, we were unable to find papers linking sentiment of public company filings to economic factors such as GDP. Refer to the following papers, which inspired the project:
 
   -  Lazy Prices, Lauren Cohen, Christopher J. Malloy, Quoc Nguyen
   -  Sentiment Analysis of Twitter Data for Predicting Stock Market Movements, Venkata Sasank Pagolu, Kamal Nayan Reddy, Ganapati Panda, Babita Majhi 

**Data Clean Up** - For our analysis, we want to focus on the “Management’s Discussion and Analysis of Financial Condition and Results of Operations” section of the 10-K filings. We will need to look through each 10-K filing and pull out that section. Once we have pulled the section from each companies filings, we will clean the text to then run in our model.

[Data Cleaning](https://mybinder.org/v2/gh/davepalazzo/Sentiment_Analysis_SP_500/master?filepath=Sentiment_Analysis_Project/Clean_MDAtext.ipynb)

**Predictive Task** - We will use Sklearn’s CountVectorizer to tokenize our cleaned text to see if using sentiment analysis we can predict fluctuations in US annual GDP.

**Required Work and Timeline** - We have divided the necessary work into five phases:<br>

1)    Data collection and cleaning – May 3rd<br>
2)    Model Evaluation and Selection -  May 10th<br>
3)    Build a Predictive Model and Evaluate – May 17th<br>
4)    Interpret Model Results and Adjust as necessary – May 24th  


```python

```
