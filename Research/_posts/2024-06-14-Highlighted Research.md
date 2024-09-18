---
layout: post
title: Research Portfolio
---

<hr style='border : 1.5px solid navy;'>

> This page gives a journey of research under the supervision of <a href="http://bbrc.postech.ac.kr/page/member01">Dr. Sang Joon Lee</a> and <a href="https://hyoungsookimm.wixsite.com/filkaist">Dr. Hyoungsoo Kim</a>.
> For more information on my research, feel free to contact me! I always look forward to discussing fascinating ideas and new perspectives.

<hr>

### Exploring Digital In-line Holographic Microscopy (DIHM)

Digital holographic microscopy is a robust 3D imaging technique used for examining various microscale objects and microfluidic issues. Especially, DIHM setup is straightforward and compact due to its single beam path. By numerically reconstructing the depth-wise information from holographic images, one can obtain the 3D positions and 2D in-focus intensity images of objects. These reconstructed images are combined into a single image to determine the x and y positions of particles. Using a focus function, the particle depth with the highest focus value is identified as the z position.


<div style="display: flex; align-items: center;gap: 10px;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/DIHMsetup.png" alt="Experimental setup" style="width: 250px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">1. Experimental setup</figcaption>
  </figure>
  <div style="display: flex; flex-direction: column;gap: 10px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image3.gif" alt="Acquired images" style="width: 210px; height: auto; margin-bottom: 30px; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">2. Acquired images</figcaption>
    </figure>
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image5.gif" alt="Numerical reconstruction" style="width: 250px; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">3. Numerical reconstruction</figcaption>
    </figure>
  </div>
  <div style="display: flex; flex-direction: column;gap: 10px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image6.jpeg" alt="Acquired images" style="width: 185px; height: auto; margin-bottom: 10px; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">4. Positioning of x,y</figcaption>
    </figure>
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image8.gif" alt="Numerical reconstruction" style="width: 275px; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">5. Depth-wise positioning</figcaption>
    </figure>
  </div>
</div>

<p style="font-size: 0.8em; text-align: right;">The above figure is related to 'T.Go, H. Byeon, S.Lee*, "Label-free sensor for automatic identification of erythrocytes using digital in-line holographic microscopy and machine learning" Biosensors and Bioelectronics, 2018, 103, 12-18 https://doi.org/10.1016/j.bios.2017.12.020'.</p>

### Utilized Machine Learning (ML) Model

With the aid of recent advances in machine learning (ML) techniques, the combination of ML and DIHM techniques gives rise to a breakthrough in solving the technical limitations of conventional DIHM. Convolutional autoencoder (CAE) and convolutional neural network (CNN) is utilized to learn and predict the feature of the images acquired from DIHM.

<br>For the self-supervised CAE model, a CAE model trained with red blood cell images can use features extracted from the latent space to predict angles or be used for data augmentation.
<img src="/Research/figures/AI1.png" alt= "CAE model">

CNNs can be used to analyze red blood cell images to predict their orientation. By training the model with labeled images, it learns to accurately determine the angle of the cells, which can be crucial for medical diagnostics.
<img src="/Research/figures/AI2.png" alt= "CNN model">

The supervised learning model partially overcame the limitations of DIHM. However, each time we study new samples, we must rebuild the dataset, which requires significant time and computational cost for data collection and model training. To address this problem, we are implementing a self-supervised learning method to predict the features of an object.
