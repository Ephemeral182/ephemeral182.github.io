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
<style>
body {
  background-color: #1a3c6e; /* 深蓝色背景 */
  color: #ffffff; /* 白色文字，确保可读性 */
}
  .fade-in {
    opacity: 0;
    transform: translateY(20px);
    transition: opacity 0.5s ease-out, transform 0.5s ease-out;
  }
  .fade-in.visible {
    opacity: 1;
    transform: translateY(0);
  }
</style>
  <!-- <link rel="icon" href="./static/images/favicon.svg"> -->

<h2 class="post-title" style="line-height: 1.3; margin-bottom: 20px; font-size: 1.6em;">
  <span style="color: #228be6; display: block; text-align: center; margin-bottom: 7px; font-size: 1.2em;">Teaching Tailored to Talent:</span>
  <span style="display: block; text-align: center; font-size: 1.1em;">Adverse Weather Restoration via Prompt Pool and Depth-Anything Constraint</span>
</h2>
<!-- <h2 class="post-title" style="margin-bottom:20px;margin-top:7px;">Unified Removal of Raindrops and Rain Streaks</h2>  -->

<div class="post-authors" style="margin-bottom:5px;">
<a href="https://ephemeral182.github.io" style="color: #228be6;">Sixiang Chen</a><sup>1</sup>&nbsp;&nbsp;&nbsp; <a href="https://owen718.github.io" style="color: #228be6;">Tian Ye</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
Kai Zhang<sup>1</sup>&nbsp;&nbsp;&nbsp;
<a href="https://ge-xing.github.io/" style="color: #228be6;">Zhaohu Xing</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
<a href="https://lyl1015.github.io/" style="color: #228be6;">Yunlong Lin</a><sup>2</sup>&nbsp;&nbsp;&nbsp;
<a href="https://sites.google.com/site/indexlzhu/home" style="color: #228be6;">Lei Zhu</a><sup>1,3 ✉️</sup>&nbsp;&nbsp;&nbsp;
<br>
<sup>1</sup>The Hong Kong University of Science and Technology (Guangzhou)&nbsp;&nbsp;&nbsp;
<sup>2</sup>Xiamen University&nbsp;&nbsp;&nbsp;<br>
<sup>3</sup>The Hong Kong University of Science and Technology&nbsp;&nbsp;&nbsp;         


<div class="post-authors" style="margin-bottom:20px;">

style="margin-bottom:20px;">
European Conference on Computer Vision <strong>(ECCV)</strong>, 2024, MiCo Milano
</div>


<div style="margin-bottom: 0.7em;" class="post-authors">
                <div class="col-md-8 col-md-offset-2 text-center">
                    <ul class="nav nav-pills nav-justified">
                        <li>
                            <a href="https://ephemeral182.github.io" style="color: #ffffff;">
                            <!-- <a href="https://arxiv.org/abs/2112.05504"> -->
                            <img class="post-logo" src="https://ephemeral182.github.io/images/paper.jpg" height="50px">
                                <h5 style="color: #ffffff;"><strong>arXiv</strong></h5>
                            </a>
                        </li>
                        <li>
                             <a href="https://ephemeral182.github.io/UDR_S2Former_deraining/" style="color: #ffffff;">
                            <img class="post-logo" src="https://ephemeral182.github.io/images/paper.jpg" height="50px">
                                <h5 style="color: #ffffff;"><strong>ECCV 2024</strong></h5>
                            </a>
                        </li>
                        <li>
                             <a href="https://ephemeral182.github.io/UDR_S2Former_deraining/" style="color: #ffffff;">
                            <img class="post-logo" src="https://ephemeral182.github.io/images/datatset.jpg" height="50px">
                                <h5 style="color: #ffffff;"><strong>Dataset</strong></h5>
                            </a>
                        </li>                        
                        <li>
                            <a href="https://ephemeral182.github.io" style="color: #ffffff;">
                            <img class="post-logo" src="https://ephemeral182.github.io/images/github.png" height="50px">
                                <h5 style="color: #ffffff;"><strong>Code</strong></h5>
                            </a>
                        </li>
                        <li>
                             <a href="https://ephemeral182.github.io/" style="color: #ffffff;">
                            <img class="post-logo" src="https://ephemeral182.github.io/images/supplementary.jpg" height="50px">
                                <h5 style="color: #ffffff;"><strong>Supplementery</strong></h5>
                            </a>
                        </li>
                    </ul>
                </div>
        </div>

<div class="post-line"></div>

