# Toxic-Challenge-Solution
Ranked 139 in the public and 528 in the private leaderboard. entered 15 days before competition end.

Scripts used for the kaggle toxic comment challenge.
1. some comment cleaning done including replacement of incorrect or misspeled words.removing puncuations,ipaddress,hyperlinks,username from the comments.
2. spell correction including replacement of the words which are not found in the embedding file.
3. using boosting and linear model on the preprocessed data.models used are: lightgbm,xgboost,ridge,logisticRegression.
4. using deep neural network model including- Lstm,Gru,Gru-Cnn and multiple layer of these models.
5. used corrrelation script to get least correlated models for the ensembling and Blending.
6. final two submits are one blending model and one ensemble model.
7. other models that are used but not in the final ensemble are Textcnn,Deepcnn,capsuleNet.All the Deep models are using pretrained glove 840b 300d embedding file and non deep models used tfidf and countvectorizer for vectorization.

Mistakes:
1. using Gpu during last 3 days only.taking 7-24 hours to train a deep learning model for 2-3 fold on cpu against 1-2 hour for 5-8 fold on Gpu.
2. using nltk lemmatizer and stemming is a big mistake because it removed the context words which are used by the rnn models.
3. using only single embedding files for all the NN model which lead to highly correlated 1 layer models. have to use the fasttext,common wiki crawl,glove twitter.
4. start ensembling on the last day
5. last overfitting on the public leaderboard.

Leason Learned and top winner techniques:
1. Train time translation

Special thanks to my teammate (Utsav) for all the support.
