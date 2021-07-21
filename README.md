# Twitter-hate/inappropriate-tweet-analysis
### Table of Content:

1. [Project Motivation](#motivation)
2. [Descriptions](#file)
3. [Installation](#installation) 
4. [Results and Improvements](#results)
   
## Project Motivation : <a name="motivation"></a>
Building an supervised classification model. We want to build an efficient supervised classification models that classifies whether a tweet is hate / inappropriate or normal tweet. 

What are we intereseted in answering the following question:
1. Which tweets posted by twitter users are inappropriate / hateful?

## Descriptions : <a name="file"></a>
The dataset `train.csv` used in this notebook contains 37k tweets with labels 0 and 1.

Here is the explanation of each feature in the file :

   `train.csv`
   - tweet : Tweet posted by a twitter user.
   - label : 0 - Normal tweet , 1 - Hatefule tweet
   
The six notebooks we see perform the follwong functions:
   - ETL Notebook : This notebook contains the Extract, Transform and load pipline (ETL pipeline).
   - Modelling Notebook : This notebook contains the Machine learning pipeline developed with NLTK and Scikit-Learn.
   - Results : Run this notebook to compare the results of different classification model implemented.
   - Transform_tweet : This notebook contains the text preprocessing pipeline to clean the input tweet.
   - Results_modelling : This notebook contains the Machine learning pipeline developed with NLTK and Scikit-Learn to classify tweets using best classification model found out using Results notebook.
   - Tweet_classification : Give the tweets as input in this notebook for classification.


The description of pickle file saved in the 'Data' folder is as follows:
   - preprocessed_data : Saved preprocessed tweet data after ETL pipleline implementation.

## Installation : <a name="installation"></a>
   - Python version  3.*.


## Results and Improvements: <a name="results"></a>
Conclusion & Improvements:
1. We are still getting incorrect tweet classifications due to limited amount of training data given to the classification model. Example of this is the wrong classification of feminism realted inappropriate tweet in the Tweet_classification notebook. As the training data does not contain many tweets with such inappropriate language regarding feminism, it is impossible for the model to classify tweets with similar language as inappropriate. To solve this issue we need to increase our training data size to incorporate all different types of hate / inappropriate tweets.  

## Licensing, Authors, Acknowledgements<a name="licensing"></a>
Credit to Kaggle and Twitter for providing the data.

