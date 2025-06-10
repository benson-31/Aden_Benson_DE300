## NUPD Data Engineering 300 Project
### Aden Benson, Rachel Silverman, Linda Liu, Harrison Gillespie

This is a readme.md file containing instructions on downloading the data and running the code for the NUPD Spring 2025 Data Engineering 300 group.

### Downloading Data
The dataset used for this project is the PADS - Parkinsons Disease Smartwatch dataset by Varghese et al. The link for downloading and exploring this dataset can be found here: https://physionet.org/content/parkinsons-disease-smartwatch/1.0.0/

To download, scroll to the bottom of the link pasted above. You'll see a section titled "Files", with a link that says "Download the Zip File". Click this link, and the database will begin downloading. 

Note: This is a very large dataset, and will need about 1.4 GB of storage. The download process may take close to an hour.

### Running the Code
In this Github, you'll see a file titled **final_rdd_imputation_classification.ipynb**. This contains all the source code for creating the relational database, completing imputation, and constructing a logistic regression model.
In the working directory for this file, the dataset downloaded above must be in an unzipped folder named 'pads-parkinsons-disease-smartwatch-dataset-1.0.0'. 
If this is correct, the .ipynb file will automatically read the data from this folder.

The following dependencies are required to run the source code:

- duckdb
- json
- pandas
- missingno
- scikit-learn
- os
- seaborn
- matplotlib

If the dataset is accurately placed inside the correct folder and the above dependencies are installed on the user's local machine, then the source code will successfully impute missing values into the PADS dataset, create a relational database structure in SQL, and perform logistic regression to predict whether a patient will develop PD in the future.
