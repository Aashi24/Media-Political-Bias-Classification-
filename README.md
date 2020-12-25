# Media-Political-Bias-Classification-\
Implemented the entire data science pipeline, from collecting, processing and analyzing over 10,000 articles from various news channels using Natural Language Processing.

# Table of Contents
1. Project Motivation
2. Project Tasks
3. Results
4. References

## Project Motivation 
In recent times, although very few of us read the newspaper, we all follow news channels on Twitter, have a news articles app on our phone and consume news, more specifically political news, from one source or another on a daily basis. There are about 10-12 top news channels that all of us follow, but have you ever wondered if these channels are truly neutral, and do not use their worldwide presence to steer the political views of their readers?

There is an age-old debate across countries about how media channels and the press have a strong influence on the public’s political opinions and inclinations. Any regular news viewer may already have developed their own view on where on political spectrum does each news channel lie. On several occassions, we have personally come across news stories where we can tell the political inclination right away.

So for this project, we felt it would be interesting to analyze articles from 12 news channels and try to gauge where on the political spectrum do they lie. Further, given an article from an unknown source, we will also be predicting the political inclinations of the writer.

Before we begin, here is a overview of what it means to be left wing or ring wing.

Left Wing -
"Left-wing is characterized by an emphasis on "ideas such as freedom, equality, fraternity, rights, progress, reform and internationalism"

Right Wing -
"Right-wing is characterized by an emphasis on "notions such as authority, hierarchy, order, duty, tradition, reaction and nationalism"

## Project Tasks

Details in the notebook

I.   Data Extraction

II.  Data Preprocessing

III. Exploratory Data Analysis

IV.  Modeling and Prediction

V.   Conclusion


## Results

Media bias is when journalists and producers let their bias show in their written articles, the topics they speak about and the ways the events are reported. Media biases can have a strong influence on the opinions of the viewers. This is one of the reasons the public's confidence in the news channels has hit a new low. The news articles today consist less of "reporting" and more of journalists vehemently expressing their opinions through a public channel.

For this project, we initially retrieved articles from Newsapi and then the articles content using newspaper3k and the url. Subsequently, we get the media biases from AllSides.com. After performing basic Exploratory analysis and visualization, we convert the articles into vector embeddings using two methods the Word2Vec (300 features) and Universal Sentence Encoder (512 features). We then visualize these embeddings by converting the features into a 2 dimentional space using t-SNE.

Moving forward, we trained two models, Logistic Regression and a Deep Learning model to predict the bias of a given article from the test set. We compared the accuracy obtained from the two embedding methods methods on the two models, and the Deep Learning model with Word2Vec gave us an highest accurracy.


## References

Media Bias: https://towardsdatascience.com/media-bias-detection-using-deep-learning-libraries-in-python-44efef4918d1

Political Bias: https://medium.com/linalgo/predict-political-bias-using-python-b8575eedef13

News Bias: https://towardsdatascience.com/ranking-news-bias-in-python-e9bb5d1ba93f

Text Bias: https://medium.com/towards-artificial-intelligence/text-mining-in-python-steps-and-examples-78b3f8fd913b

Sentiment: https://www.julienphalip.com/blog/identifying-bias-in-the-media-with-sentiment/

Word2vec: https://towardsdatascience.com/using-word2vec-to-analyze-news-headlines-and-predict-article-success-cdeda5f14751

Perplexity: https://distill.pub/2016/misread-tsne/

All Sides: https://www.allsides.com/unbiased-balanced-news