<!-- <div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)">
<div class="post-img-group">
    <img class="post-img" style="left:0;right:0;margin-bottom:0px;max-width:50%" src="https://ephemeral182.github.io/images/real_gif1.gif" alt="Left Image">
    <img class="post-img" style="left:0;right:0;margin-bottom:0px;max-width:50%" src="https://ephemeral182.github.io/images/real_gif2.gif" alt="Right Image">
  </div> 
  <div class="post-img-group">
    <img class="post-img" style="left:0;right:0;margin-bottom:0;width:100%" src="https://ephemeral182.github.io/images/350.gif" alt="Left Image">
  </div> 
  </div>  -->


<section class="section">
    <div class="container ">
      <div class=" has-text-centered">
         <!-- <h2 class="title is-3">Visual Comparisons</h2> -->
        <div class="content has-text-justified">
          <p>

  </p>
        </div>
        <div class="columns is-centered">
          <!-- Visual Effects. -->
          <div class="column">
            <div class="content">
              <div class="columns is-centered">
                <div class="column is-full-width">
                  <div id="example1" class="bal-container-small">

  <div class="bal-after">
                      <img src="images/eccv_24/eccv_adverse_real.png">
                      <div class="bal-afterPosition afterLabel" style="z-index:1;">
                        Ours
                      </div>
                    </div>

  <div class="bal-before" style="width:50.4968152866242%;">
                      <div class="bal-before-inset" style="width: 539px;">
                        <img src="images/eccv_24/eccv_adverse_real.png">
                        <div class="bal-beforePosition beforeLabel">
                          Input
                        </div>
                      </div>
                    </div>

  <div class="bal-handle" style="left:50.4968152866242%;">
                      <span class=" handle-left-arrow"></span>
                      <span class="handle-right-arrow"></span>
                    </div>

  </div>


  <div id="example2" class="bal-container-small">

  <div class="bal-after">
    <img src="images/eccv_24/eccv_adverse_real.png">
    <div class="bal-afterPosition afterLabel">
      Ours
    </div>
  </div>

  <div class="bal-before" style="width: 50%;">
    <div class="bal-before-inset" style="width: 539px;">
      <img src="images/eccv_24/eccv_adverse_real.png">
      <div class="bal-beforePosition beforeLabel">
        Input
      </div>
    </div>
  </div>

  <div class="bal-handle" style="left: 50%;">
    <span class=" handle-left-arrow"></span>
    <span class="handle-right-arrow"></span>
  </div>

  </div>
</div>
</div>
</div>
</div>


<!--/ Visual Effects. -->

<!-- Matting. -->
<div class="column">
<div class="columns is-centered">
<div class="column content">

<div id="example4" class="bal-container-small">
  <div class="bal-after">
    <img src="images/eccv_24/eccv_adverse_real.png">
    <div class="bal-afterPosition afterLabel" style="z-index:1;">
      Ours
    </div>
  </div>

  <div class="bal-before" style="width:62.10191082802548%;">
    <div class="bal-before-inset" style="width: 539px;">
      <img src="images/eccv_24/eccv_adverse_real.png">
      <div class="bal-beforePosition beforeLabel">
        Input
      </div>
    </div>
  </div>

  <div class="bal-handle" style="left:62.10191082802548%;">
    <span class=" handle-left-arrow"></span>
    <span class="handle-right-arrow"></span>
  </div>

</div>

<div id="example5" class="bal-container-small">
  <div class="bal-after">
    <img src="images/eccv_24/eccv_adverse_real.png">
    <div class="bal-afterPosition afterLabel" style="z-index:1;">
      Ours
    </div>
  </div>

  <div class="bal-before" style="width:56.77179962894249%;">
    <div class="bal-before-inset" style="width: 628px;">
      <img src="images/eccv_24/eccv_adverse_real.png">
      <div class="bal-beforePosition beforeLabel">
        Input
      </div>
    </div>
  </div>

  <div class="bal-handle" style="left:56.77179962894249%;">
    <span class=" handle-left-arrow"></span>
    <span class="handle-right-arrow"></span>
  </div>

</div>
</div>
</div>
</div>
</div>
</div>
</div>
  </section>



  <!-- <div class="post-img-group">
    <img class="post-img" src="../assets/img/VideoDesnowing/1.gif" alt="Left Image">
    <img class="post-img" src="../assets/img/VideoDesnowing/2.gif" alt="Right Image">
  </div> -->

<!-- <img src="../assets/img/VideoDesnowing/1.gif" class="post-img" role="img"> -->


