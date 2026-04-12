# Graduate Characteristics and Labour Market Outcomes
Examining the Relationship Between Graduate Characteristics and Labour Market Outcomes Across Fields of Study

## Description
This project explores the relationship between graduates characteristics from the 2020 National Graduates Survey (NGS) by Statistics Canada with employment outcomes. Methods used include Latent Class Analysis and logistic regression in R, and random forest in Python. 

The LCA focuses on all bachelor's graduates, while the logistic regression and random forest focus on the three largest fields of study (Business, Health, Law and Social Sciences).

### Background
Given that employment is top of mind for many students, our aim is to examine what graduate characteristics, if any, are relevant and can help predict an undergraduate’s employability in Canada. Additionally, a key motivation is to address the less explored area of segmented analysis by field of study.

## Data
Download the 202 NGS microdata file from statcan (https://www150.statcan.gc.ca/n1/pub/81m0011x/81m0011x2019001-eng.htm)

## html version of R files
Download and open the html files in the R_file_html_version folder to view results without executing the R code.


## LCA - Installation/Usage
Install R

### Packages
```bash
install.packages("dplyr")
install.packages("naniar")
install.packages("VIM")
install.packages("mice")
install.packages("ggplot2")
install.packages("patchwork")
install.packages("poLCA")
install.packages("survey")
install.packages("car")
install.packages("pROC")
install.packages("caret")
install.packages("Metrics")
```

### Execution
Go through the code and change pathnames for the ngs microdata csv file.

Either download the imputed data from the imputed_data folder, or run the R-code to execute the multiple imputation with MICE and generate the imputed datasets.


## LCA Analysis - Installation/Usage
Install python
### Packages
```bash
pip install pandas numpy
pip install matplotlib seaborn
pip install ipython jupyterlab notebook
```
### Execution
Export the lca_data results from the LCA R code, as a csv. Read in this csv in the first code block of python notebook.

## Logistic Regression - Installation/Usage
Install R

### Packages

```bash
install.packages("dplyr") 
install.packages("mice")
install.packages("car") 
install.packages("pROC") 
install.packages("caret")
install.packages("Metrics") 
install.packages("survey") 
```

### Execution
Go through the code and change pathname for the ngs microdata csv file.

Ensure that you download the imputed datasets from the imputed_data folder and change the pathnames accordingly for the five imp_data variables within the code. 

Do this for each logistic regression file across the three fields of study.

## Random Forest - Installation/Usage
Install Python

### Packages
```bash
pip install pandas numpy statsmodels
pip install scikit-learn
pip install matplotlib seaborn
pip install ipython jupyterlab notebook
```

### Execution

Download the five csv files contain the imputed data with weights in the imputed_data_with_weights folder, or run the R-code for imputation and joining with weights, and export results to csv.

Change filepath for the five csv files at the top of the code.




## References
Statistics Canada. (2024, March 22). National Graduates Survey (NGS). https://www23.statcan.gc.ca/imdb/p2SV.pl?Function=getSurvey&Id=1496497
