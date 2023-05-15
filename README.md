# tweets-chatgpt-extractor
This repository contains code for extraction of tweets from Twitter's API and enables interaction with ChatGPT3.5 through an OpenAI's API.

In order to study the discourse around ChatGPT in Twitter, we use Twitter's API to retrieve recent tweets discussing the use of ChatGPT.
In addition, we connect to OpenAI's API to send prompts and questions to the chatbot and record its answers.

Currently, the collection of data is done manually using the provided notebooks:
- retreive_tweets.ipynb: Extract all tweets from the last 7 days using Twitter's API, according to given keywords. Twitter's APIv2 is used.
- extract_img_from_twitter.ipynb: Extract images from URLs included in tweets and read its texts.
- interact_with_chatgpt.ipynb: Send pre-defined prompts to ChatGPT3.5 through OpenAI's API and record its answers.
