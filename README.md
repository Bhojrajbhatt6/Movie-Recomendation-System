# Movie-Recomendation-System
# Movie Recommendation System

## Overview

This repository hosts a comprehensive Movie Recommendation System implemented in Python. The system utilizes natural language processing techniques to recommend movies based on user preferences and content similarities.

## Dataset

The primary dataset comprises two CSV files: `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`. These files contain essential information about movies, including details like title, overview, genres, keywords, cast, crew, and more.

## Data Preprocessing

1. **Merging Data:** The two datasets are merged on the 'title' column to create a consolidated dataset providing a holistic view of each movie.

2. **Handling Missing Values:** Null values are handled appropriately to ensure data quality and completeness.

## Feature Engineering

The dataset undergoes extensive feature engineering to extract relevant information and create a set of tags for each movie. The tags include data from movie overviews, genres, keywords, cast, and crew.

## Model Training

The recommendation system employs a CountVectorizer to convert the textual data into a numerical format suitable for machine learning. This process involves transforming the tags into feature vectors, which are then used to calculate cosine similarity between movies.

## Movie Recommendation

The recommendation system takes a movie title as input and identifies similar movies based on cosine similarity scores. The top five recommended movies are then presented to the user.

## Example Usage

```python
# Example usage of the recommendation system
recommend('Gandhi')
# Output:
# Gandhi, My Father
# The Wind That Shakes the Barley
# A Passage to India
# Guiana 1838
# Ramanujan
```

## Model Serialization

The trained model and the similarity matrix are serialized using the `pickle` library. The serialized files, `movie_list.pkl` and `similarity.pkl`, allow for easy loading and reuse of the recommendation system.

## How to Use

1. **Run the Notebook:** Open the provided Jupyter notebook and execute the cells to train the model and generate recommendations.

2. **Explore Recommendations:** Experiment with different movie titles to receive personalized recommendations based on the trained model.

## Acknowledgments

Special thanks to the Kaggle community for providing the movie datasets used in this project.

## Questions and Feedback

If you have any questions, suggestions, or improvements, feel free to reach out. Your feedback is valuable and contributes to the enhancement of this Movie Recommendation System. Enjoy exploring the world of movies!
