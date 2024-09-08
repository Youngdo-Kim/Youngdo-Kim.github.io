---
layout: post
title: Comprehensive Particulate Matter (PM) Studies Using DIHM
truncated_preview: true
excerpt_separator: <!--more-->
---

<div class="message">
환경오염이 심해지면서 particulate matter에 대한 관심과 연구가 점점 커지고 있다. 여기에서는 DIHM을 이용해서 식물에 settling하는 PM의 dynamics를 연구하고 물에 떠다니는 PM의 농도를 측정하는 방법을 개발하였다. 여기서는 공저자로서 실험 셋업 개발이나 formal analysis에 기여하며 DIHM 기술 습득과 AI model을 익히는 유용한 기회였다.
</div>

## Visualizing Faster PM Deposition on Trichome-Rich Plant Leaves

Published as a co-author, Journal of Environmental Management (2023/04)
<br> 나뭇잎 연구에서는 PM이 식물 가까이에 접근하면서 식물의 Trichome에 접근하면 점점 빨라지는 속도장을 DIHM으로 가시화했다. 가시화 결과 Trichome에 접근할 수록 뾰족한 trichome에 의해 강화된 전기장 때문에 PM의 속도가 점점 빨라짐을 알 수 있다.

<div style="display: flex; justify-content: space-around; align-items: center;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf1.jpg" alt="Perilla leaf" style="width: 200px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">1. Experimental setup</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf3.gif" alt="Acquired images" style="width: 150px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">2. Acquired PM images</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf2.jpeg" alt="Velocity visualization" style="width: 250px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">3. Velocity field visulization</figcaption>
  </figure>
</div>

나는 leaf위에 낙하하는 PM settling velocity의 reference가 되는 freely falling PM의 velocity를 구했다. PM은 drag와 gravitational force가 평형을 이루며,
그 공식은 <p> $$V_{s,\text{theor}} = \frac{C_C (\rho_{PM} - \rho_{air}) g D^2}{18 k_s / \mu_{air}}$$ </p> 이다. Through this project, I gained experience in optical setup, imaging, reconstruction, and particle tracking using DIHM.
<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/Leaf4.jpg" alt="Velocity distribution" style="width: auto; height: auto; display: block; margin: 0 auto;">
  <figcaption style="font-size: 0.9em; color: #555;">4. Settling velocity graph by PM diameter</figcaption>
</figure>
<br><b>Publication:</b> Kim, J., Kim, J., <b>Kim, Y.</b>, Go, T., and Lee, S. J. (2023). Accelerated settling velocity of airborne particulate matter on hairy plant leaves. J. Environ. Manage. 332, 117313. doi:10.1016/j.jenvman.2023.117313


## Smartphone-based holographic measurement of polydisperse suspended particulate matter with various mass concentration ratios

Published as a co-author, Scientific Reports (2022/12)
<br>
<div style="display: flex; justify-content: space-around; align-items: center; gap: 20px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/smart1.jpeg" alt="Velocity distribution" style="width: 200; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">1. Principle of speckle pattern generation</figcaption>
    </figure>
    <div class="text">
        
        <p>
          The second project aimed to replace expensive conventional particulate matter (PM) measuring devices with a smartphone-based solution. Using DIHM and artificial intelligence,
          we predicted the PM concentration in a solution containing a mixture of fine PM (approximately 1.2 micrometers) and coarse PM (7.6 micrometers).
          I was responsible for the optical setup and sample preparation. We were able to create the setup for under $400 using a 3D printer and a Samsung smartphone.
          An object produces fringe patterns, and when these fringe patterns accumulate, they form a speckle pattern.
        </p>
    </div>
</div>


<div style="display: flex; justify-content: space-around; align-items: center;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart2.png" alt="Experimental setup" style="width: 220px; height: auto; display: block; margin: 0 auto;">
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

<br><b>Publication:</b> Kim, J., <b>Kim, Y.</b>, Howard, K. J. and Lee, S. J. (2022). Smartphone-based holographic measurement of polydisperse suspended particulate matter with various mass concentration ratios. Sci. Rep. 12, 22609. https://doi.org/10.1038/s41598-022-27215-6

