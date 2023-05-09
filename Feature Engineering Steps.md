# Feature Engineering Steps

- Firstly, we checked for the number of NaNs present in the dataset.
- We counted the frequency of the NaNs for all columns individualy.
- We calculated the 0.75th quantile for the number of NaNs.
- Then deleted the columns having NaN count more than the quantile.
- Now, we checked for the count of unique values present in independent columns.
- We can observe there are plenty of coolumns containing a single unique value.
- As these columns does not effect the dependent variable by any means, are dropped.
- Remaining missing data are imputed with the calculated mean for respective columns.
- As, the feature `var_5213` contains `Inf` values, the column is dropped.
