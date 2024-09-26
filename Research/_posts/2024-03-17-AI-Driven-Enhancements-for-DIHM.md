---
layout: post
title: AI-Driven Enhancements for DIHM
---

<h2> Research 1. <br> <a href="https://www.sciencedirect.com/science/article/pii/S0956566323001744">AI-based analysis of 3D position and orientation of a red blood cell (RBC) using a DIHM</a> </h2>

Published as a co-first author, Biosensors and Bioelectronics (2023/06)
<br>As a lead author, I took charge of all aspects of the project.
<br>

Despite their completely different morphology and rheological properties, similar Hagen-Poiseuille flows are observed in the channel flow from both a spherical bead and a healthy human red blood cell. However, red blood cells with varying membrane rigidity exhibit distinctive tumbling motions under shear flow. Therefore, a deeper and more <strong>precise analysis of an object’s physical properties</strong> or flow phenomena in fluid mechanics <strong>can be achieved by observing its orientations</strong> rather than just the velocity fields.

The biggest challenge in this research was <strong>measuring the out-of-plane angle θ</strong>, which is difficult to determine from a single-intensity image accurately. Therefore, this angle θ is predicted using a data-driven deep learning approach. To obtain the precise ground-truth angles, RBCs were trapped in polydimethylsiloxane (PDMS), a type of silicone. By meticulously manipulating the PDMS sample with a 4-axis optical stage, we were able to create datasets of RBCs with known precise out-of-plane angles.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBC1.png" alt= "Experimental setup">
  <figcaption style="font-size: 0.9em; color: #555;">1. Experimental Setup</figcaption>
</figure>


<br> The obtained datasets are used by the CAE to extract features of each image. New RBC images are generated using these extracted features to augment the data. The augmented datasets are then fed into CNN, which is trained to minimize the difference between the predicted angle θ and the ground truth out-of-plane angle. The trained CNN predicts the angles with a root mean square error of 4.73°. The figure below shows the process of reconstructing the position and orientation of arbitrary RBCs captured in a single-shot image.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBC3.png" alt= "Result">
  <figcaption style="font-size: 0.9em; color: #555;">2. Process of Acquiring Positions and Orientations of RBC</figcaption>
</figure>
<br>
<p style="font-size: 0.8em; text-align: right;"><b>Publication:</b> <strong>Y. Kim#</strong>, J. Kim#, E. Seo, S. Lee*, "AI-based analysis of 3D position and orientation of red blood cells using a digital in-line holographic microscopy" Biosensors and Bioelectronics, 2023, 229, 115232 https://doi.org/10.1016/j.bios.2023.115232</p>



<h2> Research 2. <br> AI-based analysis of 3D position and orientation of red blood cells in a channel flow using a DIHM </h2>
Co-author of Manuscript in preparation
<br>In this project, I primarily contributed to <strong>idea conceptualization</strong>, <strong>experimental setup</strong>, and <strong>the analysis of RBC tumbling</strong>.

In our previous research, we focused on analyzing the orientation of static RBCs. For the next step, we aimed to utilize a CNN model trained on static RBC datasets to <strong>predict the orientations of flowing RBCs in the microchannel</strong>. However, due to low prediction accuracy, it became clear that the training dataset should be replaced with images acquired from the channel flow.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBCflow5.gif" alt= "Result">
  <figcaption style="font-size: 0.9em; color: #555;">1. Acquired Images from the Microchannel</figcaption>
</figure>

CNN-based supervised learning approach was utilized to predict the out-of-plane angles of flowing RBCs. One of the primary challenges was obtaining the ground truth out-of-plane angle θ for the RBCs within the microchannel. We demonstrated that by employing additional side-view imaging, we could effectively analyze the tumbling angle of the RBCs under shear rates using the <a href="https://royalsocietypublishing.org/doi/10.1098/rspa.1922.0078">Jeffery equation</a>, which was originally derived to describe the flipping motions of ellipsoidal particles in shear flows.
<br>The Jeffery equation is expressed as <img src="/Research/figures/eqn1.png" style="display: inline; vertical-align: middle;">
Furthermore, we established the angles from the half-a-revolution image set, interpreted through the Jeffery equation, to serve as the ground truth out-of-plane angle.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBCflow6.png" alt= "Result">
  <figcaption style="font-size: 0.9em; color: #555;">2. Experimental Setup and the Jeffery Equation Fitting</figcaption>
