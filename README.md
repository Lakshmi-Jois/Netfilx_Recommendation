# Netfilx_Recommendation
Developed a Netflix-style recommendation system using content-based filtering and weighted scoring. Used TF-IDF and cosine similarity for personalized recommendations.


Overview

This project implements a Netflix-style Recommendation System using a combination of:

Content-Based Filtering
Weighted (Priority-Based) Scoring
Hybrid Recommendation Approach

The system recommends movies/TV shows based on content similarity, user preferences, and feature weighting, even in the absence of user interaction data.


Techniques Used
🔹 1. Content-Based Filtering
Used TF-IDF Vectorization on:
listed_in (genre)
description
Applied Cosine Similarity to find similar content

Polarity-Based Weighted Scoring
Assigned weights to features such as:
Content type (TV Show/Movie)
Genre preferences (e.g., Romance, Comedy)
Rating maturity
Created a weighted score to rank recommendations

Recommendation Based on Viewing Preferences
Recommendations generated based on:
Previously watched genre/type
User preference simulation (e.g., “Because you watched Romance”)

Hybrid Recommendation System
Combined:
Content similarity (cosine similarity)
Weighted scoring (feature importance)
Produces more personalized and relevant results

Why SVD Was Not Used
Dataset does not contain user ratings or interaction data
Collaborative filtering techniques like SVD require user-item relationships
Therefore, the system focuses on content-based and hybrid methods

Features
Recommend movies/TV shows based on genre and type
Filter by country (e.g., USA, India)
Personalized recommendations using similarity
Hybrid ranking system for better results


Technologies Used
Python
Pandas
Scikit-learn
TF-IDF Vectorizer
Cosine Similarity

Conclusion

This project demonstrates how a hybrid recommendation system can effectively generate personalized recommendations using content and feature-based techniques, especially when user interaction data is unavailable.
