# Review Analysis: A Natural Language Processing Approach

## Description
This repository contains my bachelor thesis project, which I presented in 2023. The goal was to analyze Amazon product reviews using **Natural Language Processing (NLP)** techniques. I extracted real-world data using **web scraping**, performed **Sentiment Analysis** to classify reviews, and used **Topic Modeling** to uncover hidden topics in the text.

## Objectives
- Extract Amazon reviews using Python web scraping techniques.
- Classify reviews based on their ratings (from 1 to 5) using Sentiment Analysis.
- Discover latent topics within the reviews using probabilistic models.

## Key Steps

### Data Extraction:
- Used Python libraries like `BeautifulSoup` and `Requests` to extract **63,265 reviews** from **199 products** on Amazon.
- The extraction was focused on Apple products, ensuring a business-focused review analysis.

### Sentiment Analysis:
- Applied the **VADER** lexicon-based approach for sentiment classification, achieving:
  - 46% accuracy with equidistant thresholds.
  - 51% accuracy after optimizing thresholds.
- Implemented machine learning models, including:
  - **Naive Bayes**, **MultiLayer Perceptron (MLP)**, **Support Vector Classification (SVC)**, and **Random Forest**.
  - Best results were obtained with **SVC**, which achieved 63% accuracy and 86% off-by-one accuracy.

### Topic Modeling:
- Applied **K-Means** clustering and **Latent Dirichlet Allocation (LDA)** to extract topics from the reviews.
- For low-rated reviews (ratings below 3), four key topics were identified, such as product quality issues and negative experiences with sellers.

## Results
- **Sentiment Analysis** successfully classified reviews based on sentiment, with **SVC** showing the best performance.
- **Topic Modeling** revealed coherent topics related to product categories and customer concerns, particularly in negative reviews (e.g., charger issues, product return problems).
- Despite the complexity of working with real-world data, the methods proved effective in handling large datasets and extracting meaningful insights.

