# Xiaolong - Week of 07/26/2019

## 1. Papers and code

### 1.1 Papers Read

[A Smart and Colorful Cadence for Wide-Fast Deep Survey](https://arxiv.org/abs/1812.07036) : To ensure the efficient detection of TDEs in the LSST WFD survey, the cadence should be able to measure the u-r color evolution and catch the pre-peak light curve. This paper proposed a smart cadence that allows for efficient photometric transient classification. 

[TDEs with LSST](https://docushare.lsstcorp.org/docushare/dsweb/Get/Document-30574/bricman_tde_wfd.pdf):   This paper suggest that a WFD survey with 2 visits in different filters every night or at least every second night will increase the detection of TDEs. 

### 1.2 Code Written

[TDEsDb.py](https://nbviewer.jupyter.org/github/xiaolng/maf/blob/master/TDEsDb.ipynb): Compare the performance of six opsim databases for detection of TDEs.  Both skymap and the light curve can be obtained. 

## 2. Figures

![0726_tdelc.png](https://github.com/xiaolng/weekly_report/blob/master/imgs/0726_tdelc.png?raw=true)

Figure 1:  A detected light curve from opsim database.  It meets the minimum requirements: one detection before peak, three filters near peak, and two filters post peak within two weeks.



![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0726_dbCompare.jpeg?raw=true)

Figure 2: Results from baseline operation within first two years. Pontus_2573 has the best performance.  

### 3. Results

I write a metric class *TDEsMetricTest* to evaluate the detection of TDEs using simulated light curve. It can be used to put requirements on the number of observations/filters at prePeak/nearPeak/postPeak. I use it to compare six opsim databases and find that pontus_2573.db has the best performance.  This is because it operates with mixed-filter pairs therefore  has large probability to meet the filter requirements.
