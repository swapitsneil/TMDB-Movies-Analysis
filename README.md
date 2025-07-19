# TMDB 5000 Movies Dataset Analysis

Project Overview
This project analyzes the TMDB 5000 Movies Dataset, a comprehensive collection of movie data sourced from The Movie Database (TMDB). The dataset includes information on financial performance, popularity, genres, cast, crew, and more. The analysis aims to answer key questions about movie trends, director performance, and production company success using Python and data analysis libraries like Pandas, NumPy, Matplotlib, and Seaborn.
Objectives
The project addresses the following questions:

What is the average runtime of movies over the years? Are movies getting longer or shorter?
Which director has the highest average revenue?
What is the relationship between vote average and revenue?
Do movies with a star-studded cast perform better in terms of revenue?
Which production companies have the highest average revenue?

Dataset

Source: The Movie Database (TMDB)
Files:
tmdb_5000_movies.csv: Contains movie details such as budget, revenue, runtime, genres, and vote average.
tmdb_5000_credits.csv: Includes cast and crew information for each movie.


Size: 4,803 movies with 20 columns in the movies dataset and 4 columns in the credits dataset.
Key Columns:
Movies: budget, revenue, runtime, vote_average, release_date, production_companies
Credits: cast, crew, movie_id



Prerequisites
To run this project, you need the following:

Python 3.x
Libraries:pip install pandas numpy matplotlib seaborn


Jupyter Notebook or any Python IDE
Dataset files: tmdb_5000_movies.csv and tmdb_5000_credits.csv (available from Kaggle)

Installation

Clone this repository:git clone https://github.com/your-username/tmdb-movies-analysis.git
cd tmdb-movies-analysis


Install the required dependencies:pip install -r requirements.txt


Ensure the dataset files (tmdb_5000_movies.csv and tmdb_5000_credits.csv) are in the project directory.

Usage

Open the Jupyter Notebook:jupyter notebook moviedataset.ipynb


Run the cells in the notebook to perform the analysis. The notebook includes:
Data loading and preprocessing
Analysis for each of the five questions
Visualizations and insights



Key Findings

Average Runtime: Analysis of movie runtimes over the years to identify trends in movie length.
Top Director: Chris Buck (director of Frozen) has the highest average revenue at $1.27B, followed by directors like Kyle Balda, Lee Unkrich, and James Cameron.
Vote Average vs. Revenue: A weak positive correlation (0.19) indicates higher ratings do not strongly predict higher revenue.
Cast Size Impact: A moderate positive correlation (0.34) suggests movies with larger casts tend to earn more, but cast size is not the sole factor.
Top Production Companies: Companies like Abu Dhabi Film Commission ($1.5B), Prime Focus ($1.4B), and Lightstorm Entertainment ($1.1B) have the highest average revenue.

Drawbacks

Missing Data: Some movies lack budget, revenue, or runtime data, affecting analysis accuracy.
Zero Values: Unrealistic zero values for budget and revenue skew financial insights.
Unstructured Data: JSON-like strings for genres, cast, and crew require preprocessing.
Popularity Score: The dataset's popularity metric lacks clear documentation, limiting its reliability.
Limited Scope: The dataset covers only 5,000 movies, potentially missing broader industry trends.

Project Structure
tmdb-movies-analysis/
│
├── moviedataset.ipynb          # Jupyter Notebook with the analysis
├── tmdb_5000_movies.csv        # Movie dataset
├── tmdb_5000_credits.csv       # Credits dataset
├── README.md                   # Project documentation           

Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes and commit (git commit -m "Add feature").
Push to the branch (git push origin feature-branch).
Open a pull request.
