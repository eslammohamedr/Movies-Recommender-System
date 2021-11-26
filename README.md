# Movies-Recommender-System

### In this Repository, I will be working with the Movie Tweetings data to apply each of the three methods of recommendations:
1. Knowledge Based Recommendations 
2. Collaborative Filtering Based Recommendations 
3. Content Based Recommendations 


### 1. Knowledge Based Recommendations
* Knowledge based recommendations frequently are implemented using filters, and are extremely common amongst luxury based goods. Filters that you might see when purchasing items like cars or homes are examples of knowledge based recommendations. In knowledge based recommendations, users provide information about the types of recommendations they would like back.
* Often a rank based algorithm is provided along with knowledge based recommendations to bring the most popular items in particular categories to the user's attention. In the linke below, you will get some practice implementing this type of recommendation for the MovieTweetings dataset.

### 2.Collaborative filtering
* Collaborative filtering is a method of making recommendations based only on the interactions between users and items. We don't need any information about items and users (information like user like or dislike item, … will be needed)

for example We know that Rima and Amir both have similar tastes in books. If we recommend a book Rima has read to Amir, this is an example of a...collaborative filtering(see below).

<img src="https://user-images.githubusercontent.com/86850708/143606222-1c94b57c-f252-49d5-8bad-25e1aa2f9041.png" width="500" height="500" class="center">

* There are two main ways to implement collaborative filtering:
1- Model Based Collaborative Filtering which uses machine learning techniques to make recommendation
2- Neighborhood Based Collaborative Filtering which is used to identify items or users that are "neighbors" with one another.

* To create Neighborhood Based Collaborative Filtering recommendations, we need to use the ratings from our neighbors to influence the ratings we provide to other users. There are a few ways to do this, but a simple method would be to:

1. Remove movies our user has already seen. 
2. Find ratings of the neighbors that are high. 
3. Recommend movies to each user where both 1 and 2 above hold. 

### 3.Content Based Recommendations
I implemented collaborative filtering to make recommendations based on finding similar users. However, there were a number of users who did not receive recommendations when using this technique. For this reason,the Content Based Recommendationsn technique will be used to find items to recommend to users. In this recommendation technique, we use information that is known about the user or item to make recommendations. This method of making recommendations is particularly useful when we do not have a lot of user-item connections available in our dataset.

It might be the case that content based and collaborative filtering based techniques come up with similar recommendations, but the methods by which data scientists approach these recommendations are very different. In collaborative filtering, you are using the connections of users and items (as you did before). In content based techniques, you are using information about the users and items, but not connections (hence the usefulness when you do not have a lot of internal data already available to use). By checking the link below you can take a look at how I implemented this method with the MovieTweetings data.
