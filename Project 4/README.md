# Exploring WeRateDogs Twitter Dataset Analysis

### WeRateDogs Twitter Dataset
> This dataset doesnt exist, but was pulled through the internet using tweepy module which as an API provided by twitter for accessing its data, The dataset is made of the tweets made by a twitter channel called WeRateDogs, every tweet has most of the following parameters: dog's name, some sentence which contains the description of the dog, and a hilarious greater than 1 proportion of rating for the dog, like 13/10. 
So after pulling the data from using tweepy I saved the data to a csv which had 27 columns and about 2356 instances or tweets after the data wrangling and data cleaning processes.


## Summary of Findings

Issues found with the datasets:

#### Tweet Data
Quality issues:
- the following columns can be dropped because we dont have any use for them:
   in_reply_to_status_id, in_reply_to_user_id,retweeted_status_id,retweeted_status_user_id,retweeted_status_timestamp, expanded_urls
- tweet id needs to be changed to string type
- the numerator and denominator ratings have inconsistencies.
- the timestamp column should be changed to datetime object.


Tidiness Issues:
- some of the dogs are classified by using more than one dog stages, while some have none for all the possible stages. And should be dropped because of the redundancy they offer.


#### Retweet Data
Quality issues

1. Remove the rows that contain the retweet data
- Remove the unnecessary columns
- Incorrect numerator extraction issue
- Cleaning the invalid dog names
- Dropping columns where all predictions are false, and ones where p1 is false and p2 and p3 are less than 30%.
- Fixing the datatypes
- Making the denominator uniform
- Fixing the inconsistencies of the predicted_breed column and optimising the breed prediction columns

#### Imagepred Data
Quality issues:
- tweet id column should be of type str.
- we should remove the img-num column as it is redundant.
- Should images dont contain dogs.

Tidiness issues:

- predictions vary between uppercase, lowercase, and have underscore in between words.


### Cleaning steps:


1. Remove the rows that contain the retweet data
- Some of the dogs are classified by using more than one dog stages, the columns could be brought down to one.
- Remove the unnecessary columns
- Incorrect numerator extraction issue
- Cleaning the invalid dog names
- Dropping columns where all predictions are false, and ones where p1 is false and p2 and p3 are less than 30%.
- Fixing the datatypes
- Merging the datasets
- Making the denominator uniform
- Fixing the inconsistencies of the predicted_breed column and optimising the breed prediction columns


### Insights
Insight 1
- We can observe that golden retriever is one of the most common dog breed found in the weratedogs dataset.

Insight 2
- Again, no surprise here , the most favorited breed of dogs was found to be golden retriever, Second most favorite was the Labrador Retriever alongside pembroke.

Insight 3
- Looks like Charlie and Cooper are the most common names amounting to 10 instances each in the dataset.


