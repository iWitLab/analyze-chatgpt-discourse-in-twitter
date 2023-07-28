# tweets-chatgpt-extractor
This repository contains code for extraction of tweets from Twitter's API and enables interaction with ChatGPT3.5 through OpenAI's API.

In order to study the discourse around ChatGPT in Twitter, we use Twitter's API to retrieve recent tweets discussing the use of ChatGPT.
In addition, we connect to OpenAI's API to send prompts and questions to the chatbot and record its answers.

Currently, the collection of data is done manually using the provided notebooks:
- _[To upload] ```retrieve_tweets.ipynb```: Extract all tweets from the last 7 days using Twitter's basic API, according to given keywords. Twitter's ```v2``` API is used._
- ```extract_img_from_twitter.ipynb```: Extract images from URLs included in tweets and read their texts.
- _[To upload] ```interact_with_chatgpt.ipynb```: Send pre-defined prompts to ChatGPT3.5 through OpenAI's API and record its answers._

## Usage:
- Install ```Python```  (3.7 and later versions) with Jupyter (or Jupyter-lab interface).
- Create a virtual environment (or laternatively Anaconda environment) and install the following packages: ```numpy```, ```pandas```, ```jupyter```, ```nltk```, ```tweepy```, ```spacy```, ```pyenchant```, ```beautifulsoup4```.
- Run the above notebooks.
