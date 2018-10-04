# Boston-Seattle-Airbnb-Analysis
Boston Seattle Airbnb Analysis for udacity project

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>
The code in this project is written in Python 3.6.6 :: Anaconda custom (64-bit).
The following additional libraries have been used:
- wordcloud to generate wordclouds from the text of the reviews
- langdetect to detect the languages of the review
- nltk for the Vader Sentiment Analyzer. The Vader lexicon has been downloaded nltk.downloader.download('vader_lexicon')

## Project Motivation<a name="motivation"></a>
In this project we analyze data from Airbnb listings for Seattle and Boston in 2016 and 2017. The methodology followed is CRISP-DM.
The questions we are trying to answer in this project are the following:
- Which features in the listings affect the price the most? which ones are more important in driving the price up?
- How does the rates between the two cities compare? Can we spot patterns in the seasonal or weekly data?
- Can we find a way to classify negative and positive reviews based on text?

The data has been made available by Airbnb inside, and the original source can be found [here](http://insideairbnb.com/get-the-data.html)

## File Descriptions <a name="files"></a>
The Jupyter notebooks included in this project are:
- Prices and Trends.ipynb, with the code for comparing rates between the two cities and spot patterns in the seasonal or weekly data
- Reviews Sentiment Analysis.ipynb, with the code to analyze the text reviews
- Price Prediction Analysis.ipynb, the code include a linear regression model to predict price and find what features affect the prices the most

## Results<a name="results"></a>
The following results are showed in the notebooks:
- Which features in the listings affect the price the most? which ones are more important in driving the price up?
  Neighborhoods are the most important predictors (as expected), affecting price between trendy suburbs (+68 usd) to bad ones (-67 usd). Staying in a dorm or sharing a room gives good savings, while choosing a loft comes at a premium. Additional bedrooms and bathrooms will cost you 31 usd and 22 usd respectevely, not as much as expected, but understandable considering these are not hotel rooms but privately rented apartments. The patters are similar for Boston and Seattle. Other predictors like amenities offered in the apartments also influence price, but on a much smaller scale.
- How does the rates between the two cities compare? Can we spot patterns in the seasonal or weekly data?
Boston is basically more expensive than Seattle, as the average price in Seattle is 137 dollars, while the average price in boston is 201 dollars. Prices in both cities are rising from February to August and falling from September to February. Prices in Seattle are at least 30 usd more expensive per day in the busy July and August months. In Boston prices are lower than average from December to June and way above average in September and October.
As for the weekly patterns, Thursdays and Fridays are more expensive compared to the rest of the week in both cities: in Seattle prices are around 143 usd in those dsys compared to an average of 135 on Sun, Mon, Tue and 136 on Wed and Sat. In Boston prices are 203 usd on average on thursdays and fridays compared to an average of 195 on Sun, Mon, Tue and 198 on Wed and Sat.So in the more expensive days in both cities prices are around 7-8 usd more than the less expensive ones.

- Can we find a way to classify negative and positive reviews based on text?
The Sentiment Analyser distributions are quite similar between the two cities. The plots show that only just over 6% of the reviews have a strong positive sentiment (>0.5) and the majority (61%) are in the 0.2 - 0.4 range, and most of the reviews are neutral (93%).
However the negative sentiment is very low as the majority of comments have negativity < 0.1
The compound score shows that 63% of the guests in Boston and more than 88% in Seattle give overall positive reviews.

## Licensing, Authors, Acknowledgements<a name="licensing"></a>
The Vader Sentiment Analyzer is due C.J. Hutto and Eric Gilbert fro the paper "VADER: A Parsimonious Rule-based Model for Sentiment 
Analysis of Social Media Text", available [here](http://comp.social.gatech.edu/papers/icwsm14.vader.hutto.pdf)

Langdetect is a port of Google’s [language-detection](https://code.google.com/p/language-detection/) library (version from 03/03/2014) to Python.
It supports 55 languages out of the box  

The data is part of Airbnb Inside, license is from the Kaggle pages for [Seattle](https://www.kaggle.com/airbnb/seattle) and [Boston](https://www.kaggle.com/airbnb/boston).

