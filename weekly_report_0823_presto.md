# Xiaolong - Week of 08/23/2019

## 1. Papers and code

### 1.1 Papers Read

[Models and Simulations for the PLAsTiCC](https://arxiv.org/abs/1903.11756): This article present the light curve models and the simulation method used to create the PLAsTicc datasets, which is the most comprehensive simulation of the transient and variable sky available at present.

[PLAsTiCC dataset](https://arxiv.org/abs/1810.00001): This paper describes the structure of training set and test set in details. 

[Presto-Color: A Photometric Survey Cadence for Explosive Physics and Fast Transients](https://arxiv.org/abs/1812.03146): This paper proposed a cadence to identify fast transients:

- Observations in two filters within 0.5hr;
- A same filter revisit separated by hours. 

### 1.2 Code Written

[presto_color.ipynb](https://github.com/xiaolng/weekly_report/blob/master/source/presto_color.ipynb): Run the *threeVisitsWColorMetric* and *FastTransientMetric*  on baseline2018.db and presto.db. 


## 2. Figures

![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0823_cadence_highlevel.png?raw=true)

Figure 1. Cadence of presto-color. Two visits in different filters within $\Delta T_1$, and same filter revisit within $\Delta T_2$.

![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0823_3visits_baseline2018a.png?raw=true)

Figure 2. Results of threeVisitsWColorMetric from baseline2018.db.

![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0823_3visits_pontus_gi.png?raw=true)

Figure 3. Results of threeVisitsWColorMetric from presto.db.

![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0823_kn_lc.png?raw=true)

Figure 4. An example of kilonova light curve.

![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0823_LSST_PhaseSpace.png?raw=true)

Figure 5. The distribution in phase space of different kinds of light curves.

### 3. Results

I explored code the used in the paper [*Presto-Color*](https://arxiv.org/abs/1812.03146) and use them to recreated the figures.  I run the *threeVisitsWColorMetric* and *FastTransientMetric*  on baseline2018.db and presto.db.  And also study the distribution of different kinds of light curves in phase space. 

