data source: https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29
# Overview
1.I checked for null values , and replaced non-numeric values with most
frequent value in that column

2.I checked for outliers using boxplot and checked correlation between features
using heatmap

3.I removed highly correlated features by looking at heatmap .This heatmap
shown is after filtering

4.I splitted given data in 7:3 ratio

5.I created custom function which fits model and simultaneously maximize
recall i.e minimize false negatives

6.Model selection :

Since target label is binary my first approach was Logistic Regression

Second was Random forests

Third approach included tuning the threshold for prediction in above Random
forests since data is class imbalanced
7.Results -

Minimized false negatives were 7 using third approach

Accuracy: 86.7%
