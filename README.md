# feedbacks_analysis
For Analysing the customer pain points using the customer feedbacks.

# Description
The aim of this work is to get the user problems and pain points using the feedbacks provided by them. 
The problem to get insights from feedbacks is that they are huge in numbers and manual inspection is too tiring. So I have tried to automate this process of getting insights from feedbacks using Language Processing and clustered feedbacks which have the same semantic meaning.

# Installation
To run these files you will need Jupyter Notebook.

Before start using these scripts run -

pip install -r requirements.txt

# Downloads

There are two variants of word2vec model that you can use:

1). Download the corpus of feedbacks and train your own model.

2). Download Google's pre-trained word2vec model from: [Google's Word2vec](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit)

# Usage
    -Clone the Repo
    -Make necessary installations and downloads
    -Get the feedbacks which you want to analyse and save it as .csv file.
    -Run the file modeltrain.ipynb with the downloaded data. If you have sufficient data like >6 months data you can train your   own Word2Vec model instead of using Google's Word2vec. The choice of training your own model gives better results if you have large corpus.
    -modeltrain.ipynb will take your data and preprocess it for further analysis and trains word2vec model.
    -Run the word2vec_tfidf.ipynb to get the results. You need to specify the number of clusters you want by seeing the 2-D data- points and by seeing the silhouette scores. Choose the clusters which give the max silhouette score.
    After running complete Notebook you would be able to get results in following forms : 
    a). Clusters containing the feedbacks with same sematics.
    b). The main topics from these clusters which are like tags for clusters.
    c). The summary statements for these clusters.
    d). You can search for specific keywords and filer out those feedbacks.

