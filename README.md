# Truncated-SVD
In this Mini project I have used Truncated SVD to reduce the dimensionality of Amazon fine food reviews text data.  

__PROCEDURE__:

- Tfidf Vectorization was used to vectorize the data and top 2000 features i.e words according to the idf score were saved.

- Co - Occurence matrix was constructed on these top 2000 features using the whole review text corpus.

- Co-occurence matrix was used to construct the word vectors with lower dimensions.Thus this dimensionality reduction was done using the Truncated Singular Value Decomposition.And optimal Number of dimensions were found by how much they were able to explain the variance in data.
<img src = https://github.com/yatscool007/Truncated-SVD/blob/master/Images/graph.PNG>

- After reducing the dimesnions ,K-means Clustering is performed to cluster the reviews and number of clusters were decided by plotting the elbow curve.

<img src = https://github.com/yatscool007/Truncated-SVD/blob/master/Images/hyp.PNG>

- Wordcloud is used to represent the words in each cluster to make some sense of the formation of clusters.
<img src = https://github.com/yatscool007/Truncated-SVD/blob/master/Images/Cap1.PNG>

- Finally a similarity function is constructed which outputs the most similart words to an input word

 __CONCLUSIONS__: 

- coocurrence matrix was constructed using the window size=5 and it's interpretation was pretty similar to covriance matrix
- the optimal number of dimensions that we reduced the data to was around 280,and the optimal number of clusters were around 7.
- We also observed that 'flavour' and 'taste' themes dominated the contextual formation of clusters.
- Similarity function yielded the top similar features for an incoming word
