# Financial News Sentiment and Stock Market Direction Prediction

## Overview

This repository contains the final project report for the **Financial News Sentiment and Stock Market Direction Prediction** project, developed as part of a Text Mining and Natural Language Processing research study.

The project investigates whether **daily news sentiment can predict the directional movement of the Dow Jones Industrial Average (DJIA)** using modern Natural Language Processing (NLP) techniques and machine learning models.

The study applies **FinBERT**, a transformer-based financial sentiment model, alongside **VADER**, a rule-based sentiment analysis tool, to analyze financial sentiment extracted from news headlines and evaluate their predictive capability on stock market movements.

---

## Problem Statement

Financial markets continuously react to news, public sentiment, geopolitical events, and economic developments. Understanding whether sentiment extracted from textual news data can predict stock market direction remains a significant challenge in financial analytics.

Traditional approaches often suffer from:

- Weak sentiment signals in general news data
- Lack of domain-specific NLP models
- Temporal data leakage in evaluation pipelines
- Overreliance on non-financial news sources
- Difficulty distinguishing meaningful market-moving sentiment

This project explores whether sentiment extracted from large-scale news headline datasets can provide statistically meaningful predictive signals for DJIA market direction.

---

## Project Objectives

The project was designed with the following objectives:

- Analyze financial news sentiment using advanced NLP models
- Compare transformer-based and lexicon-based sentiment approaches
- Evaluate same-day and lagged sentiment effects on market movement
- Build predictive machine learning models for DJIA direction classification
- Investigate the relationship between sentiment polarity and market volatility
- Assess the importance of source-domain relevance in financial NLP applications

---

## Dataset

The project uses the **Combined_News_DJIA** dataset from Kaggle, containing:

- 1,989 trading days
- Reddit r/worldnews headlines
- DJIA directional labels (market up/down)
- Data spanning from 2008–2016

The dataset combines daily top news headlines with corresponding stock market direction labels to support sentiment-based prediction experiments.

---

## Methodology

### Workflow

1. **Data Preprocessing**
   - Cleaned headline text
   - Removed formatting artifacts and URLs
   - Aggregated daily headlines into unified documents

2. **Sentiment Analysis**
   - Applied FinBERT for financial-domain sentiment scoring
   - Applied VADER as a rule-based baseline comparator

3. **Feature Engineering**
   - Generated same-day sentiment features
   - Created lagged sentiment variables (t−1 and t−2)
   - Constructed combined temporal feature sets

4. **Machine Learning Modeling**
   - Trained Logistic Regression models
   - Trained Support Vector Machine (SVM) classifiers
   - Applied standardized preprocessing pipelines

5. **Evaluation & Statistical Analysis**
   - Used chronological train/test split to prevent leakage
   - Evaluated Accuracy, Precision, Recall, and F1-score
   - Performed correlation and volatility analyses

---

## Technologies Used

- **Python**
- **FinBERT**
- **VADER**
- **Scikit-learn**
- **Transformers (Hugging Face)**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Machine Learning**
- **Natural Language Processing (NLP)**

---

## Key Features

- Transformer-based financial sentiment analysis
- Comparative NLP evaluation (FinBERT vs VADER)
- Time-series aware feature engineering
- Lagged sentiment prediction modeling
- Statistical correlation analysis
- Volatility and sentiment asymmetry analysis
- Chronological evaluation methodology
- Financial NLP research framework

---

## Project Impact

This project contributes to financial NLP research by:

- Demonstrating limitations of general-news sentiment for market prediction
- Highlighting the importance of domain-specific NLP models
- Establishing rigorous evaluation protocols for financial ML tasks
- Providing insights into sentiment asymmetry and market behavior
- Identifying future directions for financial-text predictive modeling

---

## Repository Contents

```text
├── Report.pdf
├── Presentation.pdf
├── Code.pdf
└── README.md
```

## Disclaimer

This repository contains academic research developed for educational purposes. The findings and implementations are intended for experimentation and research demonstration only and should not be interpreted as financial investment advice.
