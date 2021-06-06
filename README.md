# Give-me-some-credit-Kaggle
A project from Kaggle : Banks play a crucial role in market economies. They decide who can get finance and on what terms and can make or break investment decisions. For markets and society to function, individuals and companies need access to credit.   Credit scoring algorithms, which make a guess at the probability of default, are the method banks use to determine whether or not a loan should be granted. This competition requires participants to improve on the state of the art in credit scoring, by predicting the probability that somebody will experience financial distress in the next two years.

The project is devided into 4 parts:

## Data-preprocessing: 
 delete duplicates
 
 complement NANs
 
 delete outliers
 
 Balancing with SMOTE
 
## Feature-engineering:
  Binning: 
稀疏向量内积乘法运算速度快，计算结果方便存储，容易扩展；
离散化后的特征对异常数据有很强的鲁棒性：比如一个特征是年龄>30是1，否则0。如果特征没有离散化，一个异常数据“年龄300岁”会给模型造成很大的干扰；
单变量离散化后，每个变量有单独的权重，可以为逻辑回归模型引入了非线性，能够提升模型表达能力，加大拟合；
特征离散化以后，起到了简化了逻辑回归模型的作用，降低了模型过拟合的风险。
可以将缺失作为独立的一类带入模型。
  
  Choose valid features
  
  WOE-Encoding

## Training:
  LR
  
  RF
  
  XGBoost
 
## Evaluation:
  ROC, AUC

Since the test dataset is not labeled, there is no "real" evaluation part. What we can do is to split 30% of the data from the training dataset as testing dataset. Parameter still need to be fine tunned. The final AUC can reach up to 0.87 with XGBoost, 0.86 with LR and 0.84 with RF.
  
