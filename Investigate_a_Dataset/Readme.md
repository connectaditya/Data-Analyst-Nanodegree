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

> 1. What are the Top 10 Movies by Rating?

> 2. What is the distribution of average movies ratings?

> 3. What is the Number of Produced Movies by Genres?

> 4. What is the maximum production for each genre number in a year?

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

#### Analysis vs. Results

>The analysis presented in this work sheet did answer my posed questions, I have included the answers to those questions in text below:

>**1. What are the Top 10 Movies by Rating?**

>        1. The Godfather
        2. Whiplash
        3. Bill Cunningham New York
        4. Fight Club
        5. The Dark Knight
        6. Kill Bill: The Whole Bloody Affair
        7. Schindler's List
        8. Inside Out
        9. Room
        10.Intersteller

>**2. What is the distribution of average movies ratings?**

>        The average rating is fairly distributed among the different rating categories (High, Above Average, Medium, Low)
>        On average,
>        Low              499 Movies
>        Medium           526 Movies
>        Above Average    509 Movies
>        High             457 Movies
        
>**3. What is the Number of Produced Movies by Genres?**

>     For this question, the cells containig genres was splitted to rows since genres was stored in one cell 
>     separated by '|'.
>     The chart "# of Movies by Genres Per Year" has been customized to show the counts for 5 years (2010-2015).
>     The chart is too condensed and very difficult to read. However, another chart was plotted to show the number of 
>     produced moveis. Result is below:
     
        
>        Action             532
>        Adventure          361
>        Animation          170
>        Comedy             640
>        Crime              262
>        Documentary         93
>        Drama              838
>        Family             233
>        Fantasy            202
>        Foreign              6
>        History             56
>        Horror             273
>        Music               72
>        Mystery            148
>        Romance            291
>        Science Fiction    291
>        TV Movie            16
>        Thriller           575
>        War                 44
>        Western             20

>**4. What is the maximum production for each genre number in a year?**

>        As shown in the heatmap plot, there were:
        
>        Action Movies were highly produced in 2011 (60 Movies)
>        Adventure Movies were highly produced in 2010 (32 Movies)
>        Animation Movies were highly produced in 2009 (20 Movies)
>        Comedy Movies were highly produced in 2007 (75 Movies)
>        Crime Movies were highly produced in 2009 (24 Movies)
>        Documentary Movies were highly produced in 2010 (14 Movies)
>        Drama Movies were highly produced in 2010 (99 Movies)
>        Family Movies were highly produced in 2009 (24 Movies)
>        Foreign Movies were highly produced in 2007 (2 Movies)
>        History Movies were highly produced in 2015 (8 Movies)
>        Horror Movies were highly produced in 2010 (35 Movies)
>        Music Movies were highly produced in 2013 (9 Movies)
>        Mystery Movies were highly produced in 2009 (18 Movies)
>        Romance Movies were highly produced in 2009 (37 Movies)
>        Science Fiction Movies were highly produced in 2015 (35 Movies)
>        TV Movie Movies were highly produced in 2013 (4 Movies)
>        Thriller Movies were highly produced in 2011 (64 Movies)
>        War Movies were highly produced in 2014 (7 Movies)
>        Western Movies were highly produced in 2010 (5 Movies)
