# Some General concepts
- Univariant vs MultiVariant TSA (Time Series Analysis?)
  So far we are interested in predicting the energy consumption, therefore we deal with only Univariant TSA.
- In a multivariant TSA, you model the dynamics of a series itself but also the interdependence among the series.

- VAR (Vector autoregression) models applies only to stationary series.
Non stationary series can be converted to stationary using simple differencing.

# Data source and preprocessed source
- Original data source: [click here](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)
- Preprocessed data source: To be found on server under the name: `time_series_single_household.csv`

Tasked Performed:
1. Explore and implementation feature engineering trick to solve the problem using linear regression instead of RNN/LSTM.
   Advantages: 
   - Using linear regression you can explain to the production team if anything goes wrong.
   - You have better interpretability in this case.
2. Idea: Use a different basis for feature engineering (maybe cycloid function?)
