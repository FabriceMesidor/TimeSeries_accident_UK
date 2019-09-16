# An analysis of daily accidents in UK from 2014 to 2017 using Time Series
     A simple time series regression to understand the different steps of modeling

## Introduction

Linear regression is a very common model used by Data Scientist. An outcome or target variable is explained by a set of features. There is a case where the same variable is collected over time and we used a sequence of measurements of that variable made at regular time intervals. Welcome to Time Series. One difference from standard linear regression is that the data are not necessarily independent and not necessarily identically distributed. Working with time series can be frustrating as it implies that you have to find a correlation between the lag or errors of any previous prediction of the value and itself. Also, the ordering matters and changing the order will change the meaning of the data. Due to its complexity, Data Scientist got lost sometimes in the process of times series analysis. In this blog, I am going to share a full time series analysis guided by one of the well known Data Science methods: OSEMIN.


## Context and Data used

The visual above shows the methodology used in my study from gathering the data to drawing conclusions.
The data used for this analysis contained the date and amount of 1461 daily accidents in the UK from January 1st, 2014 to December 31, 2017. I used a dataset from from kaggle for this exercise. I downloaded an CSV file and used a popular python code 'pd.read_csv' to store it into a Data Frame. No other independent variables were considered in this analysis as I am focused on the time series.
The main purpose of this study is to explain the different steps of a full data science project. Other objectives are to find out if the number of accidents in a day is dependent of the number of accidents in any given day.
The 3 questions that the study is seeking to answer are:
What is the relation between the amount of accident on a current day and the day prior?
Is there any pattern that can help predict (or prevent) the amount of accident in UK on any given day?
Is the month of the year or day of week related to the number of accident during that month?

### Description of the data

![Data Sample](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/sample%20data.png)

![Stats](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/Stats.png)

## Graphs and models

![Daily Trends of accidents in UK](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/daily%20trends.png)

![Daily Trends of accidents in UK - dot](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/trends%20dot.png)

![Monthly Trends of accidents in UK](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/monthly%20trends.png)

![Weekly Trends of accidents in UK](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/weekly%20trends.png)

![Boxplot](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/boxplot.png)

![Histogram](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/histogram.png)

![KDE](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/kde%20normal.png)

![acf](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/acf.png)

![pacf](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/pacf.png)

![model](https://github.com/FabriceMesidor/TimeSeries_accident_UK/blob/master/Graphs/arma.png)


