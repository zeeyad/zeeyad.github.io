---
layout: post
title: Automated Exploratory Data Analysis Tool - Part 2
---

{{ page.title }}
================

<p class="meta">18 Oct 2022</p>

Here's the Link: [https://heyfasteda.streamlitapp.com/](https://heyfasteda.streamlitapp.com/) 📊

I designed the tool specifically for regression datasets in mind. I only chose a few charts because it was what I found useful for Feature Selection in Regression Machine Learning. I will add more charts if I find useful for Regression.    

Guide:
1. Upload the a CSV dataset (preferably a regression dataset)
2. After uploading, it will give a data preview of the first 50 rows of the dataset.
3. User *selects* a target variable for the rest of the analysis to be generated accordingly.
4. The system will provide descriptive statistics on the target variable. The descriptive variable consists of the count, mean, standard deviation, minimum and maximum value and the quartertiles percentage value range.
5. A **Histogram** will be displayed of the Target Variable so user check on the skewness.
6. A **Heatmap** will be generated to show the top 10 relationship value between independent variables and the target variable. The value closer to 1.00 indicates a stronger relationship.
7. User can *select* a multiple variables to generate **Scatter Plot** where it plots the variables selected against the target variables. This generally showcase where the values are clusters are at and also to find outliers.
8. User can *select* a multiple variables to generate **Box Plot** where it plots the variables selected against the target variables.
9. User can *select* a multiple variables to generate a **Histogram** and a probability plot. If histogram is skewed, we should generally perform a log transformation to have a normal distribution. 

