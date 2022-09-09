# Data-Wrangling-with-Python
An interesting project based on the @WeRateDog Twitter archive for my Udacity Nanodegree Program which involved 
* Gathering data from multiple sources 
* Assessing the data visually and programmatically to identify quality and tidiness issues 
* Ridding each dataframe of every tidiness and quality issue
* Merging the three dataframes into one clean master dataframe
* Analyzing, exploring relationships and visualizing insights from the clean data 

## Gathering
In this project, I gathered three different datasets with different formats in three different ways
* Downloaded the first, a .csv file in the usual traditional way and read it into the pandas dataframe 
* I programmatically downloaded the second file, an image prediction file in .tsv format from a provided url using the Requests library
* The third dataset was sourced from Twitter using the Tweepy library to query additional data via the Twitter API, saving it into a txt file (tweet_json.txt) and reading it line by line into a pandas dataframe as tweets.

## Assessing 
The bulk of the work was done here where i had to visually assess the issues within each dataframe and document the issues. I also programmatically assessed the issues with attributes such as .info, .unique, .isna, .duplicated etc. that helped me discover wrong datatypes, data spread in different columns, duplicate rows, null values represented as 'None' as well as a myriad of other issues.

## Cleaning
All issues raised and documented were solved using the Define-Code-Test frame such as melting columns, changing datatypes, removing retweets and replies, replacing column values with 'NaN' where necessary, dropping duplicates etc.  
