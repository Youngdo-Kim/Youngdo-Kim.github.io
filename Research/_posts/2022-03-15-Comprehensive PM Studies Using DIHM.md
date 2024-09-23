---
layout: post
title: Comprehensive Particulate Matter (PM) Studies Using DIHM
truncated_preview: true
excerpt_separator: <!--more-->
---

<div class="message">
As environmental pollution intensifies, interest and research in PM are growing. In these studies, we used DIHM to investigate the dynamics of PM settling on plants and developed a method to measure the concentration of PM suspended in water. As a co-author, I contributed to experiment design and formal analysis, making it a valuable opportunity to learn DIHM technology and supervised machine learning models.
</div>

<h2> Research 4. <br>Accelerated settling velocity of airborne PM on hairy plant leaves</h2>

Published as a co-author, Journal of Environmental Management (2023/04)<br>In this project, I focused primarily on <strong>formal analysis</strong>.

<br>한국에서 많이 재배되는 깻잎과 고추잎은 trichome의 측면에서 큰 차이가 있다. 두 잎은 individual한 trichome size는 비슷하지만 깻잎의 trichome이 3배 이상 빽빽하며 surface charge density도 5배 이상 크게 측정되었다. PM이 잎으로부터 충분한 거리를 이격했기 때문에 종단속도에 진입할 충분한 시간이 제공되었음에도 불구하고 PM이 잎에 낙하하면서 trichome에 가까이 접근할 수록 점점 속력이 빨라지는 모습을 가시화했다. 뾰족한 trichome에 의해 강화된 전기장 때문에 PM의 속도가 점점 빨라진다.

<div style="display: flex; justify-content: space-around; align-items: center;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf1.jpg" alt="Perilla leaf" style="width: 230px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">1. Experimental setup</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf3.gif" alt="Acquired images" style="width: 180px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">2. Acquired PM images</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/Leaf2.jpeg" alt="Velocity visualization" style="width: 330px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">3. Velocity field visulization</figcaption>
  </figure>
</div>

Leaf위에 떨어지는 PM velocity와 비교 가능한 free falling PM의 theoretical velocity는 drag와 gravitational force가 평형을 이룬다. Theoretical velocity model이 측정 값들과 비슷한 크기 정도를 보이는 것을 알 수 있다. 또한 잎에 접근하는 PM이 잎에서 비교적 떨어진 순간의 속도보다 가까이 접근했을 때 속도가 깻잎은 약 3%, 고추잎은 약 6% 정도 더 증가한 것을 관찰했다. Through this project, I gained experience in optical setup, imaging, reconstruction, and particle tracking using DIHM.

<figure style="margin: 0; text-align: center;">
  <img src="/Research/figures/Leaf4.jpg" alt="Velocity distribution" style="width: auto; height: auto; display: block; margin: 0 auto;">
  <figcaption style="font-size: 0.9em; color: #555;">4. Settling velocity graph by PM diameter</figcaption>
</figure>
<p style="font-size: 0.8em; text-align: right;"><br><b>Publication:</b> Kim, J., Kim, J., <b>Kim, Y.</b>, Go, T., and Lee, S. J. (2023). Accelerated settling velocity of airborne particulate matter on hairy plant leaves. J. Environ. Manage. 332, 117313. doi:10.1016/j.jenvman.2023.117313</p>
<br>

<h2>Research 5. <br> Smartphone-based holographic measurement of polydisperse suspended PM with various mass concentration ratios</h2>

Published as a co-author, Scientific Reports (2022/12)<br>In this project, I focused primarily on <strong>optical setup</strong> and <strong>sample preparation</strong>.
<br>
<div style="display: flex; justify-content: space-around; align-items: center; gap: 20px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/smart1.jpeg" alt="Velocity distribution" style="width: 250; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">1. Principle of speckle pattern generation</figcaption>
    </figure>
    <div class="text">
        
        <p>
          This project aimed to replace expensive conventional PM measuring devices with a smartphone-based solution. Using DIHM and machine learning,
          we predicted the PM concentration in a solution containing a mixture of fine PM (1.2 micrometers) and coarse PM (7.6 micrometers).
          When a light source meets an object, it produces fringe patterns; when these fringe patterns accumulate, they form a speckle pattern.
          These speckle patterns were utilized to predict the concentration of coarse and fine PMs.
          우리는 monodisperse한 coarse and fine PM 이미지들을 학습해서 그 둘이 섞여있는 polydisperse한 solution의 농도를 각각 예측할 것이다.
        </p>
    </div>
</div>


<div style="display: flex; justify-content: space-around; align-items: center;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart2.png" alt="Experimental setup" style="width: 350px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">2. Experimental setup</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart3.png" alt="Fine PM concentration prediction" style="width: 250px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">3. Fine PM concentration prediction</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/smart4.png" alt="Coarse PM concentration prediction" style="width: 250px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">4. Coarse PM concentration prediction</figcaption>
  </figure>
</div>

<br>보통 fine PM의 spatial frequency가 coarse PM의 spatial frequency보다 훨씬 높다. 그래서 우리는 가우시안 high and low pass filter로 mixture의 신호를 분리해서 fine PM과 coarse PM을 예측했다. 농도가 알려진 Monodisperse coarse and fine PM은 각각 low pass filter와 high pass filter를 거친 후에 CAE에 들어가서 feature가 추출된다. 추출된 feature는 fully connected neural network에 input으로 들어가고 ground truth 농도와 오차를 줄이는 방향으로 학습된다. 학습된 모델은 coarse PM과 fine PM이 섞여있는 solution의 각 농도를 예측한다. Fine PM은 농도예측이 잘 되지만 coarse PM은 예측 후에 추가적인 correction factor로 보정이 필요했다. 이 연구에는 conventional한 DIHM setup이 아니라 camera 대신 smartphone을 사용한 setup을 개발했다. We created the setup for under $400 using a 3D printer and a Samsung smartphone.

<p style="font-size: 0.8em; text-align: right;"><br><b>Publication:</b> Kim, J., <b>Kim, Y.</b>, Howard, K. J., and Lee, S. J. (2022). Smartphone-based holographic measurement of polydisperse suspended particulate matter with various mass concentration ratios. Sci. Rep. 12, 22609. https://doi.org/10.1038/s41598-022-27215-6</p>

