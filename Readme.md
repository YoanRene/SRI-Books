# Recommendation Code Report

This report provides an overview and explanation of the code for performing book recommendations based on user ratings using collaborative filtering techniques.

## Table of Contents

- [Introduction](#introduction)
- [Data Preparation](#data-preparation)
- [User-Based Recommendations](#user-based-recommendations)
- [Results](#results)
- [Conclusion](#conclusion)

## Introduction

In this code, we aim to recommend books to users based on their ratings. We utilize collaborative filtering techniques to find similar users and suggest books that these users have enjoyed.

## Data Preparation

The code starts by importing the necessary libraries: `numpy`, `pandas`, `sklearn.metrics.pairwise`, `matplotlib.pyplot`, `re`, `PIL.Image`, `requests`, and `random`. These libraries are used for data manipulation, similarity calculations, visualization, regular expressions, image processing, HTTP requests, and randomization.

The code then reads the book, rating, and user data from CSV files and performs data preprocessing steps. These steps include dropping NaN values, modifying the book title format, filtering out low-voting users, and creating a pivot table of user ratings.

## User-Based Recommendations

The code defines several functions to facilitate the recommendation process. The `users_choice()` function retrieves the top 5 favorite books of a given user based on their book ratings. The `user_based()` function recommends similar users based on cosine similarity of book ratings. The `common()` function finds common recommended books among similar users.

The code randomly selects a user from the dataset and displays their favorite books using the `users_choice()` function. It then uses the `user_based()` and `common()` functions to recommend books that similar users have enjoyed.

## Results

The code generates visualizations to display the favorite books of the selected user and the recommended books based on similar users. These visualizations include the book title, average rating, and an image of the book cover (if available, that sadly is not).

## Conclusion

In this code, we have implemented a user-based collaborative filtering approach to recommend books based on user ratings. By finding similar users and suggesting books they have enjoyed, we aim to provide personalized and relevant book recommendations to users.

For a detailed understanding, please refer to the complete code.