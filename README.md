# CSE508_Winter2024_A3_MT23056

# Amazon Electronics Product Reviews Analysis

## Introduction
The goal of this project is to develop a predictive model for user ratings and evaluate the usefulness of reviews in recommending relevant items to users. Leveraging collaborative filtering techniques, we aim to personalize the user experience by offering tailored recommendations based on past interactions and preferences.

## Dataset
- Download the 5-core dataset for Electronics Category from the Amazon Reviews Dataset.
- Read the dataset into a dataframe and keep the product metadata in a separate dataframe.

## Product Selection
Choose a specific product category, such as 'Headphones', for analysis.

## Data Preprocessing
1. Handle missing values, duplicates, and other anomalies in the dataset.
2. Perform data cleaning and preprocessing steps like removing HTML tags, accented characters, expanding acronyms, removing special characters, lemmatization, and text normalization.

## Descriptive Statistics
1. Report the total number of reviews for the chosen product.
2. Calculate the average rating score.
3. Determine the number of unique products in the category.
4. Classify ratings as 'Good' (>=3) and 'Bad' (<3), and analyze the distribution of good and bad ratings.
5. Compute the number of reviews corresponding to each rating.

## Exploratory Data Analysis (EDA)
1. Identify the top 20 most reviewed brands and the top 20 least reviewed brands in the chosen category.
2. Determine the most positively reviewed 'Headphone' or the most positively reviewed product in the selected category.
3. Analyze the count of ratings for the product over five consecutive years.
4. Create a Word Cloud for 'Good' and 'Bad' ratings to identify common words in positive and negative reviews.
5. Plot a pie chart showing the distribution of ratings versus the number of reviews.
6. Determine the year with the maximum reviews and the year with the highest number of customers.

## Feature Engineering
Utilize feature engineering techniques such as Bag of Words model, TF-IDF, Hashing Vectorizer, or Word2Vec to model review text.

## Machine Learning Models
1. Divide the dataset into training and testing data in a 75:25 ratio.
2. Evaluate the performance of five machine learning models based on Precision, Recall, F1-Score, and Support for each target class (Good, Average, Bad).

## Collaborative Filtering
1. Create a user-item rating matrix.
2. Normalize the ratings using min-max scaling.
3. Develop a user-user recommender system:
   - Find the top N similar users using cosine similarity (N = 10, 20, 30, 40, 50).
   - Implement K-folds validation (K = 5) for training and validation sets.
   - Predict missing values and calculate the Mean Absolute Error (MAE) for different values of K.
4. Build an item-item recommender system using similar steps as the user-user recommender system.
5. Plot separate graphs for both recommender systems, showing MAE against K.

## Top 10 Products by User Sum Ratings
Report the top 10 products based on the sum of user ratings.

---

This README outlines the key steps and analyses performed in the project. Detailed code implementation and results are available in the project files.
