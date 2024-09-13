# Sentiment-Analysis-of-Restaurant-Reviews



## Project Purpose
This project focuses on classifying restaurant reviews by combining a fuzzy matching technique with a dataset of reviews and using Hugging Face's sentiment analysis model (`distilbert-base-uncased-finetuned-sst-2-english`). The application has two main features:
- **Review Classification**: It compares the user's review with existing reviews in the dataset and uses a sentiment analysis model to determine the sentiment.
- **Rating Distribution Visualization**: Displays the distribution of ratings from the dataset.

## Main Files
- **`Restaurant_reviews.csv`**: This file contains the restaurant reviews and corresponding ratings.
- **`full_review_sentiment_analysis.py`**: This Python script integrates fuzzy matching and sentiment analysis using Gradio for interactive review classification and plotting rating distribution.
- **`gradio_review_classifier.py`**: This Python file focuses on building a simple Gradio interface for classifying reviews and displaying a plot of rating distribution.
- **`basic_sentiment_analysis.py`**: This Python file demonstrates a basic example of sentiment analysis using the Hugging Face model.

## How Hugging Face's Sentiment Analysis Works
The project utilizes Hugging Face’s `pipeline` API to perform sentiment analysis. It uses the `distilbert-base-uncased-finetuned-sst-2-english` model to classify text as either positive or negative.

```python
classifier = pipeline('sentiment-analysis', model='distilbert-base-uncased-finetuned-sst-2-english')
```

For example:
```python
result = classifier("The food was great!")
```

This would return a sentiment classification with a confidence score.

## Running the Code

1. **Clone the Repository:**
   ```bash
   git clone <https://github.com/faisalaldwaish/Sentiment-Analysis-of-Restaurant-Reviews/tree/main>
   
   ```

## Expected Output

### Review Classifier
Input a review, and the classifier will return:
- A rating-based classification from the dataset.
- A sentiment analysis result from the Hugging Face model.
  
For example:
```
Positive review based on rating: 5
Model prediction: POSITIVE with confidence: 0.98
Matching Score: 90%
```

### Rating Distribution
<img src="https://github.com/user-attachments/assets/33d4a290-f0af-4a68-be80-4dfb06a842db" alt="Rating plot" width="500"/>

## Hugging Face Project Page

- [Hugging Face Project](https://huggingface.co/spaces/Faisalaldwaish1/Sentiment-Analysis-of-Restaurant-Reviews)

## Video Walkthrough
A video walkthrough of the project can be found in the repository. You can view it by downloading the video file or accessing the link provided if uploaded to an external platform.

--- 

This version aligns with the files you provided. Let me know if you need any further modifications!








