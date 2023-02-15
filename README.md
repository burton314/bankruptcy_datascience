# bankruptcy_datascience


# Introduction

This repository contains a Jupyter notebook that analyzes company data from the Taiwan Economic Journal from the years 1999 to 2009 with regard to bankruptcy. The dataset, the analysis is based on, contains 6.819 entries (one row for each company) with 93 financial ratios (and 3 binary classifications). From the 6.819 companies, 220 were declared bankrupt (according to a definition of the Taiwanese stock exchange). The analysis is performed in Python.

# Research Question and Motivation:

The analyis mainly addresses 3 questions:

1. What financial ratios correlate (strongly) to the bankruptcy status?
2. What financial ratios correlate to each other for the bankrupt companies?
3. How do the finacial ratios from question 1 behave for the non-bankrupt companies in the dataset - compared to the bankrupt companies?

The motivation of this analysis was to determine whether financial ratios - as used daily for company performance evaluations - are good indicators for company bankruptcy. While the current analysis only examines the dataset statistically a future step would be to develop a regression model that predicts bankruptcy based on financial ratios as input parameters.


# Results:

1. Only 9 financial ratios correlate with the bankrupty status. Correlation is low (0.25 < abs(correlation) < 0.31. 5 negative and 4 positive correlations
2. The analysis found 60 very strong (>0.75) correlations between the different financial ratios for the bankrupt companies. However many ratios appear to depict
the same financial characteristic or vary only slightly from each other with regard to the used financial figures. 
3. While some of the found key ratios from question #1 differ significantly from the non-bankrupt companies, some show now real difference as it could have been
expected, e.g. with regard to company debt or liabilties.

# Repository Contents:

The repository only contains 1 Jupyter notebook ("Company_Bankrupty_Analysis.ipynb") and the image files generated in the notebook.

# Sources:

## Dataset

The dataset used is from Kaggle and is not included in the repository. The Link is as follows:

(https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction/download?datasetVersionNumber=2)

## Libraries used

In the Jupyter notebook I used the following libraries to help with the analysis:

    Numpy
    Pandas
    Seaborn
    Matplotlib (Pyplot)

## References for techniques used

To remove outliers, from some of the columns of the company dataset, I used a technique found on stackoverflow: (https://stackoverflow.com/questions/23199796/detect-and-exclude-outliers-in-a-pandas-dataframe)

For horizontal boxplots I used some techniques from: (https://seaborn.pydata.org/examples/horizontal_boxplot.html)

## Original research article mentioned in the dataset

Here is the original research article that developed a bankrupty prediction model: Liang D., Lu C.C., Tsai C.F., Shih G.A, Financial ratios and corporate governance indicators in bankruptcy prediction. A comprehensive study
European Journal of Operational Research 252 (2016), pp. 561-572