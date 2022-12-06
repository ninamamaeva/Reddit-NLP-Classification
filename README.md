<<<<<<< HEAD
# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & NLP

### Description

In week four we've learned about a few different classifiers. In week five we learned about webscraping, APIs, and Natural Language Processing (NLP). This project will put those skills to the test.

For project 3, your goal is two-fold:
1. Using [Pushshift's](https://github.com/pushshift/api) API, you'll collect posts from two subreddits of your choosing.
2. You'll then use NLP to train a classifier on which subreddit a given post came from. This is a binary classification problem.


#### About the API

Pushshift's API is fairly straightforward. For example, if I want the posts from [`/r/boardgames`](https://www.reddit.com/r/boardgames), all I have to do is use the following url: https://api.pushshift.io/reddit/search/submission?subreddit=boardgames

To help you get started, we have a primer video on how to use the API: https://youtu.be/AcrjEWsMi_E

**NOTE:** Pushshift now limits you to 100 posts per request (no longer the 500 in the screencast).

---

### Requirements

- Gather and prepare your data using the `requests` library.
- **Create and compare two models**. Any two classifiers at least of your choosing: random forest, logistic regression, KNN, etc.
- A Jupyter Notebook with your analysis for a peer audience of data scientists.
- An executive summary of your results.
- A short presentation outlining your process and findings for a semi-technical audience.

**Pro Tip:** You can find a good example executive summary [here](https://www.proposify.biz/blog/executive-summary).

---

### Necessary Deliverables / Submission

- Code must be in at least one clearly commented Jupyter Notebook.
- A readme/executive summary in markdown.
- You must submit your slide deck as a PDF.
- Materials must be submitted by **9:30 AM (PST) on Friday, Oct. 7th**.

---

## Rubric
Your instructors will evaluate your project (for the most part) using the following criteria.  You should make sure that you consider and/or follow most if not all of the considerations/recommendations outlined below **while** working through your project.

For Project 3 the evaluation categories are as follows:<br>
**The Data Science Process**
- Problem Statement
- Data Collection
- Data Cleaning & EDA
- Preprocessing & Modeling
- Evaluation and Conceptual Understanding
- Conclusion and Recommendations

**Organization and Professionalism**
- Organization
- Visualizations
- Python Syntax and Control Flow
- Presentation

**Scores will be out of 30 points based on the 10 categories in the rubric.** <br>
*3 points per section*<br>

| Score | Interpretation |
| --- | --- |
| **0** | *Project fails to meet the minimum requirements for this item.* |
| **1** | *Project meets the minimum requirements for this item, but falls significantly short of portfolio-ready expectations.* |
| **2** | *Project exceeds the minimum requirements for this item, but falls short of portfolio-ready expectations.* |
| **3** | *Project meets or exceeds portfolio-ready expectations; demonstrates a thorough understanding of every outlined consideration.* |


### The Data Science Process

**Problem Statement**
- Is it clear what the goal of the project is?
- What type of model will be developed?
- How will success be evaluated?
- Is the scope of the project appropriate?
- Is it clear who cares about this or why this is important to investigate?
- Does the student consider the audience and the primary and secondary stakeholders?

**Data Collection**
- Was enough data gathered to generate a significant result?
- Was data collected that was useful and relevant to the project?
- Was data collection and storage optimized through custom functions, pipelines, and/or automation?
- Was thought given to the server receiving the requests such as considering number of requests per second?

**Data Cleaning and EDA**
- Are missing values imputed/handled appropriately?
- Are distributions examined and described?
- Are outliers identified and addressed?
- Are appropriate summary statistics provided?
- Are steps taken during data cleaning and EDA framed appropriately?
- Does the student address whether or not they are likely to be able to answer their problem statement with the provided data given what they've discovered during EDA?

**Preprocessing and Modeling**
- Is text data successfully converted to a matrix representation?
- Are methods such as stop words, stemming, and lemmatization explored?
- Does the student properly split and/or sample the data for validation/training purposes?
- Does the student test and evaluate a variety of models to identify a production algorithm (**AT MINIMUM:** two models)?
- Does the student defend their choice of production model relevant to the data at hand and the problem?
- Does the student explain how the model works and evaluate its performance successes/downfalls?

**Evaluation and Conceptual Understanding**
- Does the student accurately identify and explain the baseline score?
- Does the student select and use metrics relevant to the problem objective?
- Does the student interpret the results of their model for purposes of inference?
- Is domain knowledge demonstrated when interpreting results?
- Does the student provide appropriate interpretation with regards to descriptive and inferential statistics?

**Conclusion and Recommendations**
- Does the student provide appropriate context to connect individual steps back to the overall project?
- Is it clear how the final recommendations were reached?
- Are the conclusions/recommendations clearly stated?
- Does the conclusion answer the original problem statement?
- Does the student address how findings of this research can be applied for the benefit of stakeholders?
- Are future steps to move the project forward identified?


### Organization and Professionalism

**Project Organization**
- Are modules imported correctly (using appropriate aliases)?
- Are data imported/saved using relative paths?
- Does the README provide a good executive summary of the project?
- Is markdown formatting used appropriately to structure notebooks?
- Are there an appropriate amount of comments to support the code?
- Are files & directories organized correctly?
- Are there unnecessary files included?
- Do files and directories have well-structured, appropriate, consistent names?

**Visualizations**
- Are sufficient visualizations provided?
- Do plots accurately demonstrate valid relationships?
- Are plots labeled properly?
- Are plots interpreted appropriately?
- Are plots formatted and scaled appropriately for inclusion in a notebook-based technical report?

**Python Syntax and Control Flow**
- Is care taken to write human readable code?
- Is the code syntactically correct (no runtime errors)?
- Does the code generate desired results (logically correct)?
- Does the code follows general best practices and style guidelines?
- Are Pandas functions used appropriately?
- Are `sklearn` and `NLTK` methods used appropriately?

**Presentation**
- Is the problem statement clearly presented?
- Does a strong narrative run through the presentation building toward a final conclusion?
- Are the conclusions/recommendations clearly stated?
- Is the level of technicality appropriate for the intended audience?
- Is the student substantially over or under time?
- Does the student appropriately pace their presentation?
- Does the student deliver their message with clarity and volume?
- Are appropriate visualizations generated for the intended audience?
- Are visualizations necessary and useful for supporting conclusions/explaining findings?


---

### Why did we choose this project for you?
This project covers three of the biggest concepts we cover in the class: Classification Modeling, Natural Language Processing and Data Wrangling/Acquisition.

Part 1 of the project focuses on **Data wrangling/gathering/acquisition**. This is a very important skill as not all the data you will need will be in clean CSVs or a single table in SQL.  There is a good chance that wherever you land you will have to gather some data from some unstructured/semi-structured sources; when possible, requesting information from an API, but sometimes scraping it because they don't have an API (or it's terribly documented).

Part 2 of the project focuses on **Natural Language Processing** and converting standard text data (like Titles and Comments) into a format that allows us to analyze it and use it in modeling.

Part 3 of the project focuses on **Classification Modeling**.  Given that project 2 was a regression focused problem, we needed to give you a classification focused problem to practice the various models, means of assessment and preprocessing associated with classification.   
=======
# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: by Nina Mamaeva

### Note

The scrapping Jupiter notebook has a time sensitive line of code in it. If you run it, you’ll have a different set of data, then what was used for the modeling.

---

“LovEvery” develops toys for all ages including toddlers. As a part of marketing campaign for a new toy development at “LovEvery” we need to find the target audience to make sure our adds are seen by the people who are interested in toys for toddlers.  

One of the platforms that we would like to use for our target marketing is reddit. We will research the two subreddits “r/Parents” and “r/toddlers” to determine the parents who have toddlers. 

For this project a classification model will be built to determine whether a post came from a r/Parents or r/toddlers subreddit to promote our add on the r/toddlers subreddit. 

The data has been scraped from the reddit website on September, 29, 2022. So in this project we will only look at the posts From Sept 29th and earlier. For the purposes of this project, I commented the code that determined the latest time and saved it as separate variable. 

The data came in as a massive data frame with lots of features, the only features that will be used for this project are the name of the subreddit, the title of the post, the actual test of the post, authors name and the time the post was created. 

For the analysis of the data, we determined the most popular users from each subreddits and removed the authors with names that were deleted or removed, also got rid of the posts that are empty. As part of the feature engineering, we looked at the lengths of the posts and turns out the longest post written in r/toddlers and it is 2380 words (#TLDR). This and other authors of lengthy creations (outliers) were not used for the model and were dropped. 

In order to make the model work more efficient and be more accurate, the “stop words” were removed, as well as the emojis, links, punctuation, numbers and common for these subreddits words such as ‘daughter’, ‘son’, ‘potty’, ‘day care’, ‘school’, ‘children’, ‘old’, ‘child’,’toddler’, boy’, ‘girl’ etc. After that we determined the most common words for each subreddit. 
Interestingly (for me as a mom of a toddler) for ‘r/toddler subreddit the most common words were play, tired, sleep, home, much, help, anyone. I thought it would be “tantrum”.

For r/Parents some of the most common words were the similar, some are different. 


For modeling, we took Logistic Regression, Random Forest Classifier, Decision Tree Classifier, Ada Boost Classifier with Logistic Regression estimator, KNN classifier, Multinomial Naive Bayes have been used with Count vectorizer and TfidfVectorizer each. And tuned those with hyper parameters for better performance. Despite the fact that the f1 score never went higher than 0.7, we can say that the stacking model and the voting classifier worked best. If taking the model by itself, I’d take the Multinomial NB as a working model since it had highest f1 score (0.69). 
Unsurprisingly the KNN Classifier did not perform well, it is due to its limitations when it comes to the higher dimensions. 

Overall, I’d say this is a successful project since we can predict that the post comes form r/toddlers subreddit and we can promote our new toy on that subreddit using this model. Even though the numbers are not that high due to the overlapping subjects of these two subreddits. The r/Parents subreddit may as well be considered as an umbrella for r/toddlers subreddit, as it was shown during EDA that a lot of users (152 out of 2112) are posting in both subreddits. 

In the case when this model would be wrong, people from other subreddits (such as r/Parents) will see the add and they may have friends who have toddlers or have babies who will very soon become toddlers. 

As the next steps to improve this process, I’d pull some data from the websites such as yelp where parents talk about the quality of the toys from certain stores, and see if we can collaborate with those toy stores. 
For the data cleaning, I’d suggest lemmatizing or stemming the words, to see if it increases the performance of the models. Also, if time were permitting, I’d do more model trials with more huperparameters tuning and would focus on decreasing the variance. And then try to promote these apps based on people’s interest on social media platforms such as Instagram by setting up the target adds for a certain audience. Implement/generalize this model for other types of subreddits and target audience for future use on other topics (babies, back-to-school campaign). 

---
>>>>>>> a6b733f (Project 3 completed)
