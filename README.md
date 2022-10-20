# WeRateDogs-Twitter-Data-Wrangling
This project corresponds to data wrangling project within Udacity Data Analyst Nanodegree.

## 1. Introduction
Data set in real-world scenerios are prevalently messy and untidy. Over the course of this analysis, I gathered data from a variety of sources, including scrapping data from @WeRateDogs Twitter API, and assessed its quality and tidiness both visually and programmatically, then cleaned it. This whole process is known as data wrangling.

The dataset that I wrangled is the tweet archive of Twitter user @WeRateDogs which often scores account users'dogs above 10/10, accompanying humorous texts and pictures of dogs. @WeRateDogs was created in 2015 and has currently acquired 9.3+ million followers worldwide. 

<p align="center">
  <img width="482" alt="WRD_twitter_banner" src="https://user-images.githubusercontent.com/68494141/148898814-5c45e176-f36e-4895-be21-9cde60124cd0.png">
</p>

After wrangling data, I conducted analyzing step to produce some interesting and trustworthy insights and visualizations in order to answer three specific research questions:

**Question 1: Is there any correlation between retweet_count/ favorite_count with rating?**

**Question 2: What are the top 10 dog breeds in @WeRateDogs tweets, retweets and likes?**

**Question 3: Which dog stages are tweeted/ retweeted and liked the most in @WeRateDogs tweets?**

## 2. Software requirements
The following versions of libraries were implemented to conduct the project:
- pandas==1.4
- numpy==1.22
- matplotlib==3.5
- seaborn==0.11
- requests==2.27
- scipy==1.7
- tweepy==4.4

## 3. Overview of project
This project includes four parts:

Part 1: Data Gathering

I gathered data from three different data sources and combined them together into one final master dataset in order to conduct further analyses and visualizations. Specifically, data comes from twitter_archive_enhanced.csv file, image_predictions.tsv file and @WeRateDogs Twitter API. These three datasets are later combined together into 'twitter_archive_master.csv' file and converted to the final data frame in Pandas based on the common tweet ID key.

If you are interested in further details of these files and how did I process them before merge them into the master data frame, you can check out [`wrangle_report`](https://github.com/dorothy-nguyen/WeRateDogs-Twitter-Data-Wrangling/blob/main/wrangle_report.ipynb).

Part 2: Assessing Data

During this assessment step, I detected, assessed and documented quality and tidiness issues by using both visual assessment programmatic assessement. Some data quality issues and tidiness issues that I encountered were namely incorrect data types, inaccurate values for some observations, duplication, many columns representing one unit information and unmerged data sets. 

Part 3: Cleaning Data 

First of all, I made copies of original datasets to make sure I do not make changes to the original data.

Next, I applied the Define-Code-Test framework to conduct my cleansing. It means that I started by defining the methods/steps I used to fix the issues, then wrote code to clean them and finally tested if my cleaning was successful.

Part 4: Analyzing Data 

After cleaning process, I merged the three datasets into one final master dataset and exported it to 'twitter_archive_master.csv' file and then loaded it into a Pandas dataframe for analyzing and visulizing part. Find out the full report of my analyzation and presentation via [`act_report`](https://github.com/dorothy-nguyen/WeRateDogs-Twitter-Data-Wrangling/blob/main/act_report.ipynb).

## 3. Summary of main findings
I was able to answer the three research questions mentioned in the Introduction above:

**Question 1: Is there any correlation between retweet_count/ favorite_count with rating?**
- The graphs indicate that there seems to have the correlations between retweet_count/ favorite_count and rating. Tweet with higher rating has a tendency to receive more likes and retweets.
- Rating 13 appears to acquire the highest retweet counts and favorite counts as well.

**Question 2: What are the top 10 dog breeds in @WeRateDogs tweets, retweets and likes?**
- Golden Retriever gets the highest amount of tweets followed by Labrador Retriever. The third most common tweeted breed is Pembroke. Chihuahua and Pug are the fouth and fifth most popular dog breeds in @WeRateDogs Twitter respectively. Chow, Samoyed, Pomeranian, Toy_Poodle and Malamute closely take over from the 6th to the 10th highest ranks of the most popular tweeted dog breeds.
- Golden Retriever owners are the most active dog owners in writing comments and posting photos of their dogs in Twitter.
- Regarding retweet and favorite counts, Standard Poodle, English Springer, Afghan Hound, Saluki, Giant Schnauzer, French Bulldog, Flat Coated Retriever are the seven dog breeds that have both acquired the highest number of retweets and likes in @WeRateDogs Twitter.

**Question 3: Which dog stages are tweeted/ retweeted and liked the most in @WeRateDogs tweets?**
- Dog owners seem to post images and write humourous texts on their dogs significantly more frequently when their dogs are puppies. The amount of tweets about puppies doubles that of other dog stages in total. 
- On contrary to tweets, retweets and likes get favor for puppos and doggos. 
- In term of favorite count, puppos are the winner with almost 20k of favorites which is approximately three times higher than that of puppies. 

**Check out the full report of my analyzation and presentation for charts and viz via [`act_report`](https://github.com/dorothy-nguyen/WeRateDogs-Twitter-Data-Wrangling/blob/main/act_report.ipynb).**

<p align="center">
  <img width="482" alt="WRD_twitter_banner" src="[/path/to/img](https://github.com/dorothy-nguyen/WeRateDogs-Twitter-Data-Wrangling/blob/main/Happy_image.JPG).jpg">
</p>
