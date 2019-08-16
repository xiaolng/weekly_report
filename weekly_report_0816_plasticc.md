# Xiaolong - Week of 08/16/2019

## 1. Papers and code

### 1.1 Papers Read

[Models and Simulations for the PLAsTiCC](https://arxiv.org/abs/1903.11756): This article present the light curve models and the simulation method used to create the PLAsTicc datasets, which is the most comprehensive simulation of the transient and variable sky available at present.

[PLAsTiCC dataset](https://arxiv.org/abs/1810.00001): This paper describes the structure of training set and test set in details. 

### 1.2 Code Written

[plasticc_dataset.ipynb](https://github.com/xiaolng/weekly_report/blob/master/source/plasticc_dataset.ipynb): Explore the PLAsTicc dataset. The training set includes 7,848 objects and the test set includes 3,492,892 objects.


## 2. Figures

![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0816_plasticc_1.png?raw=true)

Figure 1: An example of light curve from plasticc train set. 


### 3. Results

I explored the simulated PLAsTicc dataset. PLAsTicc contains the train set (7,848 objects) and test set (3,492,892 objects). Next step is to inject this dataset to MAF and evaluate the performance of opsim databases.

