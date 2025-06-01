## Overview

This project involves data preprocessing and exploration on the Titanic dataset.

1️ Data Import and Exploration

The dataset was imported using pandas.
Initial data inspection included checking data types and viewing sample records.

2️ Handling Missing Values

Missing values in Age were filled using the median.
Missing values in Embarked were filled using the mode (most frequent category).
The Cabin column, which had too many missing values, was dropped.

3️ Encoding Categorical Variables

The Sex column was converted to binary (0 = male, 1 = female).
The Embarked column was one-hot encoded (with drop_first=True to avoid multicollinearity).

4️ Normalization / Standardization

Age and Fare columns were standardized using StandardScaler for better model performance.

5️ Outlier Detection and Removal

Boxplots were plotted for Age and Fare to visualize outliers.
Outliers were removed using the IQR method.
