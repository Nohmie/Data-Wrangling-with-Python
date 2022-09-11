# Data-Wrangling-with-Python
An interesting project based on the @WeRateDog Twitter archive for my Udacity Nanodegree Program which involved 
* Gathering data from multiple sources 
* Assessing the data visually and programmatically to identify quality and tidiness issues 
* Ridding each dataframe of every tidiness and quality issue
* Merging the three dataframes into one clean master dataframe
* Analyzing, exploring relationships and visualizing insights from the clean data 

## Gathering
In this project, I gathered three different datasets with different formats in three different ways
* Downloaded the first, 'twitter_archive_enhanced.csv' in the usual traditional way and read it into a pandas dataframe 
* Programmatically downloaded the second file, 'image_prediction.tsv' from the provided url (https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv) using the Requests library
* Sourced data from Twitter using the Tweepy library to query additional data via the Twitter API, saving it into a txt file 'tweet_json.txt' and read it line by line into a pandas dataframe.

## Assessing 
The bulk of the work was done here where i had to visually assess the issues within each dataframe and document the issues. I also programmatically assessed the issues with attributes such as .info, .unique, .isna, .duplicated etc. that helped me discover wrong datatypes, data spread in different columns, duplicate rows, null values represented as 'None' as well as a myriad of other issues.

## Cleaning
All issues raised and documented were solved using the Define-Code-Test frame such as melting columns, changing datatypes, removing retweets and replies, replacing column values with 'NaN' where necessary, dropping duplicates etc.  
Merged the dataframes into a single dataframe and saved as a csv file 'twitter_archive_master.csv'
