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
* A sentiment analysis result from the Hugging Face model.
  
As shown in the figure below:
As shown in the figure below:
![image](https://github.com/user-attachments/assets/1ae9378e-b818-420a-bdfb-f964700c77f2)


### Rating Distribution
![image](https://github.com/user-attachments/assets/b99b659c-82d0-4be3-af6b-102e8be43994)


### Dataset Preview
![image](https://github.com/user-attachments/assets/a0258d71-ce5d-4538-9bf6-cc51ae78fa84)

## Running the Code

1. **Clone the Repository:**
   ```bash
   git clone <https://github.com/faisalaldwaish/Sentiment-Analysis-of-Restaurant-Reviews/tree/main>
   
   
   ```
 After running this command navigate the folder that you have save the repository at, then run *full_review_sentiment_analysis.py* file

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

## Video 
link video https://drive.google.com/file/d/1T1rsY1OINRqydjZ2tsTnlAkQYu3eBzBT/view?usp=sharing

## the dataset in kaggle
[Kaggle Restaurant Reviews Dataset](https://www.kaggle.com/datasets/joebeachcapital/restaurant-reviews)










