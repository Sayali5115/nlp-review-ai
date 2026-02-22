# Client Review Sentiment Analysis

An NLP-based sentiment analysis project developed during my internship to analyze and classify client reviews using TextBlob and VADER.

---

## Overview

This project analyzes client reviews and classifies them into **Positive**, **Neutral**, or **Negative** sentiment categories.

It combines multiple Natural Language Processing techniques and introduces a custom confidence scoring mechanism to evaluate sentiment strength.

The final output is exported as structured CSV reports for business insights and review analytics.

---

## What This Project Provides

- Text preprocessing using regular expressions
- Sentiment scoring using **TextBlob**
- Sentiment scoring using **VADER (NLTK)**
- Custom confidence score calculation
- Sentiment distribution visualization
- Structured CSV report generation

---

## NLP Workflow

### 1. Data Preprocessing

- Converted text to lowercase  
- Removed URLs  
- Removed punctuation  
- Removed extra whitespace  

### 2. Sentiment Analysis

Two approaches were implemented:

**TextBlob**
- Polarity score (-1 to +1)
- Subjectivity score (0 to 1)

**VADER (NLTK)**
- Compound sentiment score (-1 to +1)

### 3. Sentiment Classification Logic

- Polarity > 0.1 → Positive  
- Polarity < -0.1 → Negative  
- Otherwise → Neutral  

### 4. Confidence Score

Confidence Score =  
(|Polarity| + |VADER Compound|) / 2  

This metric estimates sentiment reliability.

---

## Reports Included

The repository contains three structured sentiment reports:

- `Client_Review_Sentiment_Report.csv`
- `Client_Review_Sentiment_Report1.csv`
- `Client_Review_Sentiment_Report2.csv`

Each report includes:

- Original Review  
- Cleaned Review  
- Polarity  
- Subjectivity  
- VADER Compound Score  
- Sentiment Label  
- Confidence Score  

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- TextBlob  
- NLTK (VADER Sentiment Analyzer)  
- Matplotlib  
- Seaborn  

---

## Internship Context

This project was developed during my internship as part of client review analytics.

Guided by:
- **Abhishek Jivrakh Sir** (overall internship mentorship)
- **Kapil Kalgi Sir** (Power BI mentorship)

---

## Key Learnings

- Practical implementation of NLP techniques  
- Combining multiple sentiment analysis methods  
- Designing custom evaluation metrics  
- Data visualization for sentiment trends  
- Generating structured business reports  
- Version control using Git  

---