<div class="fade-in" style="background-color:#f0f1f3a6; margin-bottom: 30px; border-radius: 10px;">
  <h2 class="post-section" style="
      text-align: center;
      margin-bottom: 0px;
      padding-top: 20px;
      color: #333;
      font-weight: 600;
  ">Abstract</h2>
  <p style="
      padding: 25px;
      padding-top: 10px;
      line-height: 1.6;
      color: #444;
      text-align: left;
  ">
    Recent advancements in adverse weather restoration have shown potential, yet the unpredictable and varied combinations of weather degradations in the real world pose significant challenges. Previous methods typically struggle with dynamically handling intricate degradation combinations and carrying on background reconstruction precisely, leading to performance and generalization limitations. Drawing inspiration from prompt learning and the "<u>T</u>eaching <u>T</u>ailored to <u>T</u>alent" concept, we introduce a novel pipeline, <i><strong>T<sup>3</sup>-DiffWeather</strong></i>. Specifically, we employ a prompt pool that allows the network to autonomously combine sub-prompts to construct weather-prompts, harnessing the necessary attributes to adaptively tackle unforeseen weather input. Moreover, from a scene modeling perspective, we incorporate general prompts constrained by Depth-Anything feature to provide the scene-specific condition for the diffusion process. Furthermore, by incorporating contrastive prompt loss, we ensures distinctive representations for both types of prompts by a mutual pushing strategy. Experimental results demonstrate that our method achieves state-of-the-art performance across various synthetic and real-world datasets, markedly outperforming existing diffusion techniques in terms of computational efficiency.
  </p>
</div>

<div class="fade-in">
  <h2 class="post-section" style="
      text-align: center;
      padding-left: 25px;
      margin-bottom: 10px;
      padding-top: 20px;
  ">Method</h2>
  <!-- <div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)"> -->
    <div class="post-img-group" style="width: 100%; overflow: hidden;">
      <img class="post-img" style="width: 100%; height: auto; display: block;" src="https://ephemeral182.github.io/images/eccv_24/eccv_adverse_overview.png" alt="Method Overview">
    </div>
    <div style="text-align: center; padding: 10px; font-family: 'Arial', sans-serif; font-size: 14px; color: #333; width: 100%; box-sizing: border-box;">
      <strong>Figure 2.</strong> The overview of proposed method. (a) showcases our pipeline, which adopts an innovative strategy focused on learning degradation residual and employs the information-rich condition to guide the diffusion process. (b) illustrates the utilization of our prompt pool, which empowers the network to autonomously select attributes needed to construct adaptive weather-prompts. (c) depicts the general prompts directed by Depth-Anything constraint to supply scene information that aids in reconstructing residuals. (d) shows the contrastive prompt loss, which exerts constraints on prompts driven by two distinct motivations, enhancing their representations.
    </div>
  </div>




<div class="fade-in">
<h2 class="post-section" style="
    text-align: center;
    padding-left: 25px;
    margin-bottom: 10px;
    padding-top: 20px;
">Quantitative Comparison</h2>
<!-- <div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)"> -->
  <div class="post-img-group">
    <img class="post-img" style="max-width:100%;margin-bottom:0;" src="https://ephemeral182.github.io/images/eccv_24/eccv_adverse_metric.png"  alt="Left Image">
  </div>
  <!-- </div> -->
  <!-- </div> -->

<style>
.scroll-container {
  width: 100%;
  overflow-x: auto;
  white-space: nowrap;
  margin-bottom: 10px;
  -webkit-overflow-scrolling: touch;
  scrollbar-width: thin;
  scrollbar-color: #888 #f1f1f1;
  position: relative;
}

.scroll-container::-webkit-scrollbar {
  height: 10px;
}

.scroll-container::-webkit-scrollbar-track {
  background: #f1f1f1;
}

.scroll-container::-webkit-scrollbar-thumb {
  background: #888;
  border-radius: 5px;
}

.scroll-container::-webkit-scrollbar-thumb:hover {
  background: #555;
}

.scroll-content {
  display: inline-flex;
  padding: 10px 0;
}

.scroll-content img {
  height: 300px;
  margin-right: 20px;
  flex-shrink: 0;
}

.scroll-hint {
  position: absolute;
  bottom: 20px;
  right: 20px;
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
  padding: 5px 10px;
  border-radius: 5px;
  font-size: 14px;
}

.scroll-instruction {
  text-align: center;
  font-style: italic;
  color: #666;
  margin-bottom: 20px;
}
</style>

<div class="fade-in">
  <h2 class="post-section" style="
      text-align: center;
      padding-left: 25px;
      margin-bottom: 10px;
      padding-top: 20px;
  ">Visual Comparison</h2>
  <div class="scroll-container">
    <div class="scroll-content">
      <img src="https://ephemeral182.github.io/images/eccv_24/eccv_adverse_syn.png" alt="Image 1">
      <img src="https://ephemeral182.github.io/images/eccv_24/eccv_adverse_real.png" alt="Image 2">
      <img src="https://ephemeral182.github.io/images/eccv_24/visual_real_comparison2.png" alt="Image 3">
      <img src="https://ephemeral182.github.io/images/eccv_24/visual_real_comparison3.png" alt="Image 4">
      <img src="https://ephemeral182.github.io/images/eccv_24/visual_real_comparison4.png" alt="Image 5">
      <img src="https://ephemeral182.github.io/images/eccv_24/visual_real_comparison5.png" alt="Image 6">
    </div>
    <div class="scroll-hint">Scroll ➜</div>
  </div>
  <div class="scroll-instruction">Scroll horizontally to view more images</div>
