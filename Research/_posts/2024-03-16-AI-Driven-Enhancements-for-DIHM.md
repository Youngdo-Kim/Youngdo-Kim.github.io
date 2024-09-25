---
layout: post
title: AI-Driven Enhancements for DIHM
---

<h2> Research 2. <br> AI-based analysis of 3D position and orientation of red blood cells in a channel flow using a DIHM </h2>
Co-author of Manuscript Under Revision
<br>In this project, I contributed to the project, primarily on <strong>idea conceptualization</strong>, <strong>experimental setup</strong>, and <strong>analyzing RBC tumbling</strong>.

In our previous research, we focused on analyzing the orientation of static RBCs. For the next step, we aimed to utilize a CNN model trained on static RBC datasets to <strong>predict the orientations of flowing RBCs in the microchannel</strong>. However, due to low prediction accuracy, it became clear that the training dataset should be replaced with images acquired from the channel flow.

CNN-based supervised learning approach was utilized to predict the out-of-plane angles of flowing RBCs. One of the primary challenges was obtaining the ground truth out-of-plane angle θ for the RBCs within the microchannel. We demonstrated that by employing additional side-view imaging, we could effectively analyze the tumbling motion of the RBCs under shear rates using the <a href="https://royalsocietypublishing.org/doi/10.1098/rspa.1922.0078">Jeffery equation</a>, which was originally derived to describe the flipping motions of ellipsoidal particles in shear flows.
<br>The Jeffery equation is expressed as <img src="/Research/figures/eqn1.png" style="display: inline; vertical-align: middle;">

<!--<div style="text-align: center;">
  <span style="font-family: 'Times New Roman', serif;">tan θ = r tan(γ̇ / (k + 1/k) t)</span>
</div>-->
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
<br>
