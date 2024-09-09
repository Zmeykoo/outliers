# Outliers in classification problem or how to create "Other" category

In this repo I'm going to discuss about how to create classifier with "Other" category. 
We will consider the following approaches:
ordinary classification,
classification + anomaly detect,
threshold prediction,
...


## Why?
On the one hand, it may seem that this problem is overblown, and when preparing a dataset for training, we can simply do what we always do: 
create a balanced dataset with Category1, Category2, ..., 'Other', 
split it on train, val, test, 
train it, 
evaluate it and voila✨✨

Сan we actualy prepare "Other" data? Yes, if we can anticipate the data we will encounter in future. 
For example:
Our task is a prepare dataset for Article classifier. Labels are Medicine, Politics, Technology, Art, Other. 5 classes.
In addition, we have access to the website and the articles already published there. 
Thus, we can simply take articles that are not suitable for Medicine, Politics, Technology, Art classes and add them to Other dataset.


But what if predicting ‘Other’ data is a real challenge, or even impossible? And datapoint is user feedback instead of article?
In this repo I will try to investigate this problem.