</div>


 <!-- <div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)">   -->
<div class="post-img-group">
<iframe style="max-width:50%;margin-top:0px;text-align: left;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="250"  src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=1486a714-3ea3-11ee-b5bd-6595d9b17862"></iframe>
<iframe style="max-width:50%;margin-bottom:0px;text-align: right;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="250" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=209744e0-3ea4-11ee-b5bd-6595d9b17862"></iframe>
</div> 
<div class="post-img-group">
<iframe style="max-width:50%;margin-top:0px;text-align: left;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="250"  src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=c58fedd2-3f3d-11ee-b5bd-6595d9b17862"></iframe>
<iframe style="max-width:50%;margin-bottom:0px;text-align: right;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="250" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=0ded7a4a-3f3e-11ee-b5bd-6595d9b17862"></iframe>
</div> 
<div class="post-img-group">
<iframe style="max-width:100%;margin-bottom:0px;text-align: right;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="100%" height="371" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=2ad2a594-3f3f-11ee-b5bd-6595d9b17862"></iframe>
</div>
<!-- </div> -->
<!-- </div> -->

<!-- <div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)">
<div class="post-img-group">
<img style="padding: 10px; width: 450;text-align: left;" frameborder="0" class="juxtapose" height="455" width="600" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=ae97ac46-3ea2-11ee-b5bd-6595d9b17862">
<img style="padding: 10px; width: 450;text-align: right;" frameborder="0" class="juxtapose" height="455" width="600" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=5b6cf096-3e7d-11ee-b5bd-6595d9b17862">
</div> 
</div>  -->

<!-- <div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)">
<div class="post-img-group">
    <img class="post-img" style="left:0;right:0;margin-bottom:0px;max-width:50%;height:70" src="https://ephemeral182.github.io/images/real3.gif" alt="Left Image"><!--&nbsp;&nbsp;
    <img class="post-img" style="left:0;right:0;margin-bottom:0px;max-width:50%;height:70" src="https://ephemeral182.github.io/images/real4.gif" alt="Right Image">
  </div> 
</div>  -->

<!-- <h2 class="post-section"  style="font-weight:300;"><strong>R</strong>ealistic <strong>V</strong>ideo De<strong>S</strong>nowing <strong>D</strong>ataset</h2>

- <strong>RVSD</strong> contains a total of 110 pairs of videos. 
- Each pair contains <strong>snowy</strong> and  <strong>hazy</strong> videos and corresponding snow-free and haze-free ground truth videos. 
- We use a rendering engine (Unreal Engine 5) and various augmentation techniques to generate snow and haze with diverse and realistic physical properties. This results in more realistic and varied synthesized videos, which improve the model's performance on real-world data. 



<div class="post-section"  style="font-weight:700;">Download</div>
<!-- <div style="font-weight:300;">Train (100 videos):  [Google Drive]  [Baidu Netdisk (password: 7t74)]</div>
<div style="font-weight:300;">Test (20 videos):  [Google Drive]  [Baidu Netdisk (password: 7t74)] </div> -->



<!-- - **Train (80 videos):**  
    [Google Drive]  [Baidu Netdisk (password: 7t74)]
- **Test (30 videos):**  
    [Google Drive]  [Baidu Netdisk (password: 7t74)] --> 

<h2 class="post-section">Citation</h2>


````
@InProceedings{chen2024teaching,
    title     = {Teaching Tailored to Talent: Adverse Weather Restoration via Prompt Pool and Depth-Anything Constraint},
    author    = {Chen, Sixiang and Ye, Tian and Zhang, Kai and Xing, Zhaohu and Lin, Yunlong and Zhu, Lei}, 
    booktitle = {European conference on computer vision},
    year      = {2024},
    organization={Springer}
}
````

<script>
  function handleScroll() {
    const elements = document.querySelectorAll('.fade-in');
    elements.forEach(element => {
      const rect = element.getBoundingClientRect();
      const windowHeight = window.innerHeight || document.documentElement.clientHeight;
      if (rect.top <= windowHeight * 0.75) {
        element.classList.add('visible');
      }
    });
  }

  window.addEventListener('scroll', handleScroll);
  window.addEventListener('load', handleScroll);
</script>