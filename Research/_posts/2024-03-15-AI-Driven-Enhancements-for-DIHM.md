---
layout: post
title: AI-Driven Enhancements for DIHM
---

<h2> Research 3. <br> 3D Morphology Reconstruction Using a Neural Fields from a Single DIHM Image - Ongoing Project</h2>
Although previous studies have reached a new state with the aid of AI in DIHM field, the fundamental limitations of DIHM remain unsolved. Due to the loss of phase information during the image acquisition process, DIHM experiences the <strong>twin-image problem</strong>. This problem arises due to the inherent generation of a conjugate signal during numerical reconstruction, which significantly degrades the resolution and quality of the image.
<br>Additionally, the <strong>data-driven approach of supervised learning lacks generalization capabilities</strong>, necessitating the creation of new datasets each time the research subject changes. Self-supervised learning presents a promising alternative to this issue.
<br>In this project, a <strong>physics-driven and self-supervised learning approach is utilized to address these limitations</strong>. A coordinate-based neural network with implicit representation is trained to learn the 3D structure of the object. The input consists of coordinates, while the output represents the real part of the corresponding refractive index. These output features are then mapped to the target object image through a forward model which is the angular spectrum method. The network is trained to minimize the difference between the simulated image and the target image. <strong>The goal of the model is to reconstruct the 3D refractive index of an object from a single image.</strong>
