# Graduate Characteristics and Labour Market Outcomes
Examining the Relationship Between Graduate Characteristics and Labour Market Outcomes Across Fields of Study

## Description
This project explores the relationship between graduates characteristics from the 2020 National Graduates Survey (NGS) by Statistics Canada with employment outcomes. Methods used include Latent Class Analysis and logistic regression in R, and random forest in Python.
### Background
### Modifications

## Data
Download the 202 NGS microdata file from statcan (https://www150.statcan.gc.ca/n1/pub/81m0011x/81m0011x2019001-eng.htm)


## LCA & Logistic Regression - Installation/Usage
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

For the logistic regression files, ensure that you download the imputed datasets from the imputed_data folder and change the pathnames accordingly for the imp_data variables within the code.


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
