
# Task 04: Named Entity Recognition (NER) from News Articles

## Project Overview

This project focuses on Named Entity Recognition (NER) using Natural Language Processing (NLP) and Python.

The objective is to identify and extract named entities such as people, organizations, locations, and dates from news articles.

Two approaches are implemented:
- Rule-Based Named Entity Recognition
- Model-Based Named Entity Recognition

The project also uses spaCy's displaCy visualizer to highlight and categorize extracted entities in news text.

## Internship Details

- **Organization:** Elevvo
- **Internship Domain:** Natural Language Processing (NLP)
- **Task:** Task 04 – Named Entity Recognition from News Articles
- **Platform:** Google Colab

## Technologies and Libraries

- Python
- spaCy
- Pandas
- Matplotlib
- Seaborn

## Dataset

This project uses five sample news articles created for Named Entity Recognition.

The articles contain names of people, organizations, and locations.

- **Total News Articles:** 5
- **Text Language:** English
- **NER Model:** en_core_web_sm

## Named Entity Categories

The project identifies the following entity categories:

| Entity Label | Description | Example |
|---|---|---|
| PERSON | Names of people | Satya Nadella, Sam Altman |
| ORG | Organizations and companies | Microsoft, Google, Apple |
| GPE | Countries, cities, and locations | London, New York, Paris |
| DATE | Dates and time references | January 15, 2026 |

## Project Workflow

### 1. Library Installation and Importing
Installed and imported the required libraries, including spaCy, Pandas, Matplotlib, and Seaborn.

### 2. Load spaCy Model
Loaded the pre-trained English language model `en_core_web_sm`.

### 3. News Articles Preparation
Created five sample news articles containing different named entities.

### 4. Model-Based Named Entity Recognition
Used spaCy's pre-trained NER pipeline to automatically identify and extract entities from the news articles.

### 5. Rule-Based Named Entity Recognition
Implemented rule-based entity extraction using spaCy's EntityRuler component and manually defined patterns for people, organizations, and locations.

### 6. Comparison of NER Approaches
Compared the number of entities extracted by the rule-based and model-based approaches.

### 7. Entity Visualization
Used spaCy's displaCy visualizer to highlight named entities directly within the news article text.

### 8. Entity Category Distribution
Created a count plot to visualize the distribution of different entity categories.

### 9. Unique Entity Extraction
Extracted unique named entities and organized them according to their entity labels.

### 10. Custom News Article Testing
Tested the model using a custom news article to identify additional named entities.

## Model-Based and Rule-Based NER Results

The following results were obtained from the notebook:

| NER Approach | Extracted Entities |
|---|---:|
| Model-Based NER | 14 |
| Rule-Based NER | 13 |

### Model-Based NER Category Distribution

| Entity Category | Count |
|---|---:|
| ORG | 6 |
| GPE | 5 |
| PERSON | 2 |
| DATE | 1 |
| **Total** | **14** |

### Rule-Based NER Category Distribution

| Entity Category | Count |
|---|---:|
| ORG | 6 |
| GPE | 5 |
| PERSON | 2 |
| **Total** | **13** |

## Custom News Article Testing

A custom news statement was used to test the spaCy model.

**Input:**

Microsoft announced a technology partnership in London. Satya Nadella discussed artificial intelligence with experts from Google and OpenAI.

**Extracted Entities:**

| Entity | Predicted Label |
|---|---|
| Microsoft | ORG |
| London | GPE |
| Satya Nadella | PERSON |
| Google | ORG |
| OpenAI | GPE |

## Visualization

The project includes the following visualizations:

- Rule-Based vs Model-Based NER Comparison
- Named Entity Category Distribution
- Highlighted Named Entities using displaCy

## Project Structure

```text
Task-04-Named-Entity-Recognition/
│
├── Task_04_Named_Entity_Recognition_from_News_Articles.ipynb
├── README.md
├── requirements.txt
└── screenshots/
```

## Key Learnings

Through this project, I learned:

- The fundamentals of Named Entity Recognition.
- How to use spaCy for NLP tasks.
- How to extract people, organizations, locations, and dates from text.
- The difference between rule-based and model-based NER.
- How to create custom entity patterns using EntityRuler.
- How to visualize named entities using displaCy.
- How to analyze and compare extracted entity categories.

## Limitations

- The project uses five sample news articles instead of a large benchmark dataset such as CoNLL-2003.
- Rule-based NER depends on manually defined patterns and may miss entities that are not included in those patterns.
- Model-based NER may sometimes assign incorrect entity labels.
- The comparison is based on the number of extracted entities, not precision, recall, or F1-score.
- The custom prediction example showed an incorrect category for OpenAI, demonstrating that model predictions are not always accurate.

## Conclusion

This project demonstrates how Named Entity Recognition can be used to extract meaningful information from news articles.

Both rule-based and model-based NER approaches were implemented using spaCy. A total of 14 entities were extracted through the model-based approach, while the rule-based approach extracted 13 entities.

The displaCy visualizer was also used to highlight named entities within the text.

The project provided practical experience in NLP, sequence labeling, entity extraction, text processing, and data visualization.

---

**Developed as part of the Elevvo NLP Internship – Task 04.**
