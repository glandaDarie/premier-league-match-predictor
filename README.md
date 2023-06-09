# Premier League Game Winner Predictor

Premier League Game Winner Predictor is a project aimed at building models that can classify the outcome of Premier League football matches as won, drawn, or lost. The models utilize relevant information about the teams and the match to predict the outcome. This documentation provides an overview of the project, including the problem description, data used, implemented algorithms, and results.

### Problem Description
The goal of the project is to develop models that can accurately predict the outcome of Premier League matches. The models take into account various features such as team performance, goals scored, possession, and shots on target to classify matches as won, drawn, or lost. The predictions generated by the models can be valuable for coaches, players, fans, sports organizations, and media outlets.

### Data
The dataset used for this project consists of Premier League matches played during the seasons 2020/2021 and 2021/2022. The dataset, available at Data/premier_league_matches.txt, contains comprehensive information about the matches, including team names, goals scored, possession statistics, and more.
Before utilizing the dataset, preprocessing steps are applied to ensure its suitability for model training. Irrelevant features such as "captain of the team" and "notes" are removed, and the dataset is normalized or standardized to enhance the models' ability to learn from the data.

### Algorithms
Three algorithms are implemented for the Premier League Game Winner Predictor:

##### 1) K-Nearest Neighbors (KNN)
Performs well when the number of features is limited.
Straightforward implementation.
Instance-based learning algorithm, eliminating the need for a separate training phase.
More suitable for small datasets.
##### 2) Naive Bayes
Simple and easy to implement.
Fast and efficient, requiring fewer computational resources.
Performs better with discrete rather than continuous data.
Can be impacted by limited data availability.
##### 3) Logistic Classification (One-vs-All)
Simple implementation and effective for handling multi-class problems.
Performs well with a small number of training examples.
Assumes feature independence, similar to the Naive Bayes model.
Used cross entropy as the loss function, gradient descent as the optimizer and it is trained for 10000 epochs. 

### Results
The implemented models were evaluated based on their accuracy rates in predicting Premier League match outcomes. Here are the results for the testing sets:

KNN: [model: 69%], [sklearn: 79%] accuracy

Naive Bayes: [model: 69%], [sklearn: 69%] accuracy

Logistic Classification (One-vs-All): [model: 94%], [sklearn: 84%] accuracy

It is worth noting that the logistic classifier model surpasses by a significant mile the other models, with an accuracy rate of 94%. However, the accuracy rates may be influenced by factors such as dataset size, problem complexity, and feature selection.
