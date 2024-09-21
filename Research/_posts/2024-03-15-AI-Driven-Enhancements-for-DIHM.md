---
layout: post
title: AI-Driven Enhancements for DIHM
---

<h2> Research 1. <br> <a href="https://www.sciencedirect.com/science/article/pii/S0956566323001744">AI-based analysis of 3D position and orientation of a red blood cell (RBC) using a DIHM</a> </h2>

Published as a co-first author, Biosensors and Bioelectronics (2023/06)

Despite their completely different morphology and rheological properties, similar Hagen-Poiseuille flows are observed in the channel flow from both a spherical bead and a healthy human red blood cell. However, red blood cells with varying membrane rigidity exhibit distinctive tumbling motions under shear flow. Therefore, a deeper and more precise analysis of an object’s physical properties or flow phenomena in fluid mechanics can be achieved by observing its orientations rather than just the velocity fields.

The biggest challenge in this research was measuring the out-of-plane angle θ, which is difficult to accurately determine from a single-intensity image. Therefore, this angle θ is predicted using a data-driven deep learning approach. To obtain the precise ground-truth angles, RBCs were trapped in polydimethylsiloxane (PDMS), a type of silicone. By meticulously manipulating the PDMS sample with a 4-axis optical stage, we were able to create datasets of RBCs with known precise out-of-plane angles.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBC1.png" alt= "Experimental setup">
  <figcaption style="font-size: 0.9em; color: #555;">1. Experimental Setup</figcaption>
</figure>


<br> The obtained datasets are used by the CAE to extract features of each image. New RBC images are generated using these extracted features to augment the data. The augmented datasets are then fed into CNN, which is trained to minimize the difference between the predicted angle θ and the ground truth out-of-plane angle. The trained CNN predicts the angles with a root mean square error of 4.73°. The figure below shows the process of reconstructing the position and orientation of arbitrary RBCs captured in a single-shot image.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBC3.png" alt= "Result">
  <figcaption style="font-size: 0.9em; color: #555;">2. Process of Acquiring Positions and Orientations of RBC</figcaption>
</figure>

<p style="font-size: 0.8em; text-align: right;"><br>Publication:</b> <strong>Y. Kim</strong>, J. Kim, E. Seo, S. Lee*, "AI-based analysis of 3D position and orientation of red blood cells using a digital in-line holographic microscopy" Biosensors and Bioelectronics, 2023, 229, 115232 https://doi.org/10.1016/j.bios.2023.115232</p>


<h2> Research 2. <br> AI-based analysis of 3D position and orientation of red blood cells in a channel flow using a DIHM </h2>

In this project, I focused primarily on <strong>idea conceptualization</strong>, <strong>experimental setup</strong>, and <strong>analyzing RBC tumbling</strong>.
<br>
<br>In our previous research, we focused on analyzing the orientation of static RBCs. For the next step, we aimed to utilize a CNN model trained on static RBC datasets to <strong>predict the orientations of flowing RBCs in the microchannel</strong>. However, due to low prediction accuracy, it became clear that the training dataset should be replaced with images acquired from the channel flow.

<br> In this project, we utilized a CNN-based supervised learning approach to predict the out-of-plane angles of flowing RBCs. One of the primary challenges we encountered was obtaining the ground truth out-of-plane angle θ for the RBCs within the microchannel. We demonstrated that by employing additional side-view imaging, we could effectively analyze the tumbling motion of the RBCs under shear rates using the <a href="https://royalsocietypublishing.org/doi/10.1098/rspa.1922.0078">Jeffery equation</a>, which was originally derived to describe the flipping motions of ellipsoidal particles in shear flows.
<div style="text-align: center;">
  <span style="font-family: 'Times New Roman', serif;">tan θ = r tan(γ̇ / (r + 1/r) t)</span>
</div>
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

<br>
<br>We trained the CNN model using the dataset obtained, aiming to minimize the error between the predicted angles θ and the ground truth out-of-plane angle. The completed model was able to predict the out-of-plane angle θ with a root mean square error of less than 3.62°. Using this model, we visualized the flow dynamics of red blood cells in a sudden expansion channel. Ultimately, we developed a technique that allows for the measurement of the position and orientation of flowing RBCs using only a single image.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/RBCflow4.png" alt= "Result">
  <figcaption style="font-size: 0.9em; color: #555;">2. Process of Acquiring Positions and Orientations of RBC</figcaption>
</figure>
<br>
<h2> Research 3. <br> 3D Morphology Reconstruction Using a Neural Fields from a Single DIHM Image</h2>

Ongoing project

<br>Although previous studies had reached a new state with the aid of AI in DIHM field, the fundamental limitations of DIHM remain unsolved. 이미지로 얻는 과정중 잃어버린 위상 정보 때문에 DIHM은 twin-image problem이 발생한다. twin image problem은 numerical reconstruction에 의한 depth-wise 분석에 converging or diverging하는 ㄱreal image에 반대 방향인 conjugate signal이 생기며, image의 resolution과 quality가 크게 저하된다. In addition, data-driven approach인 supervised learning은 generalization 능력이 부족해서 연구 대상을 바꿀 때마다 새로운 dataset을 생성해야 한다. Self-supervised learning은 이 문제에 대한 좋은 대안이 된다.
우리는 self-supervised learning이자 Physics driven approch로서, network에 얻어진 output feature를 beam propagation을 통해서 target object image으로 mapping시켜 두 이미지를 비교하면서 network를 갱신한다. Network는 coordinate-based neural network로 implicit representation을 사용하여 물체의 3D structure를 학습시킨다. 학습된 네트워크는...
