# CognitiveServicesDemos
Azure Cognitive Services Demos

## About the Demo:

Cognitive Services Text Analytics API with Opinion Mining (Preview) using Power BI Desktop.

Useful Links:

https://docs.microsoft.com/en-us/azure/cognitive-services/language-service/sentiment-opinion-mining/overview

## Dataset Name:

OpinRank

### Dataset Source: 

https://archive.ics.uci.edu/ml/machine-learning-databases/00205/

### Data Set Information:

Car Reviews
------------

-Full reviews of cars for model-years 2007, 2008, and 2009
-There are about 140-250 cars for each model year
-Extracted fields include dates, author names, favourites and the full textual review
-Total number of reviews: ~42,230

Hotel Reviews 
--------------

-Full reviews of hotels in 10 different cities (Dubai, Beijing, London, New York City, New Delhi, San Francisco, Shanghai, Montreal, Las Vegas, Chicago)
-There are about 80-700 hotels in each city
-Extracted fields include date, review title and the full review
-Total number of reviews: ~259,000

Note: This demo uses the Hotel Reviews data. 

## Setting up the demo:

Provision Language service in Azure and get the endpoint/key information.
Download and unzip the dataset.
Download the PowerBI dashboard file and open it using Power BI Desktop.
Click Home -> Transform Data -> Edit Parameters
Set the parameters

1) Hotels Folder Path - Local path of 'hotels' directory after unzipping the dataset.
2) Language Endpoint - Endpoint for Language Cognitive Resource from Azure Portal.
3) API Key - API Key for Language Cognitive Resource from Azure Portal.
4) Reviews to Analyse - Limit the reviews and API calls. Do not set this value too high.

Note: This demo uses Text Sentiment Analysis with Opinion Mining (Preview) and requires you to use specific endpoint. Refer the example below.

https://<your_endpoint>.cognitiveservices.azure.com/text/analytics/v3.1/sentiment?opinionMining=true&model-version=2021-10-01-preview