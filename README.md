# Avengers: Endgame Tweet Sentiment and Emotion Analysis Using NLP

## Project Overview
This project uses Natural Language Processing (NLP) to analyze tweets about the movie **Avengers: Endgame**. The goals are:

- Determine the **sentiment** of each tweet (positive, neutral, negative)
- Analyze the **emotions** expressed in tweets (anger, joy, anticipation, sadness, fear, disgust, etc.)
- Explore the relationship between tweet popularity (favoriteCount) and sentiment/emotions

## Dataset
- **tweets.csv** contains 1000 tweets with 16 features including:
  - `screenName`, `text`, `favorited`, `favoriteCount`, `replyToSN`, `created`, `truncated`, `id`, `statusSource`, `retweetCount`, `isRetweet`, `retweeted`, `longitude`, `latitude`
  
## Objectives
- Preprocess text data:
  - Convert to lowercase
  - Remove punctuation
  - Tokenization
  - Stop words removal
  - Lemmatization
- Perform **sentiment analysis** using `SentimentIntensityAnalyzer` from NLTK
- Perform **emotion analysis** using Lexmo
- Visualize results:
  - Bar plots for compound sentiment scores vs favoriteCount
  - Emotion intensity across different tweets

## Tools and Libraries
- Python
- Pandas
- NLTK
- Lexmo
- Matplotlib / Seaborn
- Jupyter Notebook

## Methodology
1. Load the dataset.
2. Preprocess the text data for NLP.
3. Use NLTK `SentimentIntensityAnalyzer` for sentiment scoring:
   - Negative, Neutral, Positive, Compound
4. Analyze tweet emotions using Lexmo.
5. Visualize sentiment scores vs engagement (favoriteCount, retweets).
6. Draw insights about the audience sentiment and emotional trends.

## Results
- Tweets showed **predominantly positive sentiment** with a mean compound score of ~0.249.
- Positive emotions like **joy and anticipation** were higher than negative emotions (anger, fear, sadness, disgust).
- Higher favorite counts often corresponded to **more positive sentiment**.
- The analysis highlights how social media reflects audience reaction and emotional engagement with a movie.
