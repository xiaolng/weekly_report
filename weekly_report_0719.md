# Xiaolong - Week of 07/05/2019

## 1. Papers and code

### 1.1 Papers Read

[A Smart and Colorful Cadence for Wide-Fast Deep Survey](https://arxiv.org/abs/1812.07036) : To ensure the efficient detection of TDEs in the LSST WFD survey, the cadence should be able to measure the u-r color evolution and catch the pre-peak light curve. This paper proposed a smart cadence that allows for efficient photometric transient classification. 

[TDEs with LSST](https://docushare.lsstcorp.org/docushare/dsweb/Get/Document-30574/bricman_tde_wfd.pdf):   This paper suggest that a WFD survey with 2 visits in different filters every night or at least every second night will increase the detection of TDEs. 

### 1.2 Code Written

[TDEs_v3.py](https://github.com/xiaolng/maf/blob/master/TDEs_v3.ipynb): Write a metric to evaluate the detection of TDEs. The structure of this metric is similar to [TransientAsciiMetric](https://github.com/LSST-nonproject/sims_maf_contrib/blob/master/mafContrib/transientAsciiMetric.py) but the condition parameters are different. It is specifically designed for the requirement that allows discrimination from supernova. 

It can be used to evaluate the 

- Total number of detections;
- Total number of filters;
- Number of detections before peak;
- Number of detections near peak for each band;
- Number of filters near peak;
- Number of detections post peak.
- And more...

## 2. Figures



![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0719_tdes.png?raw=true)

Figure 1:  The simulated light curve and fiveSigmaDepth (m5) of baseline operation in *r* band. The  points above m5 line are considered as detected.

![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0719_tdes_2.png?raw=true)

Figure 2: Results from baseline operation within first 700 days. 

### 3. Results

I write a metric class *TDEsMetricTest* to evaluate the detection of TDEs using simulated light curve. It can be used to put requirements on the number of observations/filters at prePeak/nearPeak/postPeak. Need to write better document for each  parameters and make it robust enough.