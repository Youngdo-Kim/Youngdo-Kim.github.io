---
layout: post
title: AI-Driven Enhancements for DIHM
---

<h2> Research 1. <br> <a href="https://www.sciencedirect.com/science/article/pii/S0956566323001744">AI-based analysis of 3D position and orientation of a red blood cell (RBC) using a DIHM</a> </h2>

Published as a co-first author, Biosensors and Bioelectronics (2023/06)
<br>
<br>Similar Hagen-Poiseuille flows are observed in the channel flow from both a spherical bead and a healthy human red blood cell, despite their completely different morphology and rheological properties. However, red blood cells with varying membrane rigidity exhibit distinctive tumbling motions under shear flow. Therefore, a deeper and more precise analysis of an object’s physical properties or flow phenomena in fluid mechanics can be achieved by observing its orientations rather than just the velocity fields.

<br>
<br>The biggest challenge in this research was measuring the out-of-plane angle θ, which is difficult to accurately determined from a single intensity image. Therefore, this angle θ is predicted using a data-driven deep learning approach. To obtain the precise ground-truth angles, RBCs were trapped in polydimethylsiloxane (PDMS), a type of silicone. By meticulously manipulating the PDMS sample with a 4-axis optical stage, we were able to create datasets of RBCs with known precise out-of-plane angles.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBC1.png" alt= "Experimental setup">
  <figcaption style="font-size: 0.9em; color: #555;">1. Experimental Setup</figcaption>
</figure>

<br> The obtained datasets are used by the CAE to extract features of each image. Using these extracted features, new RBC images are generated to augment the data. The augmented datasets are then fed into CNN, which is trained to minimize the difference between the predicted angle θ and the ground truth out-of-plane angle. The trained CNN predicts the angles with a root mean square error of 4.73°. The figure below shows the process of reconstructing the position and orientation of arbitrary RBCs captured in a single-shot image.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBC3.png" alt= "Result">
  <figcaption style="font-size: 0.9em; color: #555;">2. Process of Acquiring Positions and Orientations of RBC</figcaption>
</figure>

<p style="font-size: 0.8em; text-align: right;"><br>The above figure pertains to 'T.Go, H. Byeon, S.Lee*, "Label-free sensor for automatic identification of erythrocytes using digital in-line holographic microscopy and machine learning" Biosensors and Bioelectronics, 2018, 103, 12-18 https://doi.org/10.1016/j.bios.2017.12.020</p>

<br><b>Publication:</b> <strong>Y. Kim</strong>, J. Kim, E. Seo, S. Lee*, "AI-based analysis of 3D position and orientation of red blood cells using a digital in-line holographic microscopy" Biosensors and Bioelectronics, 2023, 229, 115232 https://doi.org/10.1016/j.bios.2023.115232

<h2> Research 2. <br> AI-based analysis of 3D position and orientation of red blood cells in a channel flow using a DIHM </h2>

In this project, I focused primarily on idea conceptualization, experimental setup, and analyzing RBC tumbling.
<br>
<br>Static한 RBC에 대해 관찰했으니 한 발 나아가 channel flow에서 관찰했다. In the previous research, we were focused on analyzing the orientation of static RBCs. For the next step, we tried to utilize the trained CNN model to predict the orientations on flowing red blood cells in the channel. However, due to the low prediction accuracy, training dataset should be replaced to images acquired from the channel.

<br> 이 프로젝트에서도 CNN을 이용한 supervised learning으로 각도를 예측했다. 이 project에서도 가장 큰 문제는 채널 속을 흐르는 적혈구의 ground truth out-of-plane angle을 얻는 것이었다. 우리는 side view로 ellipsoidal particle이 shear rate하에서 tumbling하는 motion을 설명하는 Jeffery equation으로 적혈구의 tumbling motion을 해석할 수 있다는 것을 추가적인 side view 촬영으로 보였다. 그리고 one-full revolution image set을 Jeffery equation으로 해석해서 얻은 각도를 ground truth angle이라고 정했다.

<div style="display: flex; align-items: center;gap: 10px;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/RBCflow1.png" alt="Experimental setup" style="width: 720px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">1. Experimental Setup</figcaption>
  </figure>
  <div style="display: flex; flex-direction: column;gap: 30px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/RBCflow2.gif" alt="Acquired images" style="width: 120px; height: auto; margin-bottom: 15px; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">2. Acquired Images</figcaption>
    </figure>
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/RBCflow3.gif" alt="Numerical reconstruction" style="width: 120px; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">3. Acquired Images</figcaption>
    </figure>
  </div>
</div>

이렇게 모인 dataset을 CNN model에 넣어서 예측한 각도와 ground truth angle의 오차가 적어지도록 학습시키고 학습이 완료된 모델은 3.62° 미만의 root mean square error로 out-of-plane angle θ를 예측한다. 우리는 이 모델로 sudden expansion channel 속을 흐르는 적혈구의 flow dynamics를 가시화했다. 우리는 single image만으로 channel 속을 흐르는 적혈구의 position와 orientation을 얻었다.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBCflow4.png" alt= "Result">
  <figcaption style="font-size: 0.9em; color: #555;">2. Process of Acquiring Positions and Orientations of RBC</figcaption>
</figure>

### Research 3. <br> Physics-driven neural network based the three-dimensional morphology reconstruction using DIHM (Ongoing project)

Ongoing project
<br> 프로젝트 소개
