- Univariant vs MultiVariant TSA (Time Series Analysis?)
  So far we are interested in predicting the energy consumption, therefore we deal with only Univariant TSA.
- In a multivariant TSA, you model the dynamics of a series itself but also the interdependence among the series.

- VAR (Vector autoregression) models applies only to stationary series.
Non stationary series can be converted to stationary using simple differencing.

Task Proposal:
1. Explore feature engineering trick to solve the problem using linear regression instead of RNN/LSTM.
   Using linear regression you can explain to the production team if anything goes wrong.
   You better interpretability in this case.
2. What kind of transformation can be used? cycloid
