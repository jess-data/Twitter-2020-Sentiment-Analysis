# Analyzing Twitter Users' 2020 Reflections using NLP
### A Sentiment Analysis Project using Python and Tableau

This is a Sentiment Analysis Project using Natural Language Processing (NLP) Techniques. In December 2020, I felt it would be a good idea to obtain insights into how Twitter users felt about the year. Twitter receives over 500 million tweets per day from its users across the globe, so I only had to find a way to retrieve the data. This Notebook makes use of several Python libraries like Pandas (for Data Cleaning/Manipulation), Tweepy (for Tweets Mining), NLTK (Natural Language Toolkit), TextBlob (for Sentiment Analysis), MatPlotlib &  WordCloud (for Data Exploration), Emot (for Emojis identification), Plotly (for some Data Visualisation)
In the Jupyter Notebook, you will leearn how I carried out the following steps for the project:

1. Import Libraries
2. Tweets Mining
3. Data Cleaning
4. Location Geocoding
5. Tweets Processing
6. Data Exploration
7. Sentiment Analysis

![alt text](https://github.com/jess-data/Twitter-2020-Sentiment-Analysis/blob/master/7709-01-7-step-horizontal-flow-diagram-for-powerpoint-16x9%20-%20PowerPoint%2028_12_2020%2011_26_38%20PM.png)

Visulizing Outcome
The Plot below was genrated using Plotly Library for Python

![alt text](https://github.com/jess-data/Twitter-2020-Sentiment-Analysis/blob/master/Twitter%20analytics2%20-%20Jupyter%20Notebook%20-%20Google%20Chrome%2026_12_2020%201_09_57%20AM.png)


Some of the insights I generated are stated below:

Tweet Sentiments: I was not surprised by the proportion of the sentiment categories because, for most people, the end of the year is a time to show gratitude and hope for a better year ahead. However, this year has been filled with so many unpalatable events, hence, 31% of the tweets being Negative. *Please note that this is not indicative of the entire Twitter community as only a subset of tweets were mined for this analysis.
Countries with Most Tweets: About 40% of the total tweets emanated from the United States, England and Canada. Since a good number of Twitter users do not have their exact location on their profiles, their tweet locations were classified as "Unknown location".
Hour of the day with the Most Tweets: It was interesting to see that most tweets were created at 5 PM (GMT). Thinking about it, in the US & Canada, this is lunchtime while in countries like Nigeria and England, it is when most individuals finish the work-day, so they have ample time to tweet.
Hour of the day with Least Tweets: 9 AM (GMT) was the hour of the day with the least number of tweets. The reason is this is when most people start their day at work in countries like Nigeria and England while it is still bed-time in other countries like the US & Canada.
Most Retweeted and Liked Tweet: For the period of 12th to 25th December 2020, the tweet with the most retweets was about a Korean boy band: "BTS" and their songs with 10,873 RTs. The most liked tweet from a user who tweeted about how "2020 was a good year for his dog who did not have to be alone for a second". The tweet had 42,295 likes.
