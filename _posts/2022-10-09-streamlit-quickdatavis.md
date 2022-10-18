---
layout: post
title: Automated Exploratory Data Analysis Tool For Regression Dataset
---

{{ page.title }}
================

<p class="meta">09 Oct 2022</p>

For the regression machine learning exercises, the process of the Exploratory Data Analysis(EDA) have been a bit repetitive for me for the most part. So why not create an automated tool for quick EDA. I've deployed a working prototype [https://heyfasteda.streamlitapp.com/](https://heyfasteda.streamlitapp.com/) hosted on the free version of the Streamlit Community Cloud services. 

The App is quite intuitive to use for a regression dataset. You require a csv file upload, then select target variable and independent variables. Voila! It will generate an interactive data visualization set.   

I'm still currently adding more EDA features onto it such as a data cleaning features, categorical features, machine learning library and model evaluation.  

I was inspired by an Author from Kaggle where he provided an EDA on the [House Prices](https://www.kaggle.com/code/pmarcelino/comprehensive-data-exploration-with-python). He goes through the EDA in an entertaining fashion which I would recommend anyone interested in EDA to read.  

Here's my take on the EDA process for a Regression Dataset:
1. Import the CSV file
2. The first portion is to analyze the output data column which has various names (Target Variable or Dependent Variable or Labels).
3. Find out if the target variable's minimum value is not less than zero as it will break the model.
4. Plot a Histogram on what kind of distribution it has.
5. Plot a Heat Map to find out the strongest numerical relationship between the Dependent Variable and the Independent Variables. 
6. The second portion is to analyze the independent variable. After finding the strongest relationship, plot a Scatter plot to ensure that there is a linear relationship between the Dependent Variable and the Independent Variable. 
7. Check for any missing data. (Rule of thumb: Drop variable with more than 15% data missing).
8. For outliers, standardize the data and drop any outliers where necessary as it may not represent the dataset. 
9. For normality, we plot the histogram. As there is a portion of the values being zero, we have to perform a log transformation without losing the zero values.   
10. Using a scatter plot, find out to see if there is a strong linear relationship with the dependent variables. 
