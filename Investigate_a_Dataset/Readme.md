# Investigate_TMDb_Movies

The primary goal of the project is to go through the dataset and the general data analysis process using numpy, pandas and matplotlib.
This data set contains information about 10,000 movies collected from The Movie Database (TMDb), including user ratings and revenue.

## Project Overview
In this project, you will analyze a dataset and then communicate your findings about it. You will use the Python libraries NumPy, pandas, and Matplotlib to make your analysis easier.

## What do you need to install?
You will need an installation of Python, plus the following libraries:

* pandas
* NumPy
* Matplotlib
* csv

## Why this Project?
In this project, you'll go through the data analysis process and see how everything fits together. Later Nanodegree projects will focus on individual pieces of the data analysis process.

You'll use the Python libraries NumPy, pandas, and Matplotlib, which make writing data analysis code in Python a lot easier! Not only that, these are sought-after skills by employers!

## What will you learn?
After completing the project, you will:

- Know all the steps involved in a typical data analysis process
- Be comfortable posing questions that can be answered with a given dataset and then answering those questions
- Know how to investigate problems in a dataset and wrangle the data into a format you can use
- Have practice communicating the results of your analysis
- Be able to use vectorized operations in NumPy and pandas to speed up your data analysis code
- Be familiar with pandas' Series and DataFrame objects, which let you access your data more conveniently
- Know how to use Matplotlib to produce plots showing your findings

## Exploratory Data Analysis
Tip: Now that you've trimmed and cleaned your data, you're ready to move on to exploration. Compute statistics and create visualizations with the goal of addressing the research questions that you posed in the Introduction section. It is recommended that you be systematic with your approach. Look at one variable at a time, and then follow it up by looking at relationships between variables.

## Research Questions
#### Summary
> **From the investegated data set "TMDb Movie Data", the follwing questions were explored:**

 
> 1.Which movies are the most profitable to the market?

> 2.Which movies have the most and least profit, budget and runtime?

> 3.How does popularity affect the profit?

> 4.Which years do movies made the most profits?

> 5.Average Runtime Of Movies From Year To Year?

> 6.Which Genre Has The Highest Release Of Movies?

> **Data Wrangling:**

> * Features with missing values were cleaned:
    - imdb_id
    - cast
    - homepage
    - director
    - tagline
    - keywords
    - overview
    - genres
    - production_companies
* 1 duplicated row was removed
* imdb_id data was cleaned by removing the unnecessary characters (tt)
* A new column "movie_rating" was added to store the data of the rating category (Low/Medium/Above Average/High)
* A clean dataset was saved in "clean_tmdb_movies.csv" 
* Data of the genres were expanded to split the values of the genre which were stored in cells separated by "|" to answer questions 3 and 4


There are some potential limitations to the analysis presented in this work and there are some potential areas were the given data could be explored such as:
* The correlation between high budget movies and given rating. Does highly budgeted movies always get high ratings?


