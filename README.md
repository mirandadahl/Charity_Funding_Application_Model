# deep-learning-challenge

Analysis:

The purpose of this analysis was to develop a predictive model that can determine whether applicants for charitable organizations are likely to have their funding applications approved or denied. 

Data Preprocessing
In the initial phase of analysis, the dataset was imported and cleaned. Non-beneficial columns, such as 'EIN' and 'NAME', were dropped from the dataset.

Binning of 'APPLICATION_TYPE' - The 'APPLICATION_TYPE' column was analyzed, and a cutoff value of 500 was chosen. Application types with counts below this threshold were grouped into an 'Other' category.

Binning of 'CLASSIFICATION' - A similar approach was applied to the 'CLASSIFICATION' column, where a cutoff value of 100 was chosen. Classifications with counts below this threshold were grouped into an 'Other' category.

Conversion to Numeric Data
To make the data suitable for machine learning, the categorical columns 'APPLICATION_TYPE' and 'CLASSIFICATION' were transformed into numerical data using one-hot encoding. This process created binary columns for each category within these columns.

Results

Model Loss: 0.539
Model Accuracy: 0.734

Summary

The model achieved an accuracy of approximately 73.4% on the test data, which is close to its training accuracy. Feature importance analysis can be conducted to identify the key factors influencing the model's prediction. Model performance can potentially be improved by collecting more relevant features or testing different data preprocessing techniques. Alternative models could be conseidered. The choice of model would depend on factors such as dataset size, feature types, etc.

