# Xiaolong - Week of 08/30/2019

## 1. Papers and code

### 1.1 Papers Read
[Generative Adversarial Networks](https://arxiv.org/abs/1406.2661): The original paper proposed the idea of GANs. 

[Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks](https://arxiv.org/abs/1511.06434): This paper proposed the idea of deep convolutional generative adversarial networks (DCGANs).


### 1.2 Code Written

[dcgan.ipynb](https://github.com/xiaolng/weekly_report/blob/master/source/dcgan.ipynb): A tutorial of DCGANs from pytorch.  It uses the [CelebA Faces dataset](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) which contains more than 200k  real celebrity faces. This code trains a DCGANs, and finally the generator is able to create fake celebrity faces. 


## 2. Figures

![](https://github.com/xiaolng/weekly_report/blob/master/imgs/0830_GANs.png?raw=true)

Figure 1. The archetecture of GANs. Two models are trained the same time, the generator and the discriminator. The generator tries to create fake image and the discriminator tries to label whether the input is fake or real. 

### 3. Results

I learned an unsupervised generative model, GANs, which is one of the hottest topic in deep learning. GANs' idea is  to train two models the same time, the generator and the discriminator. The job of the generator is to create fake data and the role of the discriminator is to label whether or not an input is from real training set or is fake from generator. And after many training steps, the generator obtains the ability to create almost the same data from training set.  GANs has huge applications. It can be used to create fake samples of any data distribution.
