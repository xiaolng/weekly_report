# Xiaolong - Week of 06/19/2019

## 1. Papers and code

### 1.1 Papers Read

[Classical Statistical Inference](https://www.jstor.org/stable/j.ctt4cgbdj) :  Chapter 4 from the book [*Statistics, Data Mining, and Machine Learning in Astronomy*](https://www.jstor.org/stable/j.ctt4cgbdj). Discuss the maximum likelihood estimation, the goodness of fit,  model selection and hypothesis testing.

 [The Diverse Science Return from a Wide-Area Survey of the Galactic Plane](https://arxiv.org/abs/1812.03137):  LSST will make contributions to the astrophysics discovery by conducting a wide-area survey of the Galactic Plane. This article discusses the importance of various survey strategy constraints and proposed some metrics to evaluate the performance of LSST.

### 1.2 Code Written

[snModel.py](https://github.com/xiaolng/maf/blob/master/snModel.ipynb) : compare two models with different parameters for the light curve of supernova. One model has three parameters, another has six parameters.  Data from Type Ia and IIp supernovas are considered.

[wp12.py](https://github.com/xiaolng/maf/blob/master/wp12.ipynb):  explore some metrics proposed in the white paper [*The Diverse Science Return from a Wide-Area Survey of the Galactic Plane*](https://arxiv.org/abs/1812.03137). For example, the NRevisitsMetric calculate the number of consecutive visits with time differences less than dT. 



## 2. Figures



![](https://github.com/xiaolng/weekly_report/blob/master/imgs/snia.png?raw=true)

Figure 1: Curve fitting for light curve of Type Ia supernova.



![](https://github.com/xiaolng/weekly_report/blob/master/imgs/snlc.png?raw=true)

Figure 2: Curve fitting for light curve of Type IIp supernova.



![](https://raw.githubusercontent.com/xiaolng/weekly_report/master/imgs/nRvisits.png)

Figure 3: Number of revisits faster than 30 minutes. 

### 3. Results

I compare the likelihoods of two models of supernova light curves. Based on the model selection described in [chapter 4](https://www.jstor.org/stable/j.ctt4cgbdj), model with 3 parameters is a better choice.  Need to figure out how to calculate the standard deviation used in the likelihood ratio test and how to intemperate the results.

The plot from NRevisitsMetric shows that Baseline Opsim database is not optimized for faster revisits  of the Galactic Plane.

