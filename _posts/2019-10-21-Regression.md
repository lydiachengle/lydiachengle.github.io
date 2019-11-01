layout: post
title: Regression Project
---
This is our regression project for Machine Learning class what we choose a dataset and find the regression of whaever variable we choose. I choose the happiness level of counrtries around world and I was trying to predict the happiness score with relationships to other variables, such as trust, region, family etc. I dropped several meaningless variables, such as happiness ranking which is directly related to happiness score, upper confidence interval and lower confidence interval. With the analysis of pair plot,the RidgeCV, and best alpha, I came up with a quardratic model that predict the happiness score of a given values of different variebles which fits the best for in the training and test model. My final results successfully predict the happinesss score of different countries with high R^2 of training data, over 99.99%
The equation I found is: Happy Score = 5.38411341224156 + 0.00041811*Australia and New Zealand + 0.00317749*Central and Eastern Europe + 0.00072392*Eastern Asia + 0.00470529*Latin America and Caribbean....
The happiness score for Western Europe is so much higher than any other regions according to the equation, which is surprising, but also makes sense. Countries like Switzeland and Denamark always rank as the happiest countries in the world when they have reliable and various sources, such as medical care and public education.

 
