"# bankruptcy_datascience"


Introduction

#######################################

This repository contains a Jupyter notebook that analyzes company data from the Taiwan Economic Journal from the years 1999 to 2009 with regard to bankrupty. The dataset, the analysis is based on, contains 6.819 entries (one row for each company) with 93 financial ratios (and 3 binary classifications). From the 6.819 companies, 220 were declared bankrupt (according to a definition of the Taiwanese stock exchange). The analysis is performed in Python.
Research Question and Motivation:

The analyis mainly addresses 3 questions:

1. What financial ratios correlate (strongly) to the bankruptcy status?
2. What financial ratios correlate to each other for the bankrupt companies?
3. How do the finacial ratios from question 1 behave for the non-bankrupt companies in the dataset - compared to the bankrupt companies?

The motivation of this analysis was to determine whether financial ratios - as used daily for company performance evaluations - are good indicators for company bankruptcy. While the current analysis only examines the dataset statistically a future step would be to develop a regression model that predicts bankruptcy based on financial ratios as input parameters.


Results:

#######################################


Repository Contents:

#######################################

The repository only contains 1 Jupyter notebook ("Company_Bankrupty_Analysis.ipynb") and the image files generated in the notebook.

Sources:

#######################################

The dataset used is from Kaggle and is not included in the repository. The Link is as follows:

https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction/download?datasetVersionNumber=2

===

In the Jupyter notebook I used the following libraries to help with the analysis:

    Numpy
    Pandas
    Seaborn
    Matplotlib (Pyplot)

===

To remove outliers, from some of the columns of the company dataset, I used a technique found on stackoverflow: https://stackoverflow.com/questions/23199796/detect-and-exclude-outliers-in-a-pandas-dataframe