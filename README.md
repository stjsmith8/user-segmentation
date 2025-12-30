# Spotify User Segmentation Analysis

## Overview
This project applies **unsupervised learning** to Spotify user survey data to identify distinct listener segments and uncover behavioral patterns. Using **K-Modes clustering** and **association rule mining**, the analysis demonstrates how categorical user data can inform **product, marketing, and retention strategies**.

📓 **Main notebook:**  
[spotify_user_segmentation_analysis.ipynb](https://github.com/stjsmith8/user-segmentation/blob/main/notebook/spotify_user_segmentation_analysis.ipynb)

---

## Objectives
- Identify meaningful Spotify user segments
- Evaluate how segments differ in engagement and subscription behavior
- Discover cross-feature relationships via association analysis

---

## Data
- **Source:** Kaggle – Spotify User Behavior Dataset https://www.kaggle.com/datasets/meeraajayakumar/spotify-user-behavior-dataset/data 
- **Observations:** 520 users  
- **Features:** 20 survey variables (mostly categorical)

Includes demographics, subscription status, listening habits, music and podcast preferences.

---

## Methods
- **Preprocessing:** category consolidation, missing value handling, discretization
- **Clustering:** K-Modes with elbow method + silhouette score (Hamming distance)
- **Association Analysis:** Apriori rules using support, confidence, and lift

---

## Key Findings

### User Segments
- **Cluster 0 (51%) – Core Music Users**  
  Long-term free users, smartphone-based, music-focused, moderate premium interest

- **Cluster 1 (28%) – Passive Free Users**  
  Free-tier only, low engagement beyond music, resistant to premium

- **Cluster 2 (21%) – Premium & Podcast Enthusiasts**  
  Highest premium usage, strong podcast engagement, more diverse age range

### Association Insights
- Rap listeners are ~2× more likely to listen in the afternoon  
- Classical listeners are ~2× more likely to use Spotify Radio  
- Comedy podcast listeners prefer short, storytelling formats  
- Health & fitness podcast listeners prefer longer episodes and unknown hosts  

---

## Business Value
The results show how Spotify could:
- Target premium conversion among heavy music users
- Improve discovery and engagement for passive free users
- Retain high-value podcast-focused subscribers
- Refine recommendation timing and content formats

---

## Tools
Python · pandas · kmodes · mlxtend · matplotlib · Jupyter

---

