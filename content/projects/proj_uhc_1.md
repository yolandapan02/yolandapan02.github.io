---
title: "Machine Learning, Sentiment Analysis, and United HealthCare CEO Shooting"
date: 2025-02-22
draft: true
---

**Research Question:** How has public opinion related to health insurance changed in the wake of the UnitedHealthcare CEO shooting?

**RQ Formulated as an ML Task:** In order to see how public opinion related to health insurance has changed in the wake of the UnitedHealthcare CEO shooting, we will conduct a machine learning classification task to predict whether Reddit posts have positive, negative, or neutral sentiments.

**Data Collection:**
- arctic_shift
- Raw data downloads in .jsonl format
- Document contains dictionaries of data
related to each comment, including
metadata, date posted (in unicode
format), username of poster, and text
from the post
- Our dataset: a dictionary mapping each
unicode date (key) to its corresponding
text content (value)

**Data Labeling:**
Using a stratified sampling method, we selected a random subset of 1,000 comments for hand-labeling, which we then used to train our model.

- To ensure consistency: We divided the dataset into four equal sections of 250 comments.

- Each of us served as the primary rater for one section and the secondary rater for another.

- We used the following labels:

    -1 for negative sentiment  
    0 for neutral sentiment  
    1 for positive sentiment  
    -99 for unrelated comments

- Once all comments had been labeled twice, we conducted a Cohen’s Kappa test to measure inter-rater agreement. Our test returned a score of 0.5, indicating a moderate level of agreement. However, disagreements existed for approximately 300 comments, which we manually reviewed and resolved.

**Data Preprocessing:**



**Exploratory Descriptive Analysis:**

**Modeling:**
- Decision Tree
- Random Forests
- Logistic Regression (Multiclassification)

**Data Analysis:**