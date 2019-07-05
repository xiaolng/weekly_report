# Xiaolong - Week of 07/05/2019

## 1. Papers and code

### 1.1 Papers Read

[A Smart and Colorful Cadence for Wide-Fast Deep Survey](https://arxiv.org/abs/1812.07036) : To ensure the efficient detection of TDEs in the LSST WFD survey, the cadence should be able to measure the u-r color evolution and catch the pre-peak light curve. This paper proposed a smart cadence that allows for efficient photometric transient classification. 

[TDEs with LSST](https://docushare.lsstcorp.org/docushare/dsweb/Get/Document-30574/bricman_tde_wfd.pdf):   This paper suggest that a WFD survey with 2 visits in different filters every night or at least every second night will increase the detection of TDEs. 

### 1.2 Code Written

[TDEs.py](https://github.com/xiaolng/maf/blob/master/TDEs.ipynb): explore the detection of TDEs using TransientAsciiMetric combined with UserPointSlicer and HealPixerSlicer. 

## 2. Figures



![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0705_1.png?raw=true)

Figure 1:  The light curve of a TDE event in three bands *i, g, r*.

![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0705_2.png?raw=true)

Figure 2: The detection of TDEs from the baseline operation of LSST. This indicates baseline operation is not optimized for the detection of TDEs.

### 3. Results

I evaluate the detection of TDEs using its light curve and  TransientAsciiMetric.  The result from baseline operation of LSST shows that it fails to detect TDEs efficiently.  Two cadences that will increase the detection of TDEs are proposed in the white paper.  Need to evaluate  the importance of other properties mentioned in the paper.
