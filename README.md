# Analysis of the discourse around ChatGPT in Twitter
This repository contains code for extraction of tweets from Twitter's API and enables interaction with ChatGPT3.5 through OpenAI's API.

In order to study the discourse around ChatGPT in Twitter, we used Twitter's API to retrieve recent tweets discussing the use of ChatGPT.
In addition, we connect to OpenAI's API to send prompts and questions to the chatbot and record its answers.
Using these sources, we created a dataset consisting of ~240K tweets, collected between February and June 2023 according to our inclusion criteria based on pre-defined keywords.
All personal identifiers in the dataset, such ```author_id``` and ```tweet_id``` are anonymized.

Several analyses were performed on the collected tweets:
- Sentiment analysis - each tweet was classified to either positive, negative or nuetral sentiment using the [BERTweet model](https://huggingface.co/finiteautomata/bertweet-base-sentiment-analysis) (a RoBERTa model trained on English tweets).
- Emotion analysis - each tweet was classfied to one of 7 emotions (anger, disgust, fear, joy, neutral, sadness and surprise) using the [RoBERTa-large model](https://huggingface.co/j-hartmann/emotion-english-distilroberta-base).
- Topic assignment - each tweet was assigned to one topic by ChatGPT, based on represntative set of topics, extracted based on a sample of tweets from our corpus.

Currently, the collection of data is done manually using the provided notebooks:
- [ ] _[To upload] ```retrieve_tweets.ipynb```: Extract all tweets from the last 7 days using Twitter's basic API, according to given keywords. Twitter's ```v2``` API is used._
- [x] ```extract_img_from_twitter.ipynb```: Extract images from URLs included in tweets and read their texts.
- [ ] _[To upload] ```interact_with_chatgpt.ipynb```: Send pre-defined prompts to ChatGPT3.5 through OpenAI's API and record its answers._

## Usage:
- Install ```Python```  (3.7 or later versions) with Jupyter (or Jupyter-lab interface).
- Create a virtual environment (or laternatively Anaconda environment) and install the following packages: ```numpy```, ```pandas```, ```seaborn```, ```jupyter```, ```nltk```, ```tweepy```, ```spacy```, ```gensim```, ```pyenchant```, ```beautifulsoup4```.
- Run the above notebooks.
