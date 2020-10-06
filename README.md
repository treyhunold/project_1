# Predicting Exxon Stock Prices Using VADER Sentiment Analysis

## Background

Built a trading strategy based on the relationship between the energy market and sentiment from new articles from the New York Times. Performed a backtest on the previous two years of Exxon stock with VADER sentiment scores to determine if our analysis would have been a good indicator of the movement of the stock.

## Project Breakdown

### Data Collection

Accessed NYT article database using their API and Python documentation to extract articles with Python code using keywords oil, petroleum,  and energy. Saved article information in JSON format.

### VADER Sentiment Analysis

Looped through JSON data of article snippets. Used the VADER sentiment analyzer from the Natural Language Toolkit (NLTK). This provided sentiment scores of positivity, negativity, or neutral to articles from the previous ten years.

### Random Forest Regression

Performed Random Forest Regression to produce predicted prices of Exxon stock. We used the previous ten years to train the data, and compared it to the previous two years of the stock. 

### Backtesting

Utilized the Backtesting toolkit to use their SmaCross backtesting strategy to use it on the previous two years of Exxon stock and our trained data using sentiment analysis on the previous two years.

### Technologies Used

* Python 
* VADER Sentiment Analysis
* New York Times API
* Natural Language Toolkit
* Backtesting
* Random Forest Regression