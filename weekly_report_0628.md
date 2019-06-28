# Xiaolong - Week of 06/28/2019

## 1. Papers and code

### 1.1 Papers Read

[Probabilistic Programming in Python using PyMC](https://arxiv.org/abs/1507.08050) :  A step-by-step guide to do model fitting by  pymc3. 

[TDE](https://docushare.lsstcorp.org/docushare/dsweb/Get/Document-30574/bricman_tde_wfd.pdf):  Disscuss the requirements for LSST to detect TDEs. 

### 1.2 Code Written

[sn_Pymc.py](https://github.com/xiaolng/maf/blob/master/sn_Pymc.ipynb): learn to use pymc3 and fit two models of supernova light curve. 



## 2. Figures



![](https://raw.githubusercontent.com/xiaolng/weekly_report/master/imgs/snmcfit.png)

Figure 1: Curve fitting for light curve of Type  IIp supernova from pymc3. Created by  [sn_Pymc.py](https://github.com/xiaolng/maf/blob/master/snModel.ipynb). 



![](https://raw.githubusercontent.com/xiaolng/weekly_report/master/imgs/snpymc.png)

Figure 2: Fitting results  for light curve of Type IIp supernova from pymc3. Created by [sn_Pymc.py](https://github.com/xiaolng/maf/blob/master/snModel.ipynb). 



### 3. Results

I fit two models of supernova light curve by pymc3. Results are similar from scipy.curve_fit for 3-parameter model. But for 6-parameter model, result from pymc3 is more reasonable. 

To evaluate the performance of LSST detect TDEs,  we can use the same metrics as for transients.  Need to figure out how TDEs different from other transients.