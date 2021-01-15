# Analyzing Twitter Users' 2020 Reflections using NLP
### A Sentiment Analysis Project using Python and Tableau. Click [here](https://jess-analytics.medium.com/) for the full article.

This Project was done using Natural Language Processing (NLP) Techniques. In December 2020, I felt it would be a good idea to obtain insights into how Twitter users felt about the year. Twitter receives over 500 million tweets per day from its users across the globe, so I only had to find a way to retrieve the data. Python libraries like Pandas (for Data Cleaning/Manipulation), Tweepy (for Tweets Mining), NLTK (Natural Language Toolkit), TextBlob (for Sentiment Analysis), MatPlotlib &  WordCloud (for Data Exploration), Emot (for Emojis identification), Plotly (for some Data Visualisation) were used for this project.

In the [Jupyter Notebook](https://github.com/jess-data/Twitter-2020-Sentiment-Analysis/blob/master/Twitter%20Sentiment%20Analysis%20Project.ipynb), you will leearn how I carried out the following steps for the project:

1. Import Libraries
2. Tweets Mining
3. Data Cleaning
4. Location Geocoding
5. Tweets Processing
6. Data Exploration
7. Sentiment Analysis

![alt text](https://github.com/jess-data/Twitter-2020-Sentiment-Analysis/blob/master/Flowchart.png)

## Tweets Processing Steps
To reach the ultimate goal, there was a need to clean up the individual tweets. To make this easy, I created a function "preProcessTweets" in my Python program which I further applied to the "Tweets" to produce the desired results. This user-defined function was used to remove punctuations, links, emojis, and stop words from the tweets in a single run. Additionally, I used a concept known as "Tokenization" in NLP. It is a method of splitting a sentence into smaller units called "tokens" to remove unnecessary elements. Another technique worthy of mention is "Lemmatization". This is a process of returning words to their "base" form. A simple illustration is shown below.

![alt text](https://github.com/jess-data/Twitter-2020-Sentiment-Analysis/blob/master/twitter.jpg)

## Word Cloud Generation
To get the most common words used to describe 2020, I made use of the POS-tag (Parts of Speech tagging) module in the NLTK library. Using the WordCloud library, one can generate a Word Cloud based on word frequency and superimpose these words on any image. In this case, I used the Twitter logo and Matplotlib to display the image. The Word Cloud shows the words with higher frequency in bigger text size while the "not-so" common words are in smaller text sizes.

![alt text](https://github.com/jess-data/Twitter-2020-Sentiment-Analysis/blob/master/wordcloud.png)

## Visulizing Most Common Words
The Plot below was genrated using Plotly Library for Python.

![alt text](https://github.com/jess-data/Twitter-2020-Sentiment-Analysis/blob/master/Twitter%20analytics%20pic.png)

## Sentiment Analysis
For this analysis, I went with TextBlob. Text Blob analyzes sentences by giving each tweet a Subjectivity and Polarity score. 
Based on the Polarity scores, one can define which tweets were Positive, Negative, or Neutral. A Polarity score of < 0 is Negative, 0 is Neutral while > 0 is Positive. I used the "apply" method on the "Polarity" column in my data frame to return the respective Sentiment Category. The distribution of the Sentiment categories is shown below. You can also see the Sentiment Category distribution per country and continent in the Tableau dashboard [HERE](https://public.tableau.com/profile/jessica.uwoghiren#!/vizhome/TwitterUsers2020ReflectionsDashboard/FinalDashboard)

![alt text](https://github.com/jess-data/Twitter-2020-Sentiment-Analysis/blob/master/Distribution%20of%20Sentiments%20Results.png)

## Remarks
Some of the insights I generated are stated below:
* __Tweet Sentiments__: I was not surprised by the proportion of the sentiment categories because, for most people, the end of the year is a time to show gratitude and hope for a better year ahead. However, this year has been filled with so many unpalatable events, hence, 31% of the tweets being Negative. *Please note that this is not indicative of the entire Twitter community as only a subset of tweets were mined for this analysis.
* __Countries with Most Tweets__: About 40% of the total tweets emanated from the United States, England and Canada. Since a good number of Twitter users do not have their exact location on their profiles, their tweet locations were classified as "Unknown location".
* __Hour of the day with the Most Tweets__: It was interesting to see that most tweets were created at 5 PM (GMT). Thinking about it, in the US & Canada, this is lunchtime while in countries like Nigeria and England, it is when most individuals finish the work-day, so they have ample time to tweet.
* __Hour of the day with Least Tweets__: 9 AM (GMT) was the hour of the day with the least number of tweets. The reason is this is when most people start their day at work in countries like Nigeria and England while it is still bed-time in other countries like the US & Canada.
* __Most Retweeted and Liked Tweet__: For the period of 12th to 25th December 2020, the tweet with the most retweets was about a Korean boy band: "BTS" and their songs with 10,873 RTs. The most liked tweet from a user who tweeted about how "2020 was a good year for his dog who did not have to be alone for a second". The tweet had 42,295 likes.

## Relevant Links
* [Tableau Dashboard](https://public.tableau.com/profile/jessica.uwoghiren#!/vizhome/TwitterUsers2020ReflectionsDashboard/FinalDashboard)
* [Jupyter Notebook](https://nbviewer.jupyter.org/github/jess-data/Twitter-2020-Sentiment-Analysis/tree/master/Twitter%20Sentiment%20Analysis%20Project.ipynb0)
* [Personal Website](https://jess-analytics.com/)
* [Medium Article](https://jess-analytics.medium.com/)
* [LinkedIn](https://www.linkedin.com/in/jessicauwoghiren/)
* [Twitter](https://twitter.com/jessica_xls)
* [DataTech Space Community](https://linktr.ee/DataTechSpace)

