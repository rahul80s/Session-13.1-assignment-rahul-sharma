# Session-13.1-assignment-rahul-sharma
Acadgild session 13.1 assignment 

1. Use the given link dataset. 

Answer the below questions:

a. Find out top 5 attributes having highest correlation (select only numeric features). 

b. Find out top 3 reasons for having more crime in a city. 

c. Which all attributes have correlation with crime rate? 

Ans 1 a. - >

library(mlbench)

library(caret)

data(Yeast)

correlationMatrix <- cor(Yeast[,1:5])

print(correlationMatrix)

highlyCorrelated <- findCorrelation(correlationMatrix, cutoff=5)

print(highlyCorrelated)

Ans 1 b. ->
