Netflix Exploratory Data Analysis Project

Project Overview

This project performs an Exploratory Data Analysis (EDA) on a comprehensive dataset of movies and TV shows available on Netflix up to mid-2021. The goal is to uncover hidden patterns, analyze content distribution, and gain insights into Netflix’s global content strategy.

Objectives

Understand the structure of a real-world dataset containing over 8,800 entries.
Clean and preprocess data, specifically handling missing values in columns like director, cast, and country.
Analyze the proportion of Movies vs. TV Shows.
Identify content release trends over time and compare availability across different countries.
Create meaningful visualizations using Matplotlib and Seaborn.
Dataset Description

The dataset was sourced from Kaggle and contains 12 original columns:

show_id: A unique identifier for every movie or TV show in the dataset.
type: Categorizes the content as either a "Movie" or a "TV Show".
title: The official name of the movie or television series.
director: The individual(s) responsible for directing the content.
cast: The lead actors and actresses featured in the production.
country: The country or countries where the content was produced.
date_added: The specific date when the title was first made available on the Netflix platform.
release_year: The actual year the movie or TV show was originally released to the public.
rating: The age-based content rating (e.g., TV-MA, PG-13, TV-14).
duration: The length of the content, measured in minutes for movies or number of seasons for TV shows.
listed_in: The genres or categories assigned to the title (e.g., Documentaries, International TV Shows, Comedies).
Key Steps & Insights

Data Cleaning
Handling Missing Values: Replaced null values in director, cast, and country with "Unknown" to maintain data integrity without dropping rows.
Date Standardization: Converted date_added from an object to a datetime format to allow for time-series analysis.
Feature Engineering: Extracted the "Primary Country" from the country column to simplify geographic visualizations.
Correction of Misaligned Data: Fixed an issue where some duration values (e.g., "74 min") were incorrectly placed in the rating column.
Initial Observations Content Dominance: Netflix's library is heavily skewed toward Movies (6,100) compared to TV Shows (2,600). Freshness Factor: With a median release year of 2017, the platform prioritizes modern "hits" over a deep archive of historical classics.
Tools Used

Pandas for Data manipulation and cleaning.
NumPy for Matrix and numerical operations.
Matplotlib & Seaborn for Data visualization.
