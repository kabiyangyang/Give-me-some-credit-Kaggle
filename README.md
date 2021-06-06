# Give-me-some-credit-Kaggle
A project from Kaggle : Banks play a crucial role in market economies. They decide who can get finance and on what terms and can make or break investment decisions. For markets and society to function, individuals and companies need access to credit.   Credit scoring algorithms, which make a guess at the probability of default, are the method banks use to determine whether or not a loan should be granted. This competition requires participants to improve on the state of the art in credit scoring, by predicting the probability that somebody will experience financial distress in the next two years.

The project is devided into  parts:

## Data-preprocessing: 
 delete duplicates
 complement NANs
 delete outliers
 Balancing with SMOTE
 
## Feature-engineering:
  Binning
  Choose valid features
  WOE-Encoding

## Training:
  LR
  RF
  XGBoost

Parameter still need to be fine tunned. The final AUC can reach up to 0.87 with XGBoost, 0.86 with LR and 0.84 with RF.
  
