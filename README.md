# Recommendation-with-IBM
## Introduction
For this project we will analyze the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles we think they will like. Below you can see an example of what the dashboard could look like displaying articles on the IBM Watson Platform.

![display](display.png)

Though the above dashboard is just showing the newest articles, you could imagine having a recommendation board available here that shows the articles that are most pertinent to a specific user.

## The project will be divided into the following tasks

**I. Exploratory Data Analysis**

Before making recommendations of any kind, you will need to explore the data you are working with for the project. Dive in to see what you can find. There are some basic, required questions to be answered about the data you are working with throughout the rest of the notebook. Use this space to explore, before you dive into the details of your recommendation system in the later sections.

**II. Rank Based Recommendations**

To get started in building recommendations, you will first find the most popular articles simply based on the most interactions. Since there are no ratings for any of the articles, it is easy to assume the articles with the most interactions are the most popular. These are then the articles we might recommend to new users (or anyone depending on what we know about them).

**III. User-User Based Collaborative Filtering**

In order to build better recommendations for the users of IBM's platform, we could look at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users. This would be a step in the right direction towards more personal recommendations for the users. You will implement this next.

**IV. Content Based Recommendations (EXTRA - NOT REQUIRED)**

Given the amount of content available for each article, there are a number of different ways in which someone might choose to implement a content based recommendations system. Using your NLP skills, you might come up with some extremely creative ways to develop a content based recommendation system. You are encouraged to complete a content based recommendation system, but not required to do so to complete this project.

**V. Matrix Factorization**

Finally, you will complete a machine learning approach to building recommendations. Using the user-item interactions, you will build out a matrix decomposition. Using your decomposition, you will get an idea of how well you can predict new articles an individual might interact with (spoiler alert - it isn't great). You will finally discuss which methods you might use moving forward, and how you might test how well your recommendations are working for engaging users.

## File Descriptions
**Recommendations_with_IBM.ipynb** - Jupyter Notebook for project<br/>
**project_test.py** - Python file contains solutions for test questions in the Jupyter Notebook.<br/>

**top_10.p** - P file contains top 10 articles.<br/>
**top_20.p** - P file contains top 20 articles.<br/> 
**top_5.p** - P file contains top 5 articles.<br/>
**user_item_matrix.zip** - zipped file for *user_item_matrix.p*. We need to unzip the file to use it. This is P file containing user item matrix that we will use to perform Singular Value Decomposition (SVD).<br/>
(**Note:** P files are used by project_test.py to test top n articles we obtained via functions we created.)<br/>

### Folder: data<br/>
**articles_community.csv** - articles available on the IBM platform<br/>
**user-item-interactions.csv** - list of articles that users interact with<br/>

## Installation
There should be no extra libraries required to install apart from those coming together with Anaconda distribution. There should be no issue to run the codes using Python 3.5 and above.

### Libraries Used
pandas, numpy, matplotlib, pickle

## Instructions
Run the codes inside Jupyter notebook to complete the project.

#### *Future Work*
Using the notebook, we could now save our recommendations for each user, develop a class to make new predictions and update our results, and make a flask app to deploy our results.

## Acknowledgements
* [IBM](https://www.ibm.com/) for providing user interaction article dataset from IBM Watson Studio.
