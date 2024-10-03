---
layout: post
title: Comprehensive Particulate Matter (PM) Studies Using DIHM
truncated_preview: true
excerpt_separator: <!--more-->
---

<div class="message">
As environmental pollution intensifies, interest and research in PM are growing. In these studies, DIHM investigated the dynamics of PM settling on plants and developed a method to measure the concentration of PM suspended in water. As a co-author, I contributed to experiment design and formal analysis, making it a valuable opportunity to learn DIHM technology and supervised machine learning models.
</div>

<h2> Research 4. <br><a href="https://www.sciencedirect.com/science/article/pii/S0301479723001019">Accelerated settling velocity of airborne PM on hairy plant leaves</a></h2>

Published as a co-author, Journal of Environmental Management (2023/04)<br>In this project, I focused primarily on <strong>formal analysis</strong>.

Perilla (sesame) and pepper leaves, which are widely cultivated in Korea, show differences in terms of trichomes. While the individual trichome sizes of both leaves are similar, the trichomes on perilla leaves are over three times denser, and the surface charge density is measured to be more than five times greater.  Although the PM was dropped from a sufficient distance away from the perilla leaves, allowing enough time to reach terminal velocity, it was observed that its <strong>velocity increased as the PM approached the leaves</strong>. This acceleration is <strong> due to the attraction between the enhanced electronic field</strong> created by the sharp trichomes, <strong>causing the PM velocity to exceed the terminal velocity of the freely falling PM</strong>.

<div style="display: flex; justify-content: space-around; align-items: center;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf1.jpg" alt="Perilla leaf" style="width: 250px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">1. Experimental Setup</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf3.gif" alt="Acquired images" style="width: 160px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">2. Acquired PM Images</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf2.jpeg" alt="Velocity visualization" style="width: 350px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">3. Velocity Field Visulization</figcaption>
  </figure>
</div>

<br>I analyzed the theoretical settling velocity of free-falling PM, which is achieved when drag and gravitational forces are balanced under low-speed conditions, known as Stokes flow. As shown by the dotted line in Figure 4, the theoretical velocity model exhibited a similar order to the measured values. Additionally, it was observed that the velocity of the PM approaching the leaves increased by approximately 3% for perilla leaves and about 6% for pepper leaves compared to when it was relatively farther away. Through this project, I gained experience in optical setup, imaging, reconstruction, and particle tracking using DIHM.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/Leaf4.jpg" alt="Velocity distribution" style="width: auto; height: auto; display: block; margin: 0 auto;">
  <figcaption style="font-size: 0.9em; color: #555;">4. Settling Velocity Graph by PM Diameter</figcaption>
</figure>

<p style="font-size: 0.8em; text-align: right;"><br><b>Publication:</b> J. Kim, J. Kim, <b>Y. Kim</b>, T. Go, and S. Lee*. (2023). Accelerated settling velocity of airborne particulate matter on hairy plant leaves. J. Environ. Manage. 332, 117313. doi:10.1016/j.jenvman.2023.117313</p>
<br>

<h2>Research 5. <br><a href="https://www.nature.com/articles/s41598-022-27215-6">Smartphone-based holographic measurement of polydisperse suspended PM with various mass concentration ratios</a></h2>

Published as a co-author, Scientific Reports (2022/12)<br>In this project, I focused primarily on <strong>optical setup</strong> and <strong>sample preparation</strong>.
<br>
<div style="display: flex; justify-content: space-around; align-items: center; gap: 20px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/smart1.jpeg" alt="Velocity distribution" style="width: 250; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">1. Principle of Speckle Pattern Generation</figcaption>
    </figure>
    <div class="text">
        
        <p>
          This project <strong>aimed to replace expensive conventional PM measuring devices with a smartphone-based solution</strong>. As for the experimental setup, I developed a device using a smartphone instead of a conventional high-speed camera, creating the entire system for under $400 using a 3D printer and the smartphone. The PM concentration in a solution containing a mixture of fine PM (1.2 micrometers) and coarse PM (7.6 micrometers) was predicted with DIHM and machine learning. When a light source interacts with an object, it produces fringe patterns, which, when accumulated, form a speckle pattern. These speckle patterns were used to predict the concentrations of coarse and fine PMs through a machine-learning model.
        </p>
    </div>
</div>


<div style="display: flex; justify-content: space-around; align-items: center;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart2.png" alt="Experimental setup" style="width: 350px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">2. Experimental Setup</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart3.png" alt="Fine PM concentration prediction" style="width: 250px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">3. Fine PM Concentration Prediction</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart4.png" alt="Coarse PM concentration prediction" style="width: 250px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">4. Coarse PM Concentration Prediction</figcaption>
  </figure>
</div>

<br>This model was trained exclusively on images of single concentrations to <strong>predict the concentrations of coarse and fine PM from images of a polydisperse solution</strong>. The spatial frequencies of the speckle pattern generated by fine PM are generally much higher than that of coarse PM. Consequently, <strong>the mixed signal from the polydisperse solution can be separated into fine and coarse PM signals using Gaussian high-pass and low-pass filters</strong>. Monodisperse coarse and fine PM samples with known concentrations were passed through these filters before entering each CAE for feature extraction. The extracted features served as inputs for fully connected neural networks to predict the PM concentration in the images. The model was trained to minimize the discrepancy between the predicted PM concentration and the ground truth concentration. While <strong>the predictions for fine PM concentrations showed moderate accuracy, the coarse PM concentrations required additional correction factors post-prediction</strong>. 

<p style="font-size: 0.8em; text-align: right;"><br><b>Publication:</b> J. Kim, <b>Y. Kim</b>, K. J. Howard, and S. Lee*. (2022). Smartphone-based holographic measurement of polydisperse suspended particulate matter with various mass concentration ratios. Sci. Rep. 12, 22609. https://doi.org/10.1038/s41598-022-27215-6</p>
