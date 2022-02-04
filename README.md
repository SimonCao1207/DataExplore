# Exploratory data analysis with COMPAS and AdultCensus datasets.

## COMPAS dataset

- My effort is to preprocess and clean the data similar to the method of IBM's AI Fairness 360 including filtering missing data, dropping irrelevant columns, explore new informative features.

- For generation of poisoned data, I poison about 10% of the training data by flipping the labels of examples that belong to a specific z attribute (for this experiment z = 1) so as to maximize the accuracy performance degradation


## Adult Census dataset

2 experiments:
- Using PCA to reduce the dimensions required from 14 to 12.
- Making use of the crowdsourcing data (by following the features selection used by crowdsourcing data) and try to construct a validation set.

## Run experiments on FR-train

![Result from paper](./img/result.png)

- Run with real data from COMPAS dataset

Accuracy : 0.654, Disparate Impact : 0.955

- Run with real data from Adult Cencus dataset (without clean validation set)

Accuracy : 0.822, Disparate Impact : 0.925

- Run with real data from Adult Cencus dataset (with crowdsouring validation set)

Accuracy : 0.791, Disparate Impact : 0.838 




## Reference
- [fr-train](https://github.com/yuji-roh/fr-train.git)
- [Propublica repo](https://github.com/propublica/compas-analysis)



