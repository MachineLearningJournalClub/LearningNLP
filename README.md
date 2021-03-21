# LearningNLP
Some Tutorials and in depth analysis of NLP's techniques / algorithms


## Tutorial 1

### Topics 
* Sentiment Analysis with Logistic Regression 
* Sentiment Analysis with Naive Bayes 

### Possible Ideas: 

**(Simo)** 
* Scrape or Find a small-size dataset (maybe from [Kaggle-Disaster Tweets](https://www.kaggle.com/c/nlp-getting-started)), randomly sample some text from it and build a logistic regression / naive bayes classifier 
* Maybe we can take a look in depth into some explainability criteria, e.g. SHAP (shapley value) [SHAP + Sentiment Analysis](https://slundberg.github.io/shap/notebooks/linear_explainer/Sentiment%20Analysis%20with%20Logistic%20Regression.html),  [Shapley Values](https://christophm.github.io/interpretable-ml-book/shapley.html), [LIME](https://christophm.github.io/interpretable-ml-book/lime.html#lime) 
* What about looking into [MultinomialBayes](https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html#:~:text=The%20multinomial%20Naive%20Bayes%20classifier,tf%2Didf%20may%20also%20work.) or something else like an introduction on [GBMs](https://en.wikipedia.org/wiki/Gradient_boosting) (e.g. [LightGBM](https://lightgbm.readthedocs.io/en/latest/))

**(Luca B.)** 
* Maybe we can use the arxiv dataset (https://www.kaggle.com/Cornell-University/arxiv) and use the abstract to extract the cateogry. It could be useful to explore this dataset because it can be used for more advanced projects later.

**(Alessio)**
* Multiclass classification. We can introduce a model beyond logist regression, maybe Softmax...or maybe Support Vector Machine? It could be a quite "simple" topic to introduce from zero...and I have no other ideas :(
