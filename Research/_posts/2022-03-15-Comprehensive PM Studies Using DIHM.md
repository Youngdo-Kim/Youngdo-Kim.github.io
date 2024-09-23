---
layout: post
title: Comprehensive Particulate Matter (PM) Studies Using DIHM
truncated_preview: true
excerpt_separator: <!--more-->
---

<div class="message">
As environmental pollution intensifies, interest and research in particulate matter (PM) are growing. In these studies, we used DIHM to investigate the dynamics of PM settling on plants and developed a method to measure the concentration of PM suspended in water. As a co-author, I contributed to experiment design and formal analysis, making it a valuable opportunity to learn DIHM technology and supervised machine learning models.
</div>

<h2> Research 4. <br>Visualizing Faster PM Deposition on Trichome-Rich Plant Leaves </h2>

Published as a co-author, Journal of Environmental Management (2023/04)<br>In this project, I focused primarily on <strong>formal analysis</strong>.

<br>나뭇잎 연구에서는 PM이 식물 가까이에 접근하면서 식물의 Trichome에 접근하면 점점 빨라지는 속도장을 DIHM으로 가시화했다. 가시화 결과 Trichome에 접근할 수록 뾰족한 trichome에 의해 강화된 전기장 때문에 PM의 속도가 점점 빨라짐을 알 수 있다.

<div style="display: flex; justify-content: space-around; align-items: center;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf1.jpg" alt="Perilla leaf" style="width: 150px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">1. Experimental setup</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf3.gif" alt="Acquired images" style="width: 120px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">2. Acquired PM images</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf2.jpeg" alt="Velocity visualization" style="width: 300px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">3. Velocity field visulization</figcaption>
  </figure>
</div>
<p>
나는 leaf위에 낙하하는 PM settling velocity의 reference가 되는 freely falling PM의 velocity를 구했다. PM은 drag와 gravitational force가 평형을 이루며,
그 공식은  $$V_{s,\text{theor}} = \frac{C_C (\rho_{PM} - \rho_{air}) g D^2}{18 k_s / \mu_{air}}$$ 이다. Through this project, I gained experience in optical setup, imaging, reconstruction, and particle tracking using DIHM.
</p>

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/Leaf4.jpg" alt="Velocity distribution" style="width: auto; height: auto; display: block; margin: 0 auto;">
  <figcaption style="font-size: 0.9em; color: #555;">4. Settling velocity graph by PM diameter</figcaption>
</figure>
<p style="font-size: 0.8em; text-align: right;"><br><b>Publication:</b> Kim, J., Kim, J., <b>Kim, Y.</b>, Go, T., and Lee, S. J. (2023). Accelerated settling velocity of airborne particulate matter on hairy plant leaves. J. Environ. Manage. 332, 117313. doi:10.1016/j.jenvman.2023.117313</p>
<br>

## Research 5. <br> Smartphone-based holographic measurement of polydisperse suspended particulate matter (PM) with various mass concentration ratios

Published as a co-author, Scientific Reports (2022/12)
<br>
<div style="display: flex; justify-content: space-around; align-items: center; gap: 20px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/smart1.jpeg" alt="Velocity distribution" style="width: 250; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">1. Principle of speckle pattern generation</figcaption>
    </figure>
    <div class="text">
        
        <p>
          This project aimed to replace expensive conventional PM measuring devices with a smartphone-based solution. Using DIHM and machine learning,
          we predicted the PM concentration in a solution containing a mixture of fine PM (around 1.2 micrometers) and coarse PM (7.6 micrometers).
          I was responsible for the optical setup and sample preparation. We were able to create the setup for under $400 using a 3D printer and a Samsung smartphone.
          An object produces fringe patterns, and when these fringe patterns accumulate, they form a speckle pattern.
        </p>
    </div>
</div>


<div style="display: flex; justify-content: space-around; align-items: center;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart2.png" alt="Experimental setup" style="width: 280px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">2. Experimental setup</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart3.png" alt="Fine PM concentration prediction" style="width: 150px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">3. Fine PM concentration prediction</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart4.png" alt="Coarse PM concentration prediction" style="width: 150px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">4. Coarse PM concentration prediction</figcaption>
  </figure>
</div>

<p style="font-size: 0.8em; text-align: right;"><br><b>Publication:</b> Kim, J., <b>Kim, Y.</b>, Howard, K. J., and Lee, S. J. (2022). Smartphone-based holographic measurement of polydisperse suspended particulate matter with various mass concentration ratios. Sci. Rep. 12, 22609. https://doi.org/10.1038/s41598-022-27215-6</p>

