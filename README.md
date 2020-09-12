# 10K-NLP-Stock-Prediction
Prediction of future stock returns through natural language processing of company financial statements.

Goal: predict stock future 21-day or 63-day returns by using text data of 10k and 10q filings

Process:
1. scrape historical 10-K and 10-Q filings into txt format (s&p 500 composites, from 1999 to today)
2. parsed the sections of interest (risk, md&a) into json format
3. extract features by bag-of-words, tfidf, word2vec, etc.
4. train a model to predict future returns in a rolling window or expanding window setting
5. analyze feature importance and build a financial sentiment dictionary by the trained model and compare it to Loughran-McDonald dictionary

Reference:
1. scrape and parse 10k and 10q filings:
https://www.quantopian.com/posts/scraping-10-ks-and-10-qs-for-alpha
2. Loughran-McDonald dictionary
https://sraf.nd.edu/textual-analysis/resources/
