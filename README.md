# Sentiment-Analysis-of-Restaurant-Reviews
# Overview
This project is a Gradio application that classifies restaurant reviews using both:

Fuzzy matching to compare user input with existing reviews in a dataset.
Sentiment analysis using the Hugging Face model distilbert-base-uncased-finetuned-sst-2-english.
The application also provides a visualization of the distribution of ratings within the dataset using Seaborn and Matplotlib.

# key Features

- Sentiment Classification: Classifies reviews as positive or negative using a Hugging Face model (distilbert-base-uncased-finetuned-sst-2-english).
- Rating Prediction: Predicts the rating based on fuzzy matching with pre-existing review data.
- Review Search: Uses fuzzy matching to find the best matching review from the dataset.
- Rating Distribution: Visualizes the distribution of ratings in the dataset

  # Components:

- `basic_sentiment_analysis.py`: Demonstrates basic sentiment analysis using a Hugging Face pipeline on two sample reviews.
- `gradio_review_classifier.py`: Implements a simple Gradio interface with hardcoded reviews and their ratings.
- `full_review_sentiment_analysis.py`: Full implementation with Gradio integration, performing both sentiment analysis and review classification using the dataset.
- `Restaurant_reviews.csv`: The dataset containing restaurant reviews and ratings.
