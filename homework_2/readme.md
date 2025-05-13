## Running the Code
All analysis is completed using the .ipynb file. The seven .csv code files are all held in the hw2_data folder, descriptions shown below.
1. ADMISSIONS.csv — patient admission details
2. ICUSTAYS.csv — ICU stay records
3. PATIENTS.csv — patient demographics
4. PROCEDURES_ICD.csv — ICU procedure codes
5. D_ICD_PROCEDURES.csv — mapping of ICD procedure codes to short title)
6. DRGCODES.csv — DRG code descriptions
7. PRESCRIPTIONS.csv — medication orders

To run the .ipynb file, the following modules must be installed.
1. duckdb
2. pandas
3. Cassandra.cluster
4. ssl
5. cassandra_sigv4.auth
6. boto3
7. uuid
8. csv
9. numpy

If all modules are installed and all datafiles are downloaded (either through the github folder or through MIMIC-III) then the docker container can be run, showing all outputs.

## Expected Outputs
1. Part 1 - Relational Databases. Part 1 will use duckdb to generate sql outputs for the three analysis questions below
- Analysis Question 1: Create a summary of type of drugs and their total amount used by ethnicity. Report the top usage in each ethnicity group.
- Analysis Question 2: Create a summary of procedures performed on patients by age groups (<=19, 20-49, 50-79, >80). Report the top three procedures, along with the name of the procedures, performed in each age group.
- Analysis Question 3: How long do patients stay in the ICU? Is there a difference in the ICU length of stay among gender or ethnicity?
2. Part 2 - Nonrelational Databases. Part 2 uses Nosql in Cassandra to analyze the same 3 analysis questions as above.
