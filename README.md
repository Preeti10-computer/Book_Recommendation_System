# Book_Recommendation_System

# Project Overview:
This project involves creating a book recommendation system using a dataset of books. The system employs a content-based approach to suggest books similar to a given book based on its features, such as title, author, and publisher. It also includes data preprocessing, visualization, and exploration to gain insights into the book dataset.

# Dataset:
The dataset, book_dataset.csv, contains information about various books. Key columns include:

    - title: The title of the book
    - author: The author of the book
    - price: The price of the book
    - pages: The number of pages in the book
    - avg_reviews: The average review rating of the book
    - n_reviews: The number of reviews the book has received
    - star5, star4, star3, star2, star1: The percentage of reviews for each star rating
    - dimensions: The dimensions of the book
    - weight: The weight of the book
    - language: The language of the book
    - publisher: The publisher of the book
    - complete_link: The link to the book’s page

# Libraries Used: 
    1. Pandas: For data manipulation and analysis.
    2. NumPy: For numerical operations.
    3. Matplotlib and Seaborn: For data visualization.
    4. Scikit-learn: For implementing the TF-IDF vectorizer and cosine similarity used in the recommendation algorithm.

# Steps:

# 1. Data Loading and Initial Exploration:
    - Load the dataset using pandas.
    - Inspect the first few rows and sample data.
    - Check for missing values and data types.

# 2. Data Cleaning and Preprocessing:
    - Fill missing values in the author column with [Anonymous].
    - Convert and impute missing values in numerical columns such as price, avg_reviews, and n_reviews.
    - Process the dimensions and weight columns to convert units and handle missing values.
    - Simplify the language and publisher columns for better analysis.
    - Map categorical variables to numerical values for model compatibility.

# 3. Feature Engineering:
    - Create new features such as size (volume of the book) from dimensions.
    - Transform the language column into numerical format.
    - Normalize star ratings and handle missing values.

# 4. Data Visualization:
    - Plot distributions of numerical columns to understand the data better.
    - Visualize relationships between price and reviews, size and price, weight and price, and pages and price.
    - Identify the best books for Python and Machine Learning based on reviews and number of reviews.

# 5. Book Recommendation System:
    - Combine relevant text features (title, author, publisher) into a single combined_features column.
    - Use TfidfVectorizer to convert text data into TF-IDF matrices.
    - Compute cosine similarity between books to measure similarity.
    - Implement a recommendation function to suggest books similar to a given book based on cosine similarity.

# 6. Evaluation and Insights:
    - Analyze and visualize top publishers by total number of reviews.
    - Explore recommendations and validate with example books.

# Result and Conclusion: 
    - Recommendation System: Successfully implemented a content-based recommendation system that suggests similar books based on text features.
    - Data Insights: Visualizations revealed useful patterns, such as the impact of price on reviews and the relationship between book size, weight, and price.
    - Top Books: Identified the best books for Python and Machine Learning, along with top-rated and most-reviewed books.
    - Publisher Analysis: Found the top publishers based on total reviews.
    
The system provides personalized book recommendations and valuable insights into the dataset, helping users find books aligned with their interests.
