# Xiaolong - Week of 08/02/2019

## 1. Papers and code

### 1.1 Papers Read

[TDEs with LSST](https://docushare.lsstcorp.org/docushare/dsweb/Get/Document-30574/bricman_tde_wfd.pdf):   This paper suggest that a WFD survey with 2 visits in different filters every night or at least every second night will increase the detection of TDEs. 

[Presto-Color: A Photometric Survey Cadence for Explosive Physics and Fast Transients](https://arxiv.org/abs/1812.03146): This paper proposed a cadence to identify fast transients:

- Observations in two filters within 0.5hr;
- A same filter revisit separated by hours. 

### 1.2 Code Written

[TDEsMonteMetric.py](https://github.com/xiaolng/maf/blob/master/TDEsMonteMetric.py): Source code of TDEsMonteMetric, which evaluate the detection of TDEs using Monte Carlo method.

[TDEsMonteMetric.ipynb](https://github.com/xiaolng/maf/blob/master/TDEsMonteMetric.ipynb): Introduction to running TDEsMonteMetric and analyzing the output result.

[TDEsMonteDbCompare.ipynb](https://github.com/xiaolng/maf/blob/master/TDEsMonteDbCompare.ipynb): Compare the performance of six opsim databases for detection of TDEs using TDEsMonteMetric.

## 2. Figures



![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0726_dbCompare.jpeg?raw=true)

Figure 1: Results from baseline operation using TDEsAsciiMetric within first two years. Pontus_2573 has the best performance.  



![0802_db_tdemc.png](https://github.com/xiaolng/weekly_report/blob/master/imgs/0802_db_tdemc.jpeg?raw=true)

Figure 2:  Results from baseline operation using TDEsMonteMetric within first two years. Same as above, pontus_2573 has the best performance. 

![0802 lc.png](https://github.com/xiaolng/weekly_report/blob/master/imgs/0802_lc.png?raw=true)

Figure 3: An detected light curve from pontus_2573. Pontus_2573 has many detections with paired filters, thus it is the best one to observe transients.


## 3. Results

I wrote two metric class *TDEsAsciiMetric* and *TDEsMonteMetric* to evaluate the detection of TDEs from simulated light curve. Both metric can be used to put requirements on the number of observations/filters at prePeak/nearPeak/postPeak. TDEsAsciiMetric injects continuous saw-tooth shaped transients into sky, while TDEsMonteMetric using a Monte Carlo approach, i.e, injects light curve at times  randomly selected from a Poisson distribution. I use them to compare six opsim databases and find that pontus_2573.db has the best performance from both metrics. Also  Monte Carlo approach is more precise and similar to real scenario. 
