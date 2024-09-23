---
layout: post1
permalink: /T3-DiffWeather/index.html #/publications.html
title: T3_DiffWeather
---

<link rel="stylesheet" href="assets/css/bulma-carousel.min.css">
<link rel="stylesheet" href="assets/css/bulma-slider.min.css">
<link rel="stylesheet" href="assets/css/fontawesome.all.min.css">
<link rel="stylesheet" href="assets/css/academicons.min.css">
<link rel="stylesheet" href="assets/css/index.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">

<h2 class="post-title" style="color: #228be6; margin-bottom:7px; margin-top:20px; font-weight:400;">
  Teaching Tailored to Talent: Adverse Weather Restoration via Prompt Pool and Depth-Anything Constraint
</h2>

<div class="post-authors" style="margin-bottom:5px;">
  <a href="https://ephemeral182.github.io">Sixiang Chen</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://owen718.github.io">Tian Ye</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
  Kai Zhang<sup>1</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://ge-xing.github.io/">Zhaohu Xing</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://lyl1015.github.io/">Yunlong Lin</a><sup>2</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://sites.google.com/site/indexlzhu/home">Lei Zhu</a><sup>1,3 ✉️</sup>&nbsp;&nbsp;&nbsp;
</div>

<div class="post-affiliations" style="margin-bottom:20px;">
  <sup>1</sup>The Hong Kong University of Science and Technology (Guangzhou)&nbsp;&nbsp;&nbsp;
  <sup>2</sup>Xiamen University&nbsp;&nbsp;&nbsp;<br>
  <sup>3</sup>The Hong Kong University of Science and Technology&nbsp;&nbsp;&nbsp;         
</div>

<div class="post-conference" style="margin-bottom:20px;">
  European Conference on Computer Vision <strong>(ECCV)</strong>, 2024, MiCo Milano
</div>

<div class="post-icons">
  <ul class="nav nav-pills nav-justified">
    <li>
      <a href="https://ephemeral182.github.io">
        <img class="post-logo" src="https://ephemeral182.github.io/images/paper.jpg" height="50px">
        <h5><strong>arXiv</strong></h5>
      </a>
    </li>
    <li>
      <a href="https://ephemeral182.github.io/UDR_S2Former_deraining/">
        <img class="post-logo" src="https://ephemeral182.github.io/images/paper.jpg" height="50px">
        <h5><strong>ECCV 2024</strong></h5>
      </a>
    </li>
    <li>
      <a href="https://ephemeral182.github.io/UDR_S2Former_deraining/">
        <img class="post-logo" src="https://ephemeral182.github.io/images/datatset.jpg" height="50px">
        <h5><strong>Dataset</strong></h5>
      </a>
    </li>
    <li>
      <a href="https://ephemeral182.github.io">
        <img class="post-logo" src="https://ephemeral182.github.io/images/github.png" height="50px">
        <h5><strong>Code</strong></h5>
      </a>
    </li>
    <li>
      <a href="https://ephemeral182.github.io/">
        <img class="post-logo" src="https://ephemeral182.github.io/images/supplementary.jpg" height="50px">
        <h5><strong>Supplementary</strong></h5>
      </a>
    </li>
  </ul>
</div>

<div class="post-line"></div>

<section class="section">
  <div class="container">
    <div class="content has-text-centered">
      <h2 class="title is-3">Visual Comparisons</h2>
      <div class="columns is-centered">
        <div class="column is-full-width">
          <div id="example1" class="bal-container-small">
            <div class="bal-after">
              <img src="images/eccv_24/eccv_adverse_real.png">
              <div class="bal-afterPosition afterLabel">Ours</div>
            </div>
            <div class="bal-before" style="width:50.5%;">
              <div class="bal-before-inset">
                <img src="images/eccv_24/eccv_adverse_real.png">
                <div class="bal-beforePosition beforeLabel">Input</div>
              </div>
            </div>
            <div class="bal-handle" style="left:50.5%;">
              <span class="handle-left-arrow"></span>
              <span class="handle-right-arrow"></span>
            </div>
          </div>
          <!-- 添加更多图片或其他视觉比较部分 -->
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2 class="post-section" style="text-align: center; padding-top: 20px;">Abstract</h2>
    <p style="padding: 25px; padding-top: 10px;">
      Recent advancements in adverse weather restoration have shown potential, yet the unpredictable and varied combinations of weather degradations in the real world pose significant challenges...
    </p>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2 class="post-section" style="text-align: center; padding-top: 20px;">Method</h2>
    <div class="post-img-group">
      <img class="post-img" style="max-width:100%" src="https://ephemeral182.github.io/images/eccv_adverse.png" alt="Method Image">
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2 class="post-section" style="text-align: center; padding-top: 20px;">Quantitative Comparison</h2>
    <div class="post-img-group">
      <img class="post-img" style="max-width:100%;" src="https://ephemeral182.github.io/images/eccv_adverse_metric.png" alt="Metric Image">
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2 class="post-section" style="text-align: center; padding-top: 20px;">Visual Comparison</h2>
    <div class="post-img-group">
      <img class="post-img" style="max-width:100%;" src="https://ephemeral182.github.io/images/eccv_24/eccv_adverse_syn.png" alt="Syn Image">
      <img class="post-img" style="max-width:100%;" src="https://ephemeral182.github.io/images/eccv_24/eccv_adverse_real.png" alt="Real Image">
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2 class="post-section">Citation</h2>
    <pre>
@InProceedings{chen2024teaching,
    title     = {Teaching Tailored to Talent: Adverse Weather Restoration via Prompt Pool and Depth-Anything Constraint},
    author    = {Chen, Sixiang and Ye, Tian and Zhang, Kai and Xing, Zhaohu and Lin, Yunlong and Zhu, Lei}, 
    booktitle = {European conference on computer vision},
    year      = {2024},
    organization={Springer}
}
    </pre>
  </div>
</section>
