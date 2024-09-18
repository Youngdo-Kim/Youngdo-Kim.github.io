---
layout: post
title: Research Portfolio
---

<hr style='border : 1.5px solid navy;'>

> This page chronicles the journey of research under the guidance of <a href="http://bbrc.postech.ac.kr/page/member01">Dr. Sang Joon Lee</a> and <a href="https://hyoungsookimm.wixsite.com/filkaist">Dr. Hyoungsoo Kim</a>.
> For more information about my research, feel free to contact me. I always eager to discussing fascinating ideas and new perspectives.

<hr>

<h2> Exploring Digital In-line Holographic Microscopy (DIHM) </h2>

Digital holographic microscopy is a robust 3D imaging technique used for examining various microscale objects and microfluidic issues. Especially, DIHM setup is straightforward and <strong>compact</strong> due to its <strong>single beam path</strong>. By numerically reconstructing the depth-wise information from holographic images, one can obtain the <strong>3D positions</strong> and <strong>2D in-focus intensity images</strong> of objects. These reconstructed images are combined into a single image to determine the x and y positions of particles. Using a focus function, the particle depth with the highest focus value is identified as the z position.


<div style="display: flex; align-items: center;gap: 10px;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/DIHMsetup.png" alt="Experimental setup" style="width: 250px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">1. Experimental Setup</figcaption>
  </figure>
  <div style="display: flex; flex-direction: column;gap: 30px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image3.gif" alt="Acquired images" style="width: 210px; height: auto; margin-bottom: 30px; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">2. Acquired Images</figcaption>
    </figure>
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image5.gif" alt="Numerical reconstruction" style="width: 250px; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">3. Numerical Reconstruction</figcaption>
    </figure>
  </div>
  <div style="display: flex; flex-direction: column;gap: 5px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image6.jpeg" alt="Positioning of x,y" style="width: 185px; height: auto; margin-bottom: 10px; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">4. Positioning of x,y</figcaption>
    </figure>
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image8.gif" alt="Depth-wise Positioning" style="width: 275px; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">5. Depth-wise Positioning</figcaption>
    </figure>
  </div>
</div>

<p style="font-size: 0.8em; text-align: right;"><br>The above figure is related to 'T.Go, H. Byeon, S.Lee*, "Label-free sensor for automatic identification of erythrocytes using digital in-line holographic microscopy and machine learning" Biosensors and Bioelectronics, 2018, 103, 12-18 https://doi.org/10.1016/j.bios.2017.12.020'.</p>

<h2> Utilized Machine Learning (ML) Model </h2>

With the aid of recent advances in machine learning (ML) techniques, the combination of ML and DIHM techniques gives rise to a breakthrough in solving the technical limitations of conventional DIHM. <strong>Convolutional autoencoder (CAE)</strong> and <strong>convolutional neural network (CNN)</strong> is utilized to learn and predict the feature of the images acquired from DIHM.

<br>For the self-supervised CAE model, a CAE model trained with red blood cell (RBC) images can use features extracted from the latent space to predict angles or be used for data augmentation.
<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/AI1.png" alt= "CAE model">
  <figcaption style="font-size: 0.9em; color: #555;">1. CAE for Extracting Angle Features of RBCs </figcaption>
</figure>


<br>CNNs can be used to analyze red blood cell images to predict their orientation. By training the model with labeled images, it learns to accurately determine the angle of the cells, which can be crucial for medical diagnostics.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/AI2.png" alt= "CNN model">
  <figcaption style="font-size: 0.9em; color: #555;">2. CNN to Learn and Predict the Orientation of RBCs</figcaption>
</figure>

<br>The supervised learning model partially overcame the limitations of DIHM. However, each time we study new samples, we must rebuild the dataset. It requires significant time and computational cost for data collection and model training. To address this problem, we are currently implementing a <strong>self-supervised learning method</strong> to predict the features from an object image.
