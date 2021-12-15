# Machine Learning Final Project
By: Michael Zeolla, Andrew Fisher, Marko Vila and Reily Siegel

## Introduction
For this project the group analyzed the Red Wine Quaity dataset provided. The main goal of the analysis was to properly predict if a specific wine could be classified into "Good" wine or "Bad" wine. The outcome would be a binary classification for the dataset entires. 

## Exploratory Data Analysis (EDA)

First the data is loaded into R Studio to being analysis. 
The CSV file is loaded from the computer, and then the data heads are printed to confirm the data was correctly imported.

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
![image](https://user-images.githubusercontent.com/62816869/146109642-b465bf72-060f-413a-b8e0-181b05ad58c1.png)

Based on the results it is clear there is only 6 different quality groupings despite there being values allowed between 3 and 10.
The largest groupings are 5 and 6 which hold majority of the data entries.
The best split of the data is likely 5.5, which is around the mean of the quality predictor.

The next best step would be to analyze the coorelation between each of the predictors and the outcome. Depedning on the correlation of the data
specific predictors can be removed to prodcuce a more accurate model. 

```
corrplot(cor(data_main))
cor(data_main)
```

![image](https://user-images.githubusercontent.com/62816869/146109868-93bd7348-563a-4251-a0e6-c895b58b9f57.png)
![image](https://user-images.githubusercontent.com/62816869/146109878-c95ae9c1-6fd1-4529-b2e3-2ee3e3b09c06.png)

## Algorithms

Logistic Regression - Marko Vila

Quadratic Discriminant Analysis? - Reily Siegel

K-Nearest Neighbors - Michael Zeolla

Artificial Neural Network - Drew Fisher


## K-Nearest Neighbors Analysis



