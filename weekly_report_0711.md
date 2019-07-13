# Xiaolong - Week of 07/05/2019

## 1. Papers and code

### 1.1 Papers Read

[Neural Network Learning](https://www.holehouse.org/mlclass/09_Neural_Networks_Learning.html): The notes from cs229 taught by Andrew Ng, 

### 1.2 Code Written

[nn_2_layers.py](https://github.com/xiaolng/weekly_report/blob/master/source/nn_2_layers.ipynb): Build a simple two layers neural network and use it as a classifier. The forward and backward propagations are achieved by gradient decent method.

## 2. Figures

![](https://raw.githubusercontent.com/xiaolng/weekly_report/master/imgs/nn_2_layers_cost.png)

Figure 1:  The cost function is decreasing  with iterations .

![](https://raw.githubusercontent.com/xiaolng/weekly_report/master/imgs/nn_2_layers_pred.png)

Figure 2: The right image shows the true data structure, the left is the prediction from  the neural network.

### 3. Results

I build a neural network classifier with 2 hidden layers. I  apply basic  gradient decent  method to do the forward propagation and backward propagation. The predictions are similar to the true data. Need to evaluate  the model use more data and optimize the algorithm.