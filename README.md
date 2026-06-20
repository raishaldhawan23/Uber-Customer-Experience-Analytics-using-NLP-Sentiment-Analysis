# Customer-Experience-Analysis

## Business Context

Ride-hailing platforms generate thousands of customer reviews every day across app stores and feedback channels. While these reviews contain valuable information about customer satisfaction, manually reading and categorising them is practically impossible at scale.

This project analyses over 12,000 Uber customer reviews to answer several business questions:

- What proportion of customers are satisfied versus dissatisfied?
- What are the most common complaints?
- Which topics drive positive experiences?
- How strong is customer loyalty based on Net Promoter Score?
- Which operational areas should management prioritise?

The objective is to transform unstructured customer reviews into actionable business insights using Natural Language Processing (NLP).

## Executive Summary
This project analyses more than 12,000 customer reviews from Uber to understand the key drivers of customer satisfaction, loyalty, and dissatisfaction. Using Natural Language Processing (NLP) techniques in Python, the project combines sentiment analysis, topic modelling, keyword extraction, and Net Promoter Score (NPS) analysis to transform unstructured customer feedback into actionable business insights.

The analysis reveals that while most customers express positive experiences with the platform, a significant proportion of reviews highlight recurring challenges related to driver experience, ride quality, waiting times, app reliability, and customer support. Topic modelling identifies the major themes influencing customer perception, while sentiment analysis quantifies the emotional intensity behind both positive and negative experiences.

The project demonstrates how businesses can leverage text analytics to systematically monitor customer sentiment, identify operational pain points, prioritise service improvements, and strengthen customer loyalty. By converting thousands of free-text reviews into measurable insights, this analysis provides a scalable framework for data-driven customer experience management.

## Methodology
1. #### Data Collection and Cleaning:
   Sourced customer feedback data, including review scores and text reviews. Cleaned and preprocessed the data to ensure consistency and readiness for analysis.

2. #### Sentiment Analysis:
   Analysed the sentiment distribution of reviews to understand overall customer satisfaction, and identified strong positive and negative sentiments to pinpoint critical pain points.

3. #### Word Cloud Generation and Topic Modelling:
   Identified the most common pain points and strengths. Generated word clouds to visualise frequently mentioned terms in positive and negative reviews.

4. #### NPS Calculation:
   Calculated the Net Promoter Score (NPS) to measure customer loyalty and identify promoters, passives, and detractors.

5. #### Visualisation:
   Created visualisations such as bar charts, pie charts, and word clouds to present insights effectively.

## Key Findings

### 1. Customer Satisfaction is Strong but Polarised

<img width="927" height="592" alt="image" src="https://github.com/user-attachments/assets/20ea9354-3b20-4592-8fbb-9b7e01499b23" />

Out of 12,000 reviews:
| Sentiment | Reviews |
| --------- | ------: |
| Positive  |   8,732 |
| Neutral   |     333 |
| Negative  |   2,935 |

Around 73% of reviews were positive, suggesting strong overall satisfaction.

However, almost 25% of customers expressed negative experiences, indicating important operational issues that require attention.

### 2. Net Promoter Score Shows Strong Brand Advocacy

Promoters = 7926 / 12000 = 66%
Passives = 806 / 12000 = 6.7%
Detractors = 3268 / 12000 = 27.2%

NPS = 66 - 27

≈ +39
Uber has a healthy base of loyal users, although a significant minority of customers remain dissatisfied.

### 3. Driver Experience Dominates Customer Perception

Customer experience is influenced primarily by:

Driver behaviour
Ride quality
Wait times
App reliability

Improving these factors would likely have the greatest effect on customer satisfaction.

### 4. Topic Modelling Revealed Five Major Customer Themes

LDA extracted:

#### Topic 1
Ride quality and driver experience

#### Topic 2
App issues and customer complaints

#### Topic 3
Service quality and safety

#### Topic 4
Pricing and ease of use

#### Topic 5
Customer support and brand comparisons

This provides management with a structured view of what customers actually care about instead of reading thousands of reviews individually.

### 5. Strong Positive Reviews Outweigh Strong Negative Reviews

| Category        | Reviews |
| --------------- | ------: |
| Strong Positive |   3,590 |
| Positive        |   4,501 |
| Neutral         |   1,732 |
| Negative        |     886 |
| Strong Negative |   1,291 |

This demonstrates:

While Uber receives a large volume of enthusiastic customer feedback, negative experiences tend to be emotionally stronger and often relate to specific operational failures.

## Implementation and Setup
To run this project, install the necessary Python libraries:

<pre>import pandas as pd
import numpy as np
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.cluster import KMeans
from sklearn.decomposition import PCA
import matplotlib.pyplot as plt
import seaborn as sns
</pre>

## Tech Stack

- Python
- Pandas
- NumPy
- NLTK (VADER)
- Scikit-learn
- Latent Dirichlet Allocation (LDA)
- Matplotlib
- Seaborn
-Jupyter Notebook

