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


## Project Structure  
```
├── data
│   ├── SPOTIFY_REVIEWS_tokens.csv
│   └── SPOTIFY_REVIEWS.csv
├── environment.yml
├── notebooks
│   ├── 0 - Data Preparation.ipynb
│   ├── 1 - Sentiment Analysis.ipynb
│   ├── 2- Token Comparison.ipynb
│   ├── 2.1 - Topic Modeling_good_bad.ipynb
│   ├── 2.2 - Topic Modeling_mid.ipynb
│   └── 3 - Classification.ipynb
├── pyproject.toml
├── README.md
├── scripts
│   ├── hello_armor.py
│   ├── hello_becky.py
│   └── hello_Liujun.py
└── src
    ├── __init__.py
    ├── mypkg.egg-info
    │   ├── dependency_links.txt
    │   ├── PKG-INFO
    │   ├── SOURCES.txt
    │   └── top_level.txt
    └── spotify
        ├── __pycache__
        │   ├── mymodule.cpython-313.pyc
        │   └── utils.cpython-313.pyc
        ├── mymodule.py
        └── utils.py
```
