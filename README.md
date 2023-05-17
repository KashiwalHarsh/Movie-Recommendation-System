# Movie Recommendation System

This is a movie recommendation system implemented in Python. The system utilizes a dataset containing information about 5000 movies to provide personalized movie recommendations to users. The recommendations are based on the user's preferences and the similarities between movies.

## Table of Contents
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Recommendation Algorithm](#recommendation-algorithm)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Dataset
The dataset used in this movie recommendation system consists of 5000 movies and is stored in a CSV file. Each movie in the dataset has the following attributes:
- Title: The title of the movie.
- Genre: The genre(s) of the movie.
- Overview: A brief summary of the movie's plot.
- Keywords: Keywords related to the movie.
- Cast: The main cast of the movie.
- Director: The director(s) of the movie.
- Average Rating: The average rating given to the movie by users.
- Popularity: The popularity score of the movie.
- Poster: The URL of the movie's poster.

## Installation
To run the movie recommendation system locally, follow these steps:

1. Clone this repository to your local machine or download the source code.
2. Install the required dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

## Usage
To use the movie recommendation system, follow these steps:

1. Ensure that you have installed the required dependencies (see [Installation](#installation)).
2. Run the following command to start the recommendation system:
   ```
   streamlit run main.py
   ```
3. Follow the instructions provided by the system to input your preferences and receive movie recommendations.

## Recommendation Algorithm
The movie recommendation system uses a content-based filtering approach to generate recommendations. The algorithm works as follows:

1. Preprocess the dataset by extracting relevant features from the movies, such as genre, keywords, and cast.
2. Compute the similarity between each pair of movies using a similarity metric, such as cosine similarity.
3. Given a user's preferences, calculate the similarity between the user's preferred movies and all other movies in the dataset.
4. Sort the movies based on their similarity to the user's preferences and recommend the top-rated movies.

## Examples
Here are a few examples of how to use the movie recommendation system:

1. Input your favorite movie genres, keywords, or actors/actresses, and the system will recommend similar movies.
2. Specify a particular movie, and the system will suggest movies that are similar in terms of genre, keywords, or cast.
3. Rate a set of movies, and the system will recommend movies that have high similarity to your rated movies.
