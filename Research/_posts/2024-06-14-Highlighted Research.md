---
layout: post
title: Research Portfolio
---

<hr style='border : 1.5px solid navy;'>

이 페이지는 이상준 교수님과 김형수 교수님께 지도를 받았던 제 연구 발자취를 적어놓았습니다. 제 연구에 대한 더 많은 정보를 위해서는 저에게 feel free to 연락주세요! 저는 흥미로운 아이디어에 대한 토론과 새로운 시각을 환영합니다!
<!-- Celeste is a lightweight Jekyll theme that features a minimalist, content-first design. It places your content center stage and lets your readers view them in a clutter-free environment without visual distractions. It is based on [Poole](https://github.com/poole/poole), the Jekyll butler, by [@mdo](https://github.com/mdo). -->

<hr>

### Exploring Digital In-line Holographic microscopy (DIHM)

DIHM은 single beam path를 가져서 simple한 optical setup을 가지고 있다. 촬영한 이미지를 angular spectrum method를 통해 numerically reconstruction해서 depth-wise 분석도 가능하다. 이렇게 reconstruction한 image들을
projection 시켜서 x,y positioning이 가능하고 z-value를 focus function으로 알아내서 particle의 3차원 position과 2D intensity를 알 수 있는 device이다.


<div style="display: flex; align-items: center;gap: 10px;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/DIHMsetup.png" alt="Experimental setup" style="width: 200px; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">1. Experimental setup</figcaption>
  </figure>
  <div style="display: flex; flex-direction: column;gap: 10px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image3.gif" alt="Acquired images" style="width: 160px; height: auto; margin-bottom: 30px; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">2. Acquired images</figcaption>
    </figure>
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image5.gif" alt="Numerical reconstruction" style="width: 200px; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">3. Numerical reconstruction</figcaption>
    </figure>
  </div>
  <div style="display: flex; flex-direction: column;gap: 10px;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image6.jpeg" alt="Acquired images" style="width: 135px; height: auto; margin-bottom: 10px; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">4. Positioning of x,y</figcaption>
    </figure>
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image8.gif" alt="Numerical reconstruction" style="width: 225px; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">5. Depth-wise positioning</figcaption>
    </figure>
  </div>
</div>

(조금 작은 글씨로) 이 피규어들은 고태식 교수의 Label-free sensor for automatic identification of erythrocytes using digital in-line holographic microscopy and machine learning을 참고했다.

<!--
<div style="display: flex; align-items: center;">
  <figure style="margin: 0; text-align: center;">
    <img src="/Research/figures/DIHMsetup.jpg" alt="Experimental setup" style="max-width: 60%; height: auto; display: block; margin: 0 auto;">
    <figcaption style="font-size: 0.9em; color: #555;">Experimental setup</figcaption>
  </figure>
  <div style="display: flex; flex-direction: column;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image3.gif" alt="Acquired images" style="max-width: 170%; height: auto; margin-bottom: 10px; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">Acquired images</figcaption>
    </figure>
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image5.gif" alt="Numerical reconstruction" style="max-width: 80%; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">Numerical reconstruction</figcaption>
    </figure>
  </div>
  <div style="display: flex; flex-direction: column;">
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image6.jpeg" alt="Acquired images" style="max-width: 100%; height: auto; margin-bottom: 10px; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">Positioning of x,y</figcaption>
    </figure>
    <figure style="margin: 0; text-align: center;">
      <img src="/Research/figures/image8.gif" alt="Numerical reconstruction" style="max-width: 110%; height: auto; display: block; margin: 0 auto;">
      <figcaption style="font-size: 0.9em; color: #555;">Depth-wise positioning</figcaption>
    </figure>
  </div>
</div>
-->
<!--Poole is the Jekyll Butler, serving as an upstanding and effective foundation for Jekyll themes by [@mdo](https://github.com/mdo). Poole, and all its derivatives (like Celeste) includes the following:

* Complete Jekyll setup included (layouts, config, [404]({{ site.baseurl }}/404.html), [RSS feed]({{ site.baseurl }}/atom.xml), posts, and a [sample page]({{ site.baseurl }}/about/))
* Mobile friendly design and development
* Easily scalable text and component sizing with `rem` units in the CSS
* Support for a wide gamut of HTML elements
* Syntax highlighting, courtesy of [rouge](https://github.com/jneen/rouge)
-->

### Utilized Artificial Intelligence (AI) Model

DIHM은 강력한 imaging tool이지만, 몇개의 limitation이 존재한다. 인공지능은 이런 한계에 breakthrough를 제공한다. 내 연구에서는 CAE랑 CNN을 사용했으며, 연구를 통해서 dataset을 생성해야 하는 문제를 해결하기 위해 현재는 physics driven unsupervised learning을 연구하고 있다. CAE는 unsupervised learning으로서, 적혈구 사진을 input으로 학습시킨 CAE모델은 latent space에서 뽑아낸 feature를 사용해 각도를 학습시키거나 data augmentation에 사용되었다. 아래 사진은 사용된 network중 1개의 schemetic이다.
<img src="/Research/figures/AI1.png" alt= "CAE model">

적혈구 연구에서 CNN network는 input으로 적혈구의 image, output으로 적혈구의 각도 라벨을 주어서 세포의 orientation을 예측하는데 사용된다. 아래 사진은 1개의 figure다. (여기 AI2 figure 넣고)
<img src="/Research/figures/AI2.png" alt= "CNN model">

The supervised learning model partially overcame the limitations of DIHM. However, each time we study new samples, we must rebuild the dataset, which requires significant time and computational cost for data collection and model training. To address this problem, we need an unsupervised learning method. (현재 연구 중)

### <a href="https://www.sciencedirect.com/science/article/pii/S0956566323001744">AI-based analysis of 3D position and orientation of red blood cells using a DIHM</a> 

Published as a co-first author, Biosensors and Bioelectronics (2023/06) : 기여도 적기
<br>적혈구의 회전거동은 질병 진단에 도움이 되며, flow dynamics에 대한 이해를 한층 더 증대시켜줄 수 있다. (어떻게 적혈구 연구하게 되었는지, 왜 이런 셋업이 필요한지)
<img src="/Research/figures/RBC1.png" alt= "Experimental setup">
(인공지능 설명하고) 결과도 설명하기
<img src="/Research/figures/RBC3.png" alt= "Result">
<b>Publication:</b> Y. Kim, J. Kim, E. Seo, S. Lee*, "AI-based analysis of 3D position and orientation of red blood cells using a digital in-line holographic microscopy" Biosensors and Bioelectronics, 2023, 229, 115232 https://doi.org/10.1016/j.bios.2023.115232

### AI-based analysis of 3D position and orientation of red blood cells in a channel flow using a DIHM

In preparation as a co-author : 기여도 적기
<br>Static한 RBC에 대해 관찰했으니 한 발 나아가 channel flow에서 관찰했다.
<img src="/Research/figures/RBCflow1.png" alt= "Experimental setup">
(인공지능 설명하고) 결과도 설명하기
<img src="/Research/figures/RBCflow2.png" alt= "Result">

### Physics-driven neural network based the three-dimensional morphology reconstruction using DIHM (Ongoing project)

Ongoing project
<br> 프로젝트 소개

<!--
* A design and structure with customizability in mind
* A clean, unobstrusive top navigation bar
* A landing page template for showcasing the most important content on your website
* Optimized for compatibility with most reading tools such as [Pocket](https://getpocket.com), [Instapaper](https://www.instapaper.com) and [Feedly](https://feedly.com/).
* Subtle animations on UI elements that give visual feedback when interacting with the page
* Over 500 scalable vector icons, courtesy of [Font Awesome](https://fontawesome.com/v4.7.0/)
-->
<!-- Additional features to follow -->
<!-- * A blog archives page, to allow easy access to old blog entries -->
<!-- * Multiple color schemes, accessible via the `@import` directive 

Check out the [README](https://github.com/nicoelayda/celeste#readme) for more details.

### Browser support

Celeste is by preference a forward-thinking project. It is best viewed on the latest versions of Chrome, Safari, Firefox and Microsoft Edge.

### Download

Celeste is developed on and hosted with GitHub. Head to the [GitHub repository](https://github.com/nicoelayda/celeste) for downloads, bug reports, and features requests.

-->
