# Introduction

This project consists of five classes:

## Class I : HouseObjectOriented Class.
1) Adds the data to the object.
2) Concats the data in one DataFrame.
3) Shows information about the data.
4) Preprocess the data before ML part.
5) Adds the data after Preprocessing for the ML part.

## Class II : Information Class.
1) Calculates the missing values.
2) Gets feature dtypes.
3) Gets feature names.
4) Gets shape of the data.
5) Prints all of these information.

## Class III : Pre-processing Class.
1) Drops the unwanted columns and rows.
2) Fills the null values with (mean, meadian, zero,....etc).
3) Applys feature engineering to the data like adding new columns, transforming columns,...etc.
4) Encodes the data using label encoder to be able to apply ML algorithms.
5) Converts your data to dummies values.
6) Normalizes the data before ML.

## Class IV : Preprocessor Class
1) Applys the Pre_processing techniques and returns the new data.

## Class V : ML Class
1) Initializes the ML algorithms.
2) Show the available ML algorithms.
3) Applys Train-Test evaluation and shows the results.
4) Applys Cross-Validation evaluation and shows the results.
5) Visualizes the results of Train-Test and Cross-Validation evaluations.
6) Find the best model and then fits it to the data.
7) Show the Predictions in a DataFrame.
8) Save the predictions to a csv file.
