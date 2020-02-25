# Recommender-System-using-Collaborative-Filtering-for-Movie-lens-dataset

We will create a recommendation system with Python using pandas and SciPy. We have used famous MovieLens dataset, which is one of the most common datasets used when implementing and testing recommender engines. It contains 100k movie ratings from 943 users and a selection of 1682 movies.

You can download the dataset [here](http://files.grouplens.org/datasets/movielens/ml-100k.zip).The MovieLens dataset we have the following information: *(user id, age, location, gender, movie id, director, actor, language, year, rating)*

Two most common types of recommender systems are *Content-Based* and *Collaborative Filtering (CF)*. 

* Collaborative filtering produces recommendations based on the knowledge of users’ attitude to items, that is it uses the "wisdom of the crowd" to recommend items. 
* Content-based recommender systems focus on the attributes of the items and give you recommendations based on the similarity between them.

In general, **Collaborative filtering (CF)** is more commonly used than content-based systems because it usually gives better results and is relatively easy to understand (from an overall implementation perspective). The algorithm has the ability to do feature learning on its own, which means that it can start to learn for itself what features to use. 

CF can be divided into **Memory-Based Collaborative Filtering** and **Model-Based Collaborative filtering**. 
Here we implement Model-Based CF by using singular value decomposition (SVD) and Memory-Based CF by computing cosine similarity. 
- Memory-based models are based on similarity between items or users, where we use cosine-similarity.
- Model-based CF is based on matrix factorization where we use SVD to factorize the matrix.

In this notebook, we create two types of recommender systems:
1. a basic recommendation system by suggesting items that are most similar to a particular item, in this case, movies. This is not a true robust recommendation system, to describe it more accurately,it just tells what movies/items are most similar to your movie choice.
2. Memory-Based Collaborative Filtering(*user-item filtering* and *item-item filtering*) and Model-Based Collaborative filtering models
