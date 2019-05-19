### Collaborative Filtering based Recommendation System  

#### Recommendation System (RS)
[Recommendation System](https://en.wikipedia.org/wiki/Recommender_system) is utilized in many fields such as ecommerce and gaming. It is of great interest to the industry world. Boosted by [Netflix prize](https://en.wikipedia.org/wiki/Netflix_Prize), many RS algorithms have been developed, such as SVD models. [Collaborative filtering](https://en.wikipedia.org/wiki/Collaborative_filtering) (CF) is a model is a method of making automatic predictions (filtering) about the interests of a user by collecting preferences or taste information from many users (collaborating).  CF has some real-world application such as Discover Weekly by Spotify. This project is an attempt to apply spark Collaborative filtering method ALS on a large dataset.  
![img](RS_CF.jpg)
(image from https://medium.com/@cfpinela/recommender-systems-user-based-and-item-based-collaborative-filtering-5d5f375a127f)

#### Methods
1. Used pre-made data from a gaming platform, cleaned data  
2. Feature engineer, build rating= user_id, game_id, rate score=log(time played)  
3. Collaborative Filtering model: trained pyspark.mllib.recommendation.ALS
4. Made user or item based recommendation
5. Model evaluation  

#### TODO:
feature engineering:  
1. normalize log(time played) with something like sklearn.preprocessing.StandardScaler ?  
2. using other information (devie etc.) to unsupervized cluster user  
