# Twitter-Scrapping-and-Sentiment-Analysis

This project demonstrates how to scrape tweets from a specific user's Twitter account using the Nitter library and perform sentiment analysis on the scraped tweets using the NLTK library's VADER sentiment analyzer.

## Dependancies

- ntscraper: A Python library for scraping tweets from Twitter.
- nltk: A Python library for natural language processing.

## Scrapping

To scrape tweets from a specific user's Twitter account, we use the Nitter library. First, we import the necessary libraries and create a Nitter scrapper object. Then, we use the `get_tweets` method of the scrapper object to scrape the tweets. The method takes three arguments: the username of the Twitter account to scrape, the mode ('user' or 'search'), and the number of tweets to scrape.

```python
scrapper = Nitter()

tweets = scrapper.get_tweets('imVkohli', mode= 'user', number = 1000)
