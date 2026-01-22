# Movie-Recommendation-System-using-KNN-K-Nearest-Neighbors-and-CF-Collaborative-Filtering-
Built a movie recommendation system using KNN and collaborative filtering on the MovieLens dataset. Performed EDA to analyze sparsity, implemented unweighted and weighted KNN, and user-based CF using cosine similarity. Compared models using RMSE, with weighted KNN achieving the best accuracy.

## Project Overview
The objective of this project is to design and evaluate recommendation models capable of handling sparse user–item interaction data. By applying neighborhood-based machine learning techniques, the system identifies similarities among users to recommend relevant movies.

The project follows a complete data mining lifecycle, including exploratory data analysis, model implementation, and performance evaluation.

## Dataset

**MovieLens Dataset**
Source: GroupLens Research  
The dataset contains user IDs, movie IDs, ratings, and timestamps. Due to the large number of users and movies, the user–item matrix is highly sparse, making it suitable for collaborative filtering techniques.

## Methodology

### Exploratory Data Analysis (EDA)
Exploratory analysis was performed to understand rating distributions, user activity levels, movie popularity, and sparsity patterns. Data cleaning and preprocessing were conducted to prepare the dataset for modeling.

### K-Nearest Neighbors (KNN)
Two KNN-based recommendation models were implemented:

Unweighted KNN predicts ratings by computing the simple average of ratings from the k-nearest neighbors.  
Weighted KNN assigns higher importance to neighbors with stronger similarity scores.

Multiple values of k (3, 5, and 10) were tested to evaluate performance differences.

### Collaborative Filtering (CF)
A User-Based Collaborative Filtering model was built using cosine similarity to identify users with similar rating behavior. Predictions were generated based on ratings from similar users.

## Key Findings
Unweighted KNN provided reasonable predictions but showed sensitivity to the choice of k.  
Weighted KNN consistently achieved lower RMSE values, improving overall prediction accuracy.  
Collaborative Filtering handled sparsity effectively, but Weighted KNN outperformed other models.

## Tools & Technologies
Python  
Pandas  
NumPy  
Scikit-learn  
Matplotlib  
Seaborn  

## Conclusion
This project demonstrates the effectiveness of neighborhood-based recommendation techniques for sparse datasets. Among all evaluated approaches, Weighted KNN delivered the highest accuracy, emphasizing the importance of similarity-weighted contributions in recommendation systems.

## Course Information
Course Name: CS 504 – Principles of Data Management and Data Mining  
Instructor: Dr. Isaac K. Gang
