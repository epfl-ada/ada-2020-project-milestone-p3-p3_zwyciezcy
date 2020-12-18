## Title:
Tweet_analysis: Do positive people cluster together?

## Abstract: 
It is said that positive people attract each other. In this project we will investigate this claim using the data set from ref. We will try to understand how positive or negative people cluster together as well as see if a change in the sentiment of a user is correlated to a change of sentiment of his followers and followee. We will look at how the average sentiment of tweets change with the seasons across a year.

## Research questions
1. How to define people's positiveness?
2. How the the sentiment of a tweet reflects to its readers?
3. Do people who usually post tweets with positive sentiment are followed by (or follows) people who also usually post tweets with positive sentiment.

## Proposed datasets
- Data set given in a paper by Liang H. et al.
- Sentiment140

## Methods
- **Fetching tweet texts** We are going to use Twitter API to download the particular tweets

- **Model for sentiment** We have decided to train a simple learning model, e.g. SVM on Sentiment140 data set.

## Proposed timeline
- **Week 1:** Fetching tweets and model training
- **Week 2:** Analysing clusters
- **Week 3:** Prepare report and a short video

## Organisation within the team (what has been done):
**Viktor:**
- training a SVM model for sentiment analysis 
- training a fasttext model for sentiment analysis
- plotting the 2 figure: number of tweet per month and number of tweet per hour on each day of the week
- obtaining a key for the twitter API
- writing the introduction section of the report

**Maciek:**
- going through Twitter API tutorial
- establishing connection with Twitter's server
- trying to fetching tweets' text
- writing second and third section of report
- updating READ.me  