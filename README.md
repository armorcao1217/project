# Analyzing Consumer Feedback on Spotify

This project analyzes user satisfaction and feedback patterns for the Spotify app using Google Play Store reviews. Through sentiment analysis, topic modeling, and predictive classification, we identify key drivers of user experience and areas for improvement. 

## Group Members  
Armor Cao, Becky Song, Liujun Chen

## Research Questions  
How can Spotify Play Store reviews be analyzed to understand evolving user satisfaction, brand perception, and review patterns?

Sub-1: What is the overall sentiment trend of Spotify reviews? 

Sub-2: What are the most common words and topics in user reviews? 

Sub-3: Can review ratings be predicted based on review text features?

## Dataset  
We use the **Spotify Google Play Store Reviews** dataset from Kaggle, containing over 3.3 million reviews. After filtering by date and text quality, we derived a final, curated dataset of 1,669,701 English-dominated reviews from November 2019 to November 2023. The original dataset is available at: [https://www.kaggle.com/datasets/bwandowando/3-4-million-spotify-google-store-reviews](https://www.kaggle.com/datasets/bwandowando/3-4-million-spotify-google-store-reviews). We used a full dataset for our analysis, but due to GitHub storage limits, we uploaded only a sample of the data to this repository to show our workflow and ensure that all code could be executed with the sample of data. 

## Results & Insights
🧩 Topic Modeling — What Users Talk About
We explored recurring themes across Spotify Play Store reviews to understand what drives user satisfaction. Most feedback centers on premium pricing, ads, updates, playlists, and app performance. Positive reviews emphasize smooth listening and playlist quality, while negative reviews focus on crashes, updates, and playback issues.

👉 Insight: Core product experience and monetization design shape most user perceptions. 


😊 Sentiment Analysis — Looking Beyond Ratings
Sentiment scores show a positively skewed distribution, with most reviews neutral-to-positive. A notable finding is the “5-star anomaly,” where users give high ratings but still mention frustrations.

👉 Insight: Text sentiment adds important nuance that star ratings alone cannot capture.


🤖 Predictive Classification — Predicting Ratings from Text
We built rating prediction models using TF-IDF and Word2Vec features. TF-IDF achieved stronger performance (~75% accuracy). Both models performed well on extreme ratings but struggled with mid-range reviews due to mixed sentiment.

👉 Insight: Machine learning can detect clear opinions, but nuanced feedback remains challenging to classify.


## Project Structure  
```
├── data
│   ├── SPOTIFY_REVIEWS_tokens.csv
│   └── SPOTIFY_REVIEWS.csv
├── notebooks
│   ├── 0 - Data Preparation.ipynb
│   ├── 1 - Sentiment Analysis.ipynb
│   ├── 2- Token Comparison.ipynb
│   ├── 2.1 - Topic Modeling_good_bad.ipynb
│   ├── 2.2 - Topic Modeling_mid.ipynb
│   └── 3 - Classification.ipynb
├── Final Report
│   ├── Final Presentation.pdf
│   └── Final Report.pdf
├── README.md
```
