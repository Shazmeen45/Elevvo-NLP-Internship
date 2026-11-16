
# Task 03: Fake News Detection Using NLP and Machine Learning

## Project Overview

This project focuses on Fake News Detection using Natural Language Processing (NLP) and Machine Learning techniques.

The objective is to classify news statements into two categories: Fake and Real. The project uses the LIAR dataset and applies text preprocessing, TF-IDF vectorization, and machine learning classification algorithms.

Two models, Logistic Regression and Multinomial Naive Bayes, are trained and evaluated to compare their performance.

## Internship Details

- **Organization:** Elevvo
- **Internship Domain:** Natural Language Processing (NLP)
- **Task:** Task 03 – Fake News Detection
- **Platform:** Google Colab

## Dataset

- **Dataset Name:** LIAR Dataset
- **Dataset Source:** [Hugging Face – LIAR Dataset](https://huggingface.co/datasets/tasksource/liar)
- **Total Records:** 12,836

### Dataset Distribution

| Dataset Split | Number of Records |
|---|---:|
| Training | 10,269 |
| Testing | 1,283 |
| Validation | 1,284 |
| **Total** | **12,836** |

The original dataset contains six labels:

- False
- Half-true
- Mostly-true
- True
- Barely-true
- Pants-fire

For this project, the six labels were grouped into two simplified categories:

- **Fake:** False, Barely-true, Pants-fire
- **Real:** Half-true, Mostly-true, True

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Hugging Face Datasets
- NLTK
- Regular Expressions

## Project Workflow

### 1. Dataset Loading
Loaded the LIAR dataset using the Hugging Face Datasets library.

### 2. Data Preparation
Converted the training, testing, and validation datasets into Pandas DataFrames.

### 3. Label Classification
Grouped the original six labels into two categories: Fake and Real.

### 4. Data Cleaning
Checked for missing values and cleaned the news statements.

### 5. Data Visualization
Visualized the distribution of Fake and Real news statements using a count plot.

### 6. Text Preprocessing
Applied the following text cleaning techniques:

- Converted text to lowercase.
- Removed URLs.
- Removed special characters and numbers.
- Removed extra whitespace.

### 7. TF-IDF Vectorization
Converted text statements into numerical features using TfidfVectorizer.

Configuration:
- Maximum Features: 20,000
- N-gram Range: (1, 2)
- Stop Words: English

### 8. Model Training
Trained two machine learning models:

- Logistic Regression
- Multinomial Naive Bayes

### 9. Model Evaluation
Evaluated both models using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix

### 10. Model Comparison
Compared the performance of Logistic Regression and Naive Bayes.

### 11. Custom Predictions
Tested the Logistic Regression model using custom news statements.

## Model Performance

The following results were obtained from the test dataset:

| Model | Accuracy |
|---|---:|
| Logistic Regression | 61.42% |
| Multinomial Naive Bayes | 61.50% |

**Best Performing Model:** Multinomial Naive Bayes

### Logistic Regression Classification Report

| Metric | Fake | Real |
|---|---:|---:|
| Precision | 0.58 | 0.63 |
| Recall | 0.41 | 0.77 |
| F1-Score | 0.48 | 0.69 |

- Accuracy: 61.42%
- Weighted F1-Score: 0.60

### Naive Bayes Classification Report

| Metric | Fake | Real |
|---|---:|---:|
| Precision | 0.61 | 0.62 |
| Recall | 0.30 | 0.85 |
| F1-Score | 0.40 | 0.72 |

- Accuracy: 61.50%
- Weighted F1-Score: 0.58

## Custom Prediction Examples

The trained Logistic Regression model was tested with custom news statements.

**Example 1:**
- Input: The government announced a new policy to improve education.
- Prediction: Fake
- Model Confidence: 52.27%

**Example 2:**
- Input: A completely fabricated statement with an unsupported claim.
- Prediction: Real
- Model Confidence: 66.68%

## Screenshots

Project screenshots are available in the `screenshots` folder.

- Dataset Preview
- Fake vs Real Category Distribution
- Logistic Regression Results
- Confusion Matrix
- Naive Bayes Results
- Model Accuracy Comparison
- Custom News Predictions
- Final Project Summary

## Project Structure

```text
Task-03-Fake-News-Detection/
│
├── Task_03_Fake_News_Detection.ipynb
├── README.md
├── requirements.txt
└── screenshots/
```

## Key Learnings

Through this project, I learned:

- How to load and explore a real-world text dataset.
- How to perform text preprocessing using Python.
- How to convert text into numerical features using TF-IDF.
- How to train Logistic Regression and Naive Bayes models.
- How to evaluate machine learning models using classification metrics.
- How to visualize and compare model performance.
- How to test trained models with custom text statements.

## Limitations

This project uses a simplified binary classification approach based on the original six LIAR dataset labels. The Fake and Real categories are educational groupings and do not represent definitive verification of news statements.

The models have limited classification performance, particularly when identifying Fake statements. Their predictions should not be considered proof that a news statement is true or false.

## Conclusion

This project demonstrates an NLP-based Fake News Detection workflow using TF-IDF and machine learning classification algorithms.

Both Logistic Regression and Multinomial Naive Bayes were trained and evaluated. Naive Bayes achieved the slightly higher test accuracy of 61.50%, compared to 61.42% for Logistic Regression.

The project provided practical experience in dataset handling, text preprocessing, feature extraction, model training, evaluation, and comparison.

---

**Developed as part of the Elevvo NLP Internship – Task 03.**
