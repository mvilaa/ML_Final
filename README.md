# ML_Final

## Introduction
For this project the group analyzed the Red Wine Quaity dataset provided. The main goal of the analysis was to properly predict if a specific wine could be classified into "Good" wine or "Bad" wine. The outcome would be a binary classification for the dataset entires. 

## Exploratory Data Analysis (EDA)



## Algorithms

Logistic Regression - Marko Vila

Quadratic Discriminant Analysis? - Reily Siegel

K-Nearest Neighbors - Michael Zeolla

Artificial Neural Network - Drew Fisher


## K-Nearest Neighbors Analysis

First I load the data into R Studio to being analysis. 
The CSV file is loaded from my machine, and then the data heads are printed to confirm the data was correctly imported.

```
data_main = read.table("C://Users//mjzeo//OneDrive//Desktop/School//B Term 2021-2022//CS4342//Term Project//winequality-red.csv",sep=",",header=T)
head(data_main)
```
![image](https://user-images.githubusercontent.com/62816869/146108432-2f35ca8b-d207-4dad-bf2d-dfad65c03c9d.png)

Using the summary() function in R can report important values for the dataset. To get the perfect value in which to predict the different between "Good" and "Bad" wine summary can be used to calcualte the median and mean of the quality dataset. 
Furthermore, the table() function can produce how many different qualities there are in the data, and the number of wines that belong to each quality grouping.

```
summary(data_main$quality)
table(data_main$quality)
```
![image](https://user-images.githubusercontent.com/62816869/146109179-f3071863-6be7-416f-9600-e5cdc8cfcfb6.png)

