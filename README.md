## Title:
Tweet_analysis: Do positive people cluster together?

## Abstract: 
The authors of the paper claim that the BFS sampling approach could not generate representative samples. Our aim is to verify this assertion. Hence, we are going construct a new dataset, then validate its representativeness using Kolmogorov-Smirnov test as the authors in the paper, and finally repeat some investigations made by the Hai L. et al. In order to generate the dataset we will randomly generate some Twitter IDs and check if there exists a corresponding Twitter user. Then we will use those egos as sources to launch BFSs. The nodes of a search graph are Twitter users while edges are both follower and followee relationships. We will generate a dataset which size will be approximately equal to the one used by the authors of the paper. Finally, using new dataset we will repeat verifications of some prepositions. 

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