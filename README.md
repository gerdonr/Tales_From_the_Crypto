# Tales_From_the_Crypto
An application of natural language processing to understand the sentiment in the latest news articles featuring Bitcoin and Ethereum

## Sentiment Analysis
##### The first step for this project was to use newsapi to get some recent articles about bitcoin and ethereum. Once we had the articles, we used SentimentIntensityAnalyzer to calculate the sentiment for each of the articles. This process returned a positive, negative, neutral, and compound sentiment score. We added these scores to a dataframe along with the text. 

##### Based on the results, Bitcoin had the highest mean positive score, but Ethereum had the highest compound score, as well as the highest positive score.

##### Next we tokenized the articles by setting stopwords, getting rid of anything that was not a letter, lemmatizing the words, and making everything lowercase. We then added these new tokenized words to our dataframe.

##### Next we looked at ngrams and the word frequency for each coin and showed the top ten words for each coin. 

##### We created wordclouds for both coins by connecting together their respective tokens into a string and then putting that string into a wordcloud generator. 

##### Lastly we build a Named Entity Recognition Model for both coins using spaCy and displaCy. Once we had the full NER visualization rendered we showed a list of all the entities in the document. 

##### Created by Rebecca Gerdon