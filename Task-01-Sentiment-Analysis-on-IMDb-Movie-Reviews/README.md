Task 01: Sentiment Analysis on IMDb Movie Reviews
Project Overview
This project focuses on Sentiment Analysis using Natural Language Processing (NLP) and Machine Learning. The objective is to classify IMDb movie reviews into two sentiment categories: Positive and Negative.

Internship Details
Organization: Elevvo
Domain: Natural Language Processing (NLP)
Task: Task 01 – Sentiment Analysis on Product Reviews
Dataset
Dataset: IMDb Movie Reviews
Source: Hugging Face – IMDb Dataset
Total Reviews Used: 25,000
Positive Reviews: 12,500
Negative Reviews: 12,500
Technologies and Libraries
Python
Google Colab
Pandas
NumPy
Matplotlib
NLTK
Scikit-learn
Project Workflow
1. Data Loading and Exploration
Loaded the IMDb movie reviews dataset.
Explored the dataset structure and sample reviews.
Checked missing values and sentiment distribution.
2. Text Preprocessing
Converted text into lowercase.
Removed HTML tags and unnecessary characters.
Removed English stopwords while preserving important negation words such as "not", "no", and "nor".
3. Feature Extraction
Applied TF-IDF (Term Frequency–Inverse Document Frequency).
Used unigrams and bigrams to convert text into numerical features.
Limited the feature set to 20,000 features.
4. Model Training
Trained two machine learning models:

Logistic Regression
Multinomial Naive Bayes
The dataset was divided into:

Training samples: 20,000
Testing samples: 5,000
5. Model Evaluation
Evaluated model performance using:

Accuracy
Precision
Recall
F1-Score
Confusion Matrix
6. Data Visualization
Visualized frequently occurring words in positive reviews.
Visualized frequently occurring words in negative reviews.
Generated a confusion matrix.
Compared the performance of both machine learning models.
7. Custom Predictions
Tested the trained sentiment classifier on custom movie reviews to predict positive or negative sentiment.

Results
Logistic Regression
Metric	Result
Accuracy	89.80%
Negative Precision	0.91
Negative Recall	0.88
Negative F1-Score	0.90
Positive Precision	0.89
Positive Recall	0.91
Positive F1-Score	0.90
Weighted F1-Score	0.90
Model Comparison
Model	Accuracy
Logistic Regression	89.80%
Multinomial Naive Bayes	87.74%
Logistic Regression achieved higher accuracy than Multinomial Naive Bayes on this dataset.

Project Structure
Elevvo-NLP-Internship/
│
├── Task-01-Sentiment-Analysis-on-IMDb-Movie-Reviews/
│   ├── Task_01_Sentiment_Analysis_on_IMDb_Movie_Reviews.ipynb
│   ├── README.md
│   └── Screenshots/
Conclusion
This project demonstrates how Natural Language Processing and machine learning algorithms can be used to classify movie reviews based on sentiment. It provided practical experience in text preprocessing, TF-IDF feature extraction, model training, model evaluation, and data visualization.

Author
Shazmeen Irshad

Internship: Elevvo NLP Internship




