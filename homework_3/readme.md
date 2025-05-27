# HW3: MapReduce with Spark

## Note on Docker
The assignment requires that this code be run in an EC2 instance so a docker container can be constructed. However, I found that running this code on an EC2 instance was incredibly difficult, and all cells were run locally. I spent hours trying to convert my local code into EC2-friendly code that wouldn't crash my instance, but unfortunately AWS could not handle the large csv files used in this assignment. Each time I called .collect() or .show() after an operation, I would have to reboot my EC2 instance.

## Overview
This project implements MapReduce frameworks on two projects using Pyspark.

1. TF–IDF on the AG News dataset (“`agnews_clean.csv`”)  
   - Compute term frequencies (TF), document frequencies (DF), inverse document frequencies (IDF), and the final TF–IDF weights for each term in each document.
2. SVM Objective and Prediction
   - Implement the SVM loss entirely using MapReduce, and make predictions via a single map.
  
## Running the Code
All analysis is completed using the .ipynb file. The four .csv files used are described below.
1. agnews_clean.csv - Only file used for part 1, contains document numbers and a list of key words for each doc.
2. bias.csv - Singular float value for bias term in part 2.
3. w.csv - Vector of weights for loss term in part 2.
4. data_for_svm.csv - Large file containing data and features for linear regression in part 2.

To run the .ipynb file, the following modules must be installed.
1. Pyspark.sql.functions
2. Pyspark.sql.types
3. Numpy
4. Pandas
5. Operator

If all modules are installed and the four data files are placed in a folder labeled "dataset", the .ipynb file will successfully run.

## Expected Outputs
1. Part 1 - TF-IDF. Part 1 calculates the TF-IDF term for each document. The final output calculates the tf_idf measure for each term in the first five documents in our dataset.
2. Part 2 - SVM. Part 2 finds the loss term for our given data then predicts based on a y_hat function. The final output contains the objective value of our given data, the predictions using the y_hat function, and the loss function of our predictors.
