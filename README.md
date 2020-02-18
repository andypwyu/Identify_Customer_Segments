# identify-customer-segments
Udacity Data Scientist Nanodegree Project 3 Identify Customer Segments

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*.

## Project Motivation<a name="motivation"></a>

This is the project of Term 1 Udacity Data Scientist Nanodegree. In this project, I applied unsupervised learning techniques to identify segments of the population that form the core customer base for a mail-order sales company in Germany. These segments can then be used to direct marketing campaigns towards audiences that will have the highest expected rate of returns.


## File Descriptions <a name="files"></a>

Identify_Customer_Segments.ipynb: showcase data processing and analysis of the project

Due to the sensitive and proprietary nature of the demographics data used in the project, the data will not be provided:
* Udacity_AZDIAS_Subset.csv: Demographics data for the general population of Germany; 891211 persons (rows) x 85 features (columns).
* Udacity_CUSTOMERS_Subset.csv: Demographics data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).
* Data_Dictionary.md: Detailed information file about the features in the provided datasets.
* AZDIAS_Feature_Summary.csv: Summary of feature attributes for demographics data; 85 features (rows) x 4 columns

## Results<a name="results"></a>

For cluster 1, which is overrepresented:

* Number of 6-10 family houses in the PLZ8 region is lower (PLZ8_ANTG3=1.16)
* Prosperous households (WEALTH=2.08)
* Estimated household net income is high income (HH_EINKOMMEN_SCORE = 2.39)
* In life stage of Families With School Age Children or Older Families & Mature Couples (LIFE_STAGE=3.63)
* Density of households per square kilometer is 150 - 319 households per km^2 (EWDICHTE = 3.93)
* Movement patterns is low(MOBI_REGIO = 4.17)
* Number of 1-2 family houses in the microcell is close to high share (KBA05_ANTG1 = 2.76)

Cluster 1 segment is company's target audiences, with a characteristic of higher income, family with children or mature couples, and stable in movement pattern.


For cluster 0, which is underrepresented:

* Number of 6-10 family houses in the PLZ8 region is between average and high (PLZ8_ANTG3=2.68)
* Less Affluent or poorer Households households (WEALTH=4.54)
* Estimated household net income is lower income (HH_EINKOMMEN_SCORE = 5.64)
* In life stage of Young Couples With Children (LIFE_STAGE=1.85)
* Density of households per square kilometer is 320 - 999 households per km^2 or more(EWDICHTE = 5.65)
* Movement patterns is high(MOBI_REGIO = 1.46)
* Number of 1-2 family houses in the microcell is close to no 1-2 family homes (KBA05_ANTG1 = 0.20)

Cluster 0 segment seems not to be company's audiences, with a characteristic of lower income, young couples, and easy to move.


## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Credits must be given to Udacity for providing starting code for this project. The data was provided by Udacity partners at Bertelsmann Arvato Analytics.
