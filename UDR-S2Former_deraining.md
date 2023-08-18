---
layout: post1
permalink: /UDR-S2Former_deraining/index.html #/publications.html
title: Projects
---


<h2 class="post-title" style="margin-bottom:7px;margin-top:20px;font-weight:400;">Sparse Sampling Transformer with Uncertainty-Driven Ranking for </h2>
<h2 class="post-title" style="margin-bottom:20px;margin-top:7px;">Unified Removal of Raindrops and Rain Streaks</h2> 

<div class="post-authors" style="margin-bottom:5px;">
<a href="https://owen718.github.io"><strong>Sixiang Chen</strong></a><sup>1,3</sup>*&nbsp;&nbsp;&nbsp; <a href="https://owen718.github.io">Tian Ye</a><sup>1,3</sup>*&nbsp;&nbsp;&nbsp;
<a href="https://noyii.github.io">Jinbin Bai</a><sup>2</sup>*&nbsp;&nbsp;&nbsp;
<a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=hWo1RTsAAAAJ">Erkang Chen</a><sup>3</sup>*&nbsp;&nbsp;&nbsp;
Jun Shi<sup>4</sup>*&nbsp;&nbsp;&nbsp;
<a href="https://sites.google.com/site/indexlzhu/home">Lei Zhu</a><sup>1,5 ✉️</sup>&nbsp;&nbsp;&nbsp;
<br>
<sup>1</sup>The Hong Kong University of Science and Technology (Guangzhou)&nbsp;&nbsp;&nbsp;
<sup>2</sup>National University of Singapore&nbsp;&nbsp;&nbsp;<br>
<sup>3</sup>School of Ocean Information Engineering, Jimei University&nbsp;&nbsp;&nbsp;             
<sup>4</sup>Xinjiang University&nbsp;&nbsp;&nbsp; 
<sup>5</sup>The Hong Kong University of Science and Technology&nbsp;&nbsp;&nbsp;         
</div>

<div class="post-authors" style="margin-bottom:20px;">
International Conference on Computer Vision <strong>(ICCV)</strong>, 2023
</div>


<div class="post-line"></div>

<div class="post-img-group">
    <img class="post-img" style="max-width:48%" src="https://ephemeral182.github.io/images/real_gif1.gif" alt="Left Image">&nbsp;&nbsp;
    <img class="post-img" style="max-width:48%" src="https://ephemeral182.github.io/images/real_gif2.gif" alt="Right Image">
  </div> 



  <!-- <div class="post-img-group">
    <img class="post-img" src="../assets/img/VideoDesnowing/1.gif" alt="Left Image">
    <img class="post-img" src="../assets/img/VideoDesnowing/2.gif" alt="Right Image">
  </div> -->

<!-- <img src="../assets/img/VideoDesnowing/1.gif" class="post-img" role="img"> -->


<h2 class="post-section">Abstract</h2>

In the real world, image degradations caused by rain often exhibit a combination of rain streaks and raindrops, thereby increasing the challenges of recovering the underlying clean image. Note that the rain streaks and raindrops have diverse shapes, sizes, and locations in the captured image, and thus modeling the correlation relationship between irregular degradations caused by rain artifacts is a necessary prerequisite for image deraining. 
This paper aims to present an efficient and flexible mechanism to learn and model degradation relationships in a global view, thereby achieving a unified removal of intricate rain scenes. 
To do so, we propose a <u>S</u>parse <u>S</u>ampling Trans<u>former</u> based on <u>U</u>ncertainty-<u>D</u>riven <u>R</u>anking, dubbed **UDR-S<sup>2</sup>Former**. 
Compared to previous methods, our UDR-S<sup>2</sup>Former has three merits. First, it can adaptively sample relevant image degradation information to model underlying degradation relationships. 
Second, explicit application of the uncertainty-driven ranking strategy can facilitate the network to attend to degradation features and understand the reconstruction process. 
Finally, experimental results show that our UDR-S<sup>2</sup>Former clearly outperforms state-of-the-art methods for all benchmarks.


  <div class="post-img-group">
    <img class="post-img" style="max-width:100%" src="https://ephemeral182.github.io/images/uncertainty_map.png" alt="Left Image">
  </div>

<div class="post-img-group">
    <img class="post-img" style="max-width:50%" src="https://ephemeral182.github.io/images/udr_overview1.png" alt="Left Image">
    <img class="post-img" style="max-width:50%" src="https://ephemeral182.github.io/images/udr_overview2.png" alt="Right Image">
  </div> 


  <div class="post-img-group">
    <img class="post-img" style="max-width:100%" src="https://ephemeral182.github.io/images/metric.png"  alt="Left Image">
  </div>

<h2 class="post-section"  style="font-weight:300;"><strong>R</strong>ealistic <strong>V</strong>ideo De<strong>S</strong>nowing <strong>D</strong>ataset</h2>

- <strong>RVSD</strong> contains a total of 110 pairs of videos. 
- Each pair contains <strong>snowy</strong> and  <strong>hazy</strong> videos and corresponding snow-free and haze-free ground truth videos. 
- We use a rendering engine (Unreal Engine 5) and various augmentation techniques to generate snow and haze with diverse and realistic physical properties. This results in more realistic and varied synthesized videos, which improve the model’s performance on real-world data. 



<div class="post-section"  style="font-weight:700;">Download</div>
<!-- <div style="font-weight:300;">Train (100 videos):  [Google Drive]  [Baidu Netdisk (password: 7t74)]</div>
<div style="font-weight:300;">Test (20 videos):  [Google Drive]  [Baidu Netdisk (password: 7t74)] </div> -->



- **Train (80 videos):**  
    [Google Drive]  [Baidu Netdisk (password: 7t74)]
- **Test (30 videos):**  
    [Google Drive]  [Baidu Netdisk (password: 7t74)]

<h2 class="post-section">Citation</h2>


```
@inproceedings{chen2023deraining,
  title={Snow Removal in Video: A New Dataset and A Novel Method},
  author={Chen, Sixiang and Ye, Tian and Bai, Jinbin and Chen, Erkang and Shi, Jun and Zhu, Lei},
  booktitle={Proceedings of the IEEE/CVF International Conference on Computer Vision},
  year={2023}
}
```