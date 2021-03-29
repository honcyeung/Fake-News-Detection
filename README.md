# Fake News Detection
"Fake news" is "fabricated information that mimics news media content in form but not in organizational process or intent. It has been existing for a long time and becomes a common problem we face every day since the advent of internet. The phenomenon has becomes more evident when social media are increasingly popular. 
This project is to build models to detect fake news from a given dataset, to evaluate the accuracy of different models, and to perform a prediction.

<p align = "center">
  <img src = "http://static1.squarespace.com/static/5a37f0782278e769113d3880/t/5fa6ad7a8657be665edb5038/1604758912368/FAKE+NEWS.jpg?format=1500w"
       </p>

2 datasets are given for this case study: training and testing datasets. Since they are labelled and time independent, I use supervised machine learning to study the problem. I inspect, visualize, and clean the training dataset to see their patterns and characteristics. Then I deploy various models to find out which one is the most suitable for the study case. Finally I test the best model with the testing dataset to see how the prediction is.

The training dataset contains 15000 rows and  6 columns. You may combine the 3 training datasets for your convenience. The 6 variables are:
- id: unique id for a news article
- title: the title of a news article
- author: author of the news article
- text: the text of the article; could be incomplete
- label: a label that marks the article as potentially unreliable
  - 1: unreliable
  - 0: reliable



The best model is SVM which I am going to use to predict. Other than kNN, all the other algorithms show similar accuracy, which is around 90% or more.
The number of predicted unreliable article is 3117 and that of reliable article is 401. In contrast to the training dataset, the testing dataset has a much higher proportion of fake news as you can see from the bar plot. Since the model is highly accurate, we can conclude that the testing dataset has more unreliable news than reliable news, and higher proportion of unreliable news than that of training dataset.
