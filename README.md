# NextBook-Recommender-System
This repository explores recommendation engines from simple Matrix Factorization methods to NeurMF Methods

## Data Set
ratings: The data set contains ratings information of ~53,000 user on 10,000 books ordered in chronological order.
books: Contains meta information of the books including year of publishing, author, title etc.


## Collaborative Filtering
Using explicit rating information from users has been a popular way to build recommendation systems. Collaborative Filtering is one such method where predictions/ recommendation of one user are generated from interests and tastes of many users.

These recommender systems aim to fill in this missing information, by predicting the user rating of items where the score is missing. Then recommender systems will recommend items to the customer that have the highest score.

Unlike an attribute based model, this approach doesn't use any attribute information on item side(genre, author) or the user side(age, gender)

In this repo we decompose the item-user-rating matrix into its constituent item and user matrix, which are latent representations of the interactions made by the users. We use these latent factor to build item-item similarity and recommend new books to a user.

We see the t-SNE plots of the item features to understand how the books are represented in the feature space. Additionally we average out these features at author level and see if the similar authors are placed close by

