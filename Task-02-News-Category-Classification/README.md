# Task 02: News Category Classification

## Project Overview

This project focuses on News Category Classification using Natural Language Processing (NLP) and Machine Learning.

The objective is to automatically classify news articles into four categories:

- World
- Sports
- Business
- Sci/Tech

The project uses TF-IDF for text feature extraction and Machine Learning algorithms to predict the category of news articles.

## Internship Details

- **Organization:** Elevvo
- **Domain:** Natural Language Processing (NLP)
- **Task:** Task 02 – News Category Classification
- **Intern:** Shazmeen Irshad

## Dataset

- **Dataset Name:** AG News
- **Source:** Hugging Face Datasets
- **Training Samples:** 120,000
- **Testing Samples:** 7,600
- **Number of Categories:** 4

Dataset Link: https://huggingface.co/datasets/fancyzhx/ag_news

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- Hugging Face Datasets
- Scikit-learn

## Project Workflow

1. Loaded the AG News dataset using Hugging Face Datasets.
2. Explored the dataset and analyzed news categories.
3. Cleaned and preprocessed the text data.
4. Converted text into numerical features using TF-IDF Vectorization.
5. Trained a Logistic Regression classification model.
6. Evaluated the model using accuracy, precision, recall, and F1-score.
7. Visualized model performance using a confusion matrix.
8. Trained a Multinomial Naive Bayes model for comparison.
9. Compared the performance of both models.
10. Tested the model with custom news examples.

## Model Performance

### Logistic Regression

- **Accuracy:** 91.97%
- **Weighted Precision:** 0.92
- **Weighted Recall:** 0.92
- **Weighted F1-Score:** 0.92

### Naive Bayes

- **Accuracy:** 90.17%

### Model Comparison

Logistic Regression achieved 91.97% accuracy, while Multinomial Naive Bayes achieved 90.17% accuracy on the test dataset.

Logistic Regression performed better in this experiment.

## Visualizations

The project includes:

- News category distribution
- Frequent words for each news category
- Confusion matrix
- Model accuracy comparison

## Project Structure

```text
Task-02-News-Category-Classification/
│
├── Task_02_News_Category_Classification.ipynb
├── README.md
├── requirements.txt
└── screenshots/
```

## Conclusion

This project demonstrates how Natural Language Processing and Machine Learning can be used to automatically classify news articles into different categories.

By comparing Logistic Regression and Multinomial Naive Bayes, the project evaluates two classification approaches. Logistic Regression achieved better accuracy in this experiment.

## Author

**Shazmeen Irshad**

NLP Intern – Elevvo
