---
layout: post
title: List of Publications
---

<hr style='border : 1.5px solid navy;'>
Notes: # indicates equally contributing first authors. * indicates the corresponding author(s).
<ol>
  <li><strong>Y. Kim#</strong>, J. Kim#, E. Seo, S. Lee*, AI-based analysis of 3D position and orientation of red blood cells using digital in-line holographic microscopy, Biosensors and Bioelectronics 223, 115232 (2023) 
 [<a href="https://youngdo-kim.github.io/research/2024/03/17/AI-Driven-Enhancements-for-DIHM/">More Info</a>] [<a href="https://www.sciencedirect.com/science/article/pii/S0956566323001744#section-cited-by">Published in</a>]</li>
  <li>J. Kim, J Kim, <strong>Y. Kim</strong>, T. Go, S. Lee*, Acceleration in the settling velocity of airborne particulate matter on hairy plant leaves, Journal of Environmental Management 332, 117313 (2023) [<a href="https://youngdo-kim.github.io/research/2022/03/16/Comprehensive-PM-Studies-Using-DIHM/">More Info</a>] [<a href="https://www.sciencedirect.com/science/article/pii/S0301479723001019">Published in</a>]</li>
  <li>J. Kim, <strong>Y. Kim</strong>, K. Howard, S. Lee*, Smartphone-based holographic monitoring of polydisperse suspended particulate matter concentrations, Scientific reports 12, 22609 (2022) [<a href="https://youngdo-kim.github.io/research/2022/03/16/Comprehensive-PM-Studies-Using-DIHM/">More Info</a>] [<a href="https://www.nature.com/articles/s41598-022-27215-6">Published in</a>]</li>
  <li>Y. Lee#, S. Shin#, G. Choi, H. Jeon, <strong>Y. Kim</strong>, H. Kim*, Symmetry breaking of Worthington jets by gradients in liquid pool depth, Physics of  Fluids 32, 112104 (2020) [<a href="https://youngdo-kim.github.io/research/2020/11/09/First-project/">More Info</a>] [<a href="https://pubs.aip.org/aip/pof/article/32/11/112104/1033346/Symmetry-breaking-of-Worthington-jets-by-gradients">Published in</a>]</li>
</ol>

<h1 style="font-size: 30px;">Catalyst for My Research Career</h1>
<a href="https://youngdo-kim.github.io/research/2020/11/09/First-project/">My first research</a> started in high school with a question that arose while trying to stop a nosebleed at the sink: Why do the falling blood droplets always splash in the same direction? As I delved into this topic, I realized that my academic foundation was insufficient for fully grasping a phenomenon I would later understand to be a function of fluid dynamics. Therefore, I chose to pursue mechanical engineering to deepen my knowledge of fluid dynamics. Along the way, I also set a goal to conduct research as a lead author. After six years of endeavor, I achieved both aspirations. My research journey, driven by curiosity and passion, will continue.

<div class="message">
This page chronicles the journey of research under the guidance of <a href="https://me.postech.ac.kr/page/professor13_en">Dr. Sang Joon Lee</a> and <a href="https://hyoungsookimm.wixsite.com/filkaist">Dr. Hyoungsoo Kim</a>. For more information about my research, feel free to contact me via email at youngdokim@postech.ac.kr. I am always eager to discuss fascinating ideas and new perspectives.
</div>

<hr>
<h2> Exploring Digital In-line Holographic Microscopy (DIHM) </h2>

Digital holographic microscopy is a robust 3D imaging technique used for examining various microscale objects and microfluidic issues. Specifically, DIHM setup is straightforward and <strong>compact</strong> due to its <strong>single beam path</strong>. By numerically reconstructing the depth-wise information from holographic images can be reconstructed to yield the <strong>3D positions</strong> and <strong>2D in-focus intensity images</strong> of objects. These reconstructed images are combined into a single image to determine the x and y positions of particles. The focus function identifies the particle depth with the highest focus value as the z position.


<div style="display: flex; align-items: center;gap: 10px;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/DIHMsetup.png" alt="Experimental setup" style="width: 250px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">1. Experimental Setup</figcaption>
  </figure>
  <div style="display: flex; flex-direction: column;gap: 35px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image3.gif" alt="Acquired images" style="width: 210px; height: auto; margin-bottom: 30px; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">2. Acquired Images</figcaption>
    </figure>
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image5.gif" alt="Numerical reconstruction" style="width: 250px; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">3. Numerical Reconstruction</figcaption>
    </figure>
  </div>
  <div style="display: flex; flex-direction: column;gap: 0px;">
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

<p style="font-size: 0.8em; text-align: right;"><br>The above figure pertains to 'T.Go, H. Byeon, S.Lee*, "Label-free sensor for automatic identification of erythrocytes using digital in-line holographic microscopy and machine learning" Biosensors and Bioelectronics, 2018, 103, 12-18 https://doi.org/10.1016/j.bios.2017.12.020</p>

<h2> Utilized Machine Learning (ML) Model </h2>

With the aid of recent advances in artificial intelligence, the combination of ML and DIHM techniques gives rise to a breakthrough in solving the technical limitations of conventional DIHM. <strong>Convolutional autoencoder (CAE)</strong> and <strong>convolutional neural network (CNN)</strong> are utilized to learn and predict the features of the images acquired from DIHM.

For the self-supervised CAE model, the model trained with red blood cell (RBC) images can use features extracted from the latent space to predict angles or be used for data augmentation.
<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/AI1.png" alt= "CAE model">
  <figcaption style="font-size: 0.9em; color: #555;">1. CAE for Extracting Angle Features of RBCs </figcaption>
</figure>


<br>CNNs can be used to analyze red blood cell images to predict their orientation. By training the model with labeled images, it learns to accurately determine the angle of the cells, which can be crucial for medical diagnostics.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/AI2.png" alt= "CNN model">
  <figcaption style="font-size: 0.9em; color: #555;">2. CNN to Learn and Predict the Orientation of RBCs</figcaption>
</figure>

<br>The supervised learning model partially overcame the limitations of DIHM. However, each time we study new samples, we must rebuild the dataset. It requires significant time and computational cost for data collection and model training. To address this problem, we are implementing a <strong>self-supervised learning method</strong> to directly predict the features from an object image.
