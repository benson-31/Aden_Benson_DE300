# Homework 1 - DE300
#### Name: Aden Benson, Course: Data Engineering 300, Assignment: Homework 1, Due Date: April 17, 11:59PM

## Description
In this homework, we explore the aircraft inventory dataset from 2006 to 2023 (Source: Bureau of Transportation Statistics, www.bts.gov).

## Contents
This folder contains my submission for homework 1. The components include:
- 'benson_hw1.ipynb' - Jupyter notebook file containing code, vizualizations, and some comments in Markdown.
- 'benson_hw1.pdf' - Document containing analysis and written answers for all questions.
- 'readme.md' - This file.

## Instructions to Run the Code
1. **Download the Dataset**:
   The dataset can be downloaded [here](https://canvas.northwestern.edu/courses/230993/files/21744819?wrap=1). Once the dataset is downloaded, unzipped, and
   placed in the same folder as the .ipynb file, it will be compatible with our submission. The dataset can be explored [here](https://www.transtats.bts.gov/Fields.asp?gnoyr_VQ=GEH).
2. **Running the Code**:
   Once the dataset is placed in the same folder as the .ipynb file, the code can be run using Colab, Jupyterlab, VScode, etc.
   NOTE: The following modules must be installed (Pandas, Numpy, Matplotlib, sklearn.impute, scipy.stats).
   
## Expected Ouputs
When the notebook is ran, it produces the following outputs:
1. **Missing Data Imputation**:
   Imputed missing values for columns CARRIER, CARRIER_NAME, MANUFACTURE_YEAR, NUMBER_OF_SEATS, CAPACITY_IN_POUNDS, and AIRLINE_ID.
2. **Column Transformation and Standardization**:
   Standardized messy entries in columns MANUFACTURER, MODEL, AIRCRAFT_STATUS, and OPERATING_STATUS.
3. **Derivative Variables**:
   Checked skewness of NUMBER_OF_SEATS and CAPACITY_IN_POUNDS, applixed boxcox transformation to normalize both columns.
4. **Feature Engineering**:
   Created a new column SIZE, attaching a qualitative value to the quantitative column NUMBER_OF_SEATS.
5. **Visual Outputs**:
   Histograms were created before and after boxcox transformation for NUMBER_OF_SEATS and CAPACITY_IN_POUNDS. Proportions were plotted for SIZE column against OPERATING_STATUS and AIRCRAFT_STATUS.

These ouputs are all shown in the .ipynb file.

## Authors
Aden Benson, student at Northwestern University (adenbenson2026@u.northwestern.edu)
