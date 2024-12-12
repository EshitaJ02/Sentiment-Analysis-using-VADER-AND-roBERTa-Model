# Sentiment-Analysis-using-VADER-AND-roBERTa-Model

Opinion mining, also known as sentiment analysis, is a subfield of Natural Language Processing (NLP) that focuses on identifying, extracting, and analysing subjective information from text. It involves determining the sentiment or emotion conveyed in a piece of text, such as whether the sentiment is positive, negative, or neutral. This process plays a critical role in understanding public opinion, customer feedback, and social media trends.

METHODOLOGY

#Step 1: Data Loading and Preprocessing

1.Data Collection:
o Read Amazon reviews dataset (Reviews.csv) containing review text and metadata such as Score (ratings).
o Limit to the first 500 reviews for faster experimentation.

2.Exploratory Data Analysis (EDA):
o Analyze review distribution by star ratings using bar plots.
o Highlight patterns, such as imbalanced ratings, that might affect model performance.

3.Text Tokenization and Tagging:
o Use nltk for tokenization and Part-of-Speech tagging.
o Perform Named Entity Recognition (NER) to identify named entities (e.g., product names, locations).

#Step 2: VADER Sentiment Analysis

•Calculate sentiment scores for all reviews using VADER.
•Aggregate and analyze the distribution of compound, pos, neu, and neg scores for each star rating.
•Use bar plots to visualize the correlation between sentiment scores and review ratings.

#Step 3: Roberta Sentiment Analysis

1.Text Tokenization:
o Tokenize review text into model-compatible formats using AutoTokenizer.

2.Model Prediction:
o Process each review through the Roberta model to extract sentiment probabilities.

3.Aggregation:
o Store scores for Negative, Neutral, and Positive sentiments.
o Merge results with VADER outputs for comparison.

#Step 4: Comparison of Sentiment Models

#Step 5: Visualization:
o Used line plots to compare overall sentiment scores from VADER and Roberta.