</figure>

<br>The parameters of the Jeffery equation fitted from the experimental data showed a similar trend to the theoretical parameter values. This result supports the validity of the calculated out-of-plane angle from the Jeffery equation. We trained the CNN model using the obtained dataset to minimize the error between the predicted angles θ and the ground truth out-of-plane angle. The completed model was able to predict the out-of-plane angle θ with a root mean square error of less than 3.62°. Using this model, <strong>flow dynamics of red blood cells in a sudden expansion channel were visualized</strong>. Ultimately, we developed a technique that allows for the measurement of the position and orientation of flowing RBCs using only a single image.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBCflow7.png" alt= "Result">
  <figcaption style="font-size: 0.9em; color: #555;">3. The Trend of Fitted Parameters, the Prediction Performance of Model and Visualization of RBCs in Sudden Expansion Channel</figcaption>
</figure>


<!--

<h2> Research 2. <br> AI-based analysis of 3D position and orientation of red blood cells in a channel flow using a DIHM </h2>
Co-author of Manuscript Under Revision
<br>In this project, I primarily contributed to <strong>idea conceptualization</strong>, <strong>experimental setup</strong>, and the <strong>analysis of RBC tumbling</strong>.

In our previous research, we focused on analyzing the orientation of static RBCs. For the next step, we aimed to utilize a CNN model trained on static RBC datasets to <strong>predict the orientations of flowing RBCs in the microchannel</strong>. However, due to low prediction accuracy, it became clear that the training dataset should be replaced with images acquired from the channel flow.

CNN-based supervised learning approach was utilized to predict the out-of-plane angles of flowing RBCs. One of the primary challenges was obtaining the ground truth out-of-plane angle θ for the RBCs within the microchannel. We demonstrated that by employing additional side-view imaging, we could effectively analyze the tumbling motion of the RBCs under shear rates using the <a href="https://royalsocietypublishing.org/doi/10.1098/rspa.1922.0078">Jeffery equation</a>, which was originally derived to describe the flipping motions of ellipsoidal particles in shear flows.
<br>The Jeffery equation is expressed as <img src="/Research/figures/eqn1.png" style="display: inline; vertical-align: middle;">

Furthermore, we established that the angles obtained from the half-full revolution image set, interpreted through the Jeffery equation, serve as the ground truth out-of-plane angle.

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


<br>We trained the CNN model using the dataset obtained, aiming to minimize the error between the predicted angles θ and the ground truth out-of-plane angle. The completed model was able to predict the out-of-plane angle θ with a root mean square error of less than 3.62°. Using this model, <strong>flow dynamics of red blood cells in a sudden expansion channel were visualized</strong>. Ultimately, we developed a technique that allows for the measurement of the position and orientation of flowing RBCs using only a single image.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBCflow4.png" alt= "Result">
  <figcaption style="font-size: 0.9em; color: #555;">2. Process of Acquiring Positions and Orientations of RBC</figcaption>
</figure>

-->


<br>
<h2> Research 3. <br> 3D Morphology Reconstruction Using Neural Fields from a Single DIHM Image - Ongoing Project</h2>
Although previous studies have reached a new state with the aid of AI in DIHM field, the fundamental limitations of DIHM remain unsolved. Due to the loss of phase information during the image acquisition process, DIHM experiences the <strong>twin-image problem</strong>. This problem arises due to the inherent generation of a conjugate signal during numerical reconstruction, which significantly degrades the resolution and quality of the image.
<br>Additionally, the <strong>data-driven approach of supervised learning lacks generalization capabilities</strong>, necessitating the creation of new datasets each time the research subject changes. Self-supervised learning presents a promising alternative to this issue.
<br>In this project, a <strong>physics-driven and self-supervised learning approach is utilized to address these limitations</strong>. A coordinate-based neural network with implicit representation is trained to learn the 3D structure of the object. The input consists of coordinates, while the output represents the real part of the corresponding refractive index. These output features are then mapped to the target object image through a forward model which is the angular spectrum method. The network is trained to minimize the difference between the simulated image and the target image. <strong>The goal of the model is to reconstruct the 3D refractive index of an object from a single image.</strong>
