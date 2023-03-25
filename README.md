Exploratory Data Analysis, Model Training, and Dashboard Development for Movie Recommendation System
This repository contains the Exploratory Data Analysis (EDA), model training, and dashboard development of a movie recommendation system using two datasets taken from Kaggle.com. The datasets are:

The Movies Dataset - This dataset contains information about movies such as title, release date, budget, revenue, genres, and ratings.

The dataset also contains movies such as genres, release year, and title.

Data Sources
The Movies Dataset: https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?select=tmdb_5000_movies.csv
Data Cleaning and Preparation
Before performing the EDA and model training, some data cleaning and preparation was necessary.

The Movies Dataset required more cleaning and preparation. The following steps were taken:

Only movies with a known release year were included.

Only movies with a minimum number of votes were included to remove outliers and ensure a more representative sample.

Duplicate entries and entries with missing values were removed.

The genres column was split into separate binary columns for each genre.

The MovieLens 20M Dataset was already in a clean and structured format, but some columns such as timestamps and user IDs were dropped as they were not needed for the analysis.

Model Training
The model was trained using the Surprise library in Python, which provides a variety of recommendation algorithms. The model was trained using the MovieLens 20M Dataset and was evaluated using cross-validation. The best algorithm was selected based on its performance in terms of root mean squared error (RMSE).

Dashboard Development
The dashboard was developed using Streamlit, a Python library for building interactive web applications. The dashboard allows users to search for movies based on their title, and displays the top 10 recommended movies based on their ratings and genres. The dashboard also displays information about the selected movie, such as its title, release date, budget, revenue, and poster image.

To run the dashboard, run the app.py file and open the generated link in a web browser.

Repository Structure
data_cleaning.ipynb: Jupyter notebook containing the data cleaning and preparation code
model_training.ipynb: Jupyter notebook containing the model training code
app.py: Python file containing the code for the Streamlit dashboard
movies_metadata_cleaned.csv: Cleaned and prepared version of The Movies Dataset
movie_lens_cleaned.csv: Cleaned and prepared version of the MovieLens 20M Dataset
Note: Due to the size limitations of Github, the datasets used in this project are not included in the repository.
