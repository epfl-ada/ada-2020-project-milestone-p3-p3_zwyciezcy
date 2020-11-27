## Title:
Testing BFS sampling approach as a generation method of representative samples

## Abstract: 
The authors of the paper claim that the BFS sampling approach could not generate representative samples. Our aim is to verify this thesis. Hence, we are going construct a new dataset, then validate its representativeness using Kolmogorov-Smirnov test as the authors in the paper, and finally repeat some investigations made by the Hai L. et al. In order to generate the dataset we will randomly generate some Twitter IDs and check if there exists a corresponding Twitter user. Then we will use those egos as sources to launch BFSs. The nodes of a search graph are Twitter users while edges are both follower and followee relationships. We will generate a dataset which size will be approximately equal to the one used by the authors of the paper. Finally, using new dataset we will repeat verifications of some prepositions. 

## Research questions
1. Is the BFS sampling approach representative based on Kolmogorov-Smirnov test?
2. How many sources we need to to generate a representative dataset?
3. Are the authors' prepositions agree with the conclusions drew from our dataset?

## Proposed datasets
- Dataset generated in a way described below

## Methods
- **Dataset generation** We will try different number of sources (100-1000) for BFS and choose the best dataset using Kolmogorov-Smirnov test. To download the data we will use Twitter API

- **Verification of prepositions** We have decided to focus on one preposition from each section, i.e. "Circadian rhythms" (usage), "Dunbar’s number" (structure), and "Influential hypothesis" (information diffusion).

## Proposed timeline
- **Week 1:** Dataset generation
- **Week 2:** Verification of chosen prepositions
- **Week 3:** Prepare report and a short video

## Organisation within the team:
- Viktor will find out how to get an access to Twitter API
- Maciek will write BFS and the setup for fetching data using Twitter API
- Maciek will clean the data and verify two prepositions (usage and structure)
- Viktor will verify the third preposition (information diffusion)
- Maciek will organise and clean the code, and work on making a data story notebook
- Viktor will prepare video



1.	Title: Testing exposure hypothesis for exposure to Tweets on global warming
2.	Abstract
The paper explores propositions on a randomly selected dataset. We propose to replicate the results on the exposure hypothesis for exposures to tweets about global warming. To achieve this we will train a NLP algorithm on the Kaggle “Twitter Climate Change Sentiment Dataset“. The goal is to classify Tweets about global warming in the following categories: i) (News) the Tweet is news ii) (Pro) the Tweet supports the belief of man-made climate change iii) (Neutral) the tweet neither supports nor refutes the belief of man-made climate change, iv) (Anti) the tweet does not believe in man-made climate change. This model will then be applied to new Tweets to label them. The Twitter API will be used to build a dataset of users selected on the basis of whether some words related to climate change appear in their Tweets. The followers and followee of these accounts will be added to the dataset along with their Tweets and the other required information. The method used to build this dataset will be to generate random user ids and test if they exist. Only users who’s language is English will be retained.

3.	Research questions
1. What is the probability of retweeting Tweets about global warming as a function of the number of exposures to Tweets about global warming? How do the results change for exposure to Tweets about global warming with the label Pro, Neutral or Anti ? How do the results change for probability of retweeting Tweets with the labels Pro, Neutral or Anti ?
2. Think about a meaningful way to describe the time evolution of user’s Tweet labels. And look for people who changed their mind about global warming.
4.	Proposed datasets
o	Testing Propositions Derived from Twitter Studies dataset from the paper for comparing our results (if replicating figure 6 is too time consuming we could skip this part and use a screenshot for comparing results).
o	Build a dataset of users Tweeting about the environment using the Twitter API (think about how much time this will take if we use randomly generated Twitter ids, if it takes too long we could employ a BFS algorithm but then the dataset would not allow generalizability)
o	Twitter Climate Change Sentiment Dataset from Kaggle, https://www.kaggle.com/edqian/twitter-climate-change-sentiment-dataset
5.	Methods

NLP sentiment analysis model: We will do research on what model would perform well on classifying Tweets. We will consider random tree, and SVM as well as other models found in literature.
Data collection: We have signed up to the Twitter API to build a dataset including the number of followees, the number of followers, a list of Tweets including words like “climate change” in some time window (up to 10 years if this is possible), a list of the dates of those Tweets, probability of retweeting Tweets with each of the labels. An obstacle to building this dataset might be the number of requests that can be made through the Twitter API (up to 3200 requests / hour).
Data analysis: We are interested on how exposure to Tweets of the 4 different categories (New, Pro, Neutral, Anti) influence users to Retweet or Tweet messages of different categories. We might be able to do dimensionality reduction to isolate important effects.
Time series analysis: The labels of a user’s Tweets in time define a time series. We could imagine keeping only the labels corresponding to the categories Pro and Anti and fitting a linear model. We will refer to this time series as the “opinion time series”. The slope thus obtained would be a good proxy for change of opinion. We could then study what causes users to change their opinions. Is it the characteristics of the cluster they are part of? Or is it their individual properties that cause them to change their mind? We will have to think about how we can infer causality instead of just correlation.

We realize that this project proposal is full of wild ideas. We are prepared to find out that the data does not allow to realize some of these ideas. We will clarify what we do as we explore the data.

6.	Proposed timeline
Week 1: One of us will build the dataset and the other will train the NLP model.
Week 2: We will work together on plotting the probability of Tweet/Retweet of a certain category as a function to exposure to difference categories of Tweet.
Week 3: Explore interesting data analysis opportunities, preparing the data story and short video.
7.	
8.	Organization within the team
o	Viktor will work on building the dataset using the Twitter API and Maciek will train a NLP model for the classification task using the Kaggle dataset
o	Viktor will work on making plots similar to figure 6 in the paper and Maciek will explore the possibilities of data analysis using the opinion time series
o	Viktor will work on making the video while Maciek will work on making a data story notebook

