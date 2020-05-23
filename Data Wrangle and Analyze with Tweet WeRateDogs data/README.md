# Wrangle and Analyze Data by Aditya Kumar

_Data Analyst nanodegree - Udacity_

# Introduction

This project focused on wrangling data from the WeRateDogs Twitter account using Python, documented in a Jupyter Notebook (wrangle_act.ipynb). This Twitter account rates dogs with humorous commentary. The rating denominator is usually 10, however, the numerators are usually greater than 10.
[They’re Good Dogs Brent](http://knowyourmeme.com/memes/theyre-good-dogs-brent)
wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations. WeRateDogs has over 4 million followers and has received international media coverage.

WeRateDogs downloaded their Twitter archive and sent it to Udacity via email exclusively for us to use in this project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017

## The Data

### Enhanced Twitter Archive

The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, which I used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced.".We manually downloaded this file manually by clicking the following link: [twitter_archive_enhanced.csv](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/59a4e958_twitter-archive-enhanced/twitter-archive-enhanced.csv)

### Additional Data via the Twitter API

Back to the basic-ness of Twitter archives: retweet count and favorite count are two of the notable column omissions. Fortunately, this additional data can be gathered by anyone from Twitter's API. Well, "anyone" who has access to data for the 3000 most recent tweets, at least. But we, because we have the WeRateDogs Twitter archive and specifically the tweet IDs within it, can gather this data for all 5000+. And guess what? We're going to query Twitter's API to gather this valuable data.

### Image Predictions File

he tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file (image_predictions.tsv) hosted on Udacity's servers and we downloaded it programmatically using python Requests library on the following (URL of the file: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv)

## Key Points

Key points to keep in mind when data wrangling for this project:

* We only want original ratings (no retweets) that have images. Though there are 5000+ tweets in the dataset, not all are dog ratings and some are retweets.

* Fully assessing and cleaning the entire dataset requires exceptional effort so only a subset of its issues (eight (8) quality issues and two (2) tidiness issues at minimum) need to be assessed and cleaned.

* Cleaning includes merging individual pieces of data according to the rules of tidy data.

* The fact that the rating numerators are greater than the denominators does not need to be cleaned. This unique rating system is a big part of the popularity of WeRateDogs.

* We do not need to gather the tweets beyond August 1st, 2017. We can, but note that we won't be able to gather the image predictions for these tweets since we don't have access to the algorithm used.

# Project Details

Fully assessing and cleaning the entire dataset would require exceptional effort so only a subset of its issues (eight quality issues and two tidiness issues at minimum) needed to be assessed and cleaned.

The tasks for this project were:

* Data wrangling, which consists of:
  * Gathering data
  * Assessing data
  * Cleaning data
* Storing, analyzing, and visualizing our wrangled data
* Reporting on 1) our data wrangling efforts and 2) our data analyses and visualizations

## Installing

* Install Jupyter Notebook to run `wrangle_act.ipynb`.
* Need consumer_key, consumer_secret, access_token, access_secret to query from Twitter API.
* Require the following libraries installed.

* numpy
* pandas
* requests
* tweepy
* json
* matplotlib.pyplot

## Files

* `act_report`: Communicates the insights and displays the Visualizations produced from the wrangled data.
* `./Data/image_prediction.tsv`: Data downloaded using Requests library and URL.
* `./Data/tweet_json.txt`: Data gathered from twitter API.
* `./Data/twitter-archive-enhanced.csv`: File downloaded from Udacity.
* `./Data/twitter_archive_master.csv`: The clean DataFrame 1.
* `./Data/twitter_image_predictions.csv`: The clean DataFrame 2.
* `wrangle_act.ipynb`: The main file containing all the gathering, wrangling and analyzing work.
* `wrangle_report`: Briefly describes my wrangling efforts.

(Check the wrangling [here](http://htmlpreview.github.io/?https://github.com/connectaditya/Wrangle-and-Analyze-Data/blob/master/wrangle_reports.pdf) )

## Resources

* Twitter API
* Files downloaded from Udacity
