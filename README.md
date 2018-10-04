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

- How does the rates between the two cities compare? Can we spot patterns in the seasonal or weekly data?

- Can we find a way to classify negative and positive reviews based on text?


## Licensing, Authors, Acknowledgements<a name="licensing"></a>
The Vader Sentiment Analyzer is due C.J. Hutto and Eric Gilbert fro the paper "VADER: A Parsimonious Rule-based Model for Sentiment 
Analysis of Social Media Text", available [here](http://comp.social.gatech.edu/papers/icwsm14.vader.hutto.pdf)

Langdetect is a port of Google’s [language-detection](https://code.google.com/p/language-detection/) library (version from 03/03/2014) to Python.
It supports 55 languages out of the box  

The data is part of Airbnb Inside, license is from the Kaggle pages for [Seattle](https://www.kaggle.com/airbnb/seattle) and [Boston](https://www.kaggle.com/airbnb/boston).

