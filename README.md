# Reddit NLP Classification

### Included in this repo: 
- Code directory:
    - 01_scraping.ipynb - used to retrieve data from web
    - 02_EDA.ipynb - data cleaning and EDA
    - 03_Modeling.ipynb - models and evaluation
- Data directory
    - contains the collected and cleaned data sets
- Images directory
    - contains the plots that were created in the EDA and modelling process

### Problem Statement:

“LovEvery” develops toys for all ages including toddlers. As a part of marketing campaign for a new toy development at “LovEvery” we need to find the target audience to make sure our adds are seen by the people who are interested in toys for toddlers.  

One of the platforms that we would like to use for our target marketing is reddit. We will research the two subreddits “r/Parents” and “r/toddlers” to determine the parents who have toddlers. 

For this project a classification model will be built to determine whether a post came from a r/Parents or r/toddlers subreddit to promote our add on the r/toddlers subreddit. 

The data has been scraped from the reddit website on September, 29, 2022. So in this project we will only look at the posts From Sept 29th and earlier. For the purposes of this project, I commented the code that determined the latest time and saved it as separate variable. 

### Summary

The data came in as a massive data frame with lots of features, the only features that will be used for this project are the name of the subreddit, the title of the post, the actual test of the post, authors name and the time the post was created. 

For the analysis of the data, we determined the most popular users from each subreddits and removed the authors with names that were deleted or removed, also got rid of the posts that are empty. As part of the feature engineering, we looked at the lengths of the posts and turns out the longest post written in r/toddlers and it is 2380 words (#TLDR). This and other authors of lengthy creations (outliers) were not used for the model and were dropped. 

In order to make the model work more efficient and be more accurate, the “stop words” were removed, as well as the emojis, links, punctuation, numbers and common for these subreddits words such as ‘daughter’, ‘son’, ‘potty’, ‘day care’, ‘school’, ‘children’, ‘old’, ‘child’,’toddler’, boy’, ‘girl’ etc. After that we determined the most common words for each subreddit. 
Interestingly (for me as a mom of a toddler) for ‘r/toddler subreddit the most common words were play, tired, sleep, home, much, help, anyone. I thought it would be “tantrum”.

For r/Parents some of the most common words were the similar, some are different. 

For modeling, we took Logistic Regression, Random Forest Classifier, Decision Tree Classifier, Ada Boost Classifier with Logistic Regression estimator, KNN classifier, Multinomial Naive Bayes have been used with Count vectorizer and TfidfVectorizer each. And tuned those with hyper parameters for better performance. Despite the fact that the f1 score never went higher than 0.7, we can say that the stacking model and the voting classifier worked best. If taking the model by itself, I’d take the Multinomial NB as a working model since it had highest f1 score (0.69). 
Unsurprisingly the KNN Classifier did not perform well, it is due to its limitations when it comes to the higher dimensions. 

### Conclusion

Overall, I’d say this is a successful project since we can predict that the post comes form r/toddlers subreddit and we can promote our new toy on that subreddit using this model. Even though the numbers are not that high due to the overlapping subjects of these two subreddits. The r/Parents subreddit may as well be considered as an umbrella for r/toddlers subreddit, as it was shown during EDA that a lot of users (152 out of 2112) are posting in both subreddits. 

In the case when this model would be wrong, people from other subreddits (such as r/Parents) will see the add and they may have friends who have toddlers or have babies who will very soon become toddlers. 

As the next steps to improve this process, I’d pull some data from the websites such as yelp where parents talk about the quality of the toys from certain stores, and see if we can collaborate with those toy stores. 
For the data cleaning, I’d suggest lemmatizing or stemming the words, to see if it increases the performance of the models. Also, if time were permitting, I’d do more model trials with more huperparameters tuning and would focus on decreasing the variance. And then try to promote these apps based on people’s interest on social media platforms such as Instagram by setting up the target adds for a certain audience. Implement/generalize this model for other types of subreddits and target audience for future use on other topics (babies, back-to-school campaign). 
