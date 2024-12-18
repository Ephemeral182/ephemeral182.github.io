---
layout: page
permalink: /publications/index.html #/publications.html
title: Publications
---

<style>
/* 基础样式优化 */
.custom-link {
  display: inline-block;
  padding: 5px 12px;
  border-radius: 4px;
  text-decoration: none;
  transition: all 0.3s ease;
  margin: 0 5px;
}

.custom-link—project { 
  color: rgb(255,115,227);
  background: rgba(255,115,227,0.1);
}

.custom-link—code { 
  color: rgb(103,100,248);
  background: rgba(103,100,248,0.1);
}

.custom-link—paper { 
  color: rgb(39,207,236);
  background: rgba(39,207,236,0.1);
}

/* 悬停效果增强 */
.custom-link:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

/* 图片容器悬停效果 */
.image-wrapper {
  position: relative;
  overflow: hidden;
  border-radius: 8px;
  transition: all 0.3s ease;
}

/* 添加图片悬停效果和简介 */
.image-wrapper:hover img {
  transform: scale(1.05);
  filter: brightness(0.8);
}

.image-wrapper:hover::after {
  opacity: 1;
}

.image-wrapper::after {
  content: attr(data-description);
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: rgba(0,0,0,0.75);
  color: white;
  padding: 15px;
  font-size: 14px;
  opacity: 0;
  transition: all 0.3s ease;
}

/* 论文标题样式优化 */
papertitle {
  display: block;
  font-size: 1.1em;
  margin: 10px 0;
  line-height: 1.4;
  transition: all 0.3s ease;
}

papertitle:hover {
  color: #2196F3;
}

/* 添加论文类型标签 */
.paper-tag {
  display: inline-block;
  padding: 3px 8px;
  border-radius: 12px;
  font-size: 12px;
  margin: 5px;
  background: #f0f0f0;
  color: #666;
}

/* 添加引用数量徽章 */
.citation-badge {
  display: inline-block;
  padding: 2px 6px;
  border-radius: 10px;
  font-size: 12px;
  background: #e3f2fd;
  color: #1976d2;
  margin-left: 10px;
}

/* 优化表格布局 */
.publication-table {
  width: 100%;
  border-spacing: 0 20px;
  margin: 20px auto;
}

.publication-table tr {
  background: white;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
  transition: all 0.3s ease;
}

.publication-table tr:hover {
  transform: translateY(-3px);
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
}
</style>


# Publications

7&nbsp; ***CVPR*** / ***ICCV*** / ***ECCV*** /  ***NeurIPS*** &nbsp;&nbsp;&nbsp;5&nbsp; ***AAAI*** / ***IJCAI*** / ***ACM MM*** &nbsp;&nbsp;&nbsp; 1&nbsp; ***MICCAI*** &nbsp;&nbsp;&nbsp; 1&nbsp; ***CVPRW*** / ***ICCVW*** / ***ECCVW*** &nbsp;&nbsp;&nbsp;2&nbsp; ***ACCV*** / ***BMVC*** &nbsp;&nbsp;&nbsp;2&nbsp; ***ICME*** / ***ICASSP*** &nbsp;&nbsp;&nbsp;

<!-- =================================================================================== -->
<table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
    <tr>
      <td style="margin:5px;padding:5px;width:35%;max-width:90%" align="center" class="image-wrapper" data-description="NeurIPS'2024">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/nips2024/overview.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
          <papertitle>
            <strong>
              RestoreAgent: Autonomous Image Restoration Agent via Multimodal Large Language Models
            </strong>
          </papertitle>
          <div>
        <span class="paper-tag">Computer Vision</span>
            <span class="paper-tag">Deep Learning</span>
          </div>
          <br>
          Haoyu Chen, Wenbo Li, Jinjin Gu, Jingjing Ren, <strong><u>Sixiang Chen</u></strong>, Tian Ye, Renjing Pei, Kaiwen Zhou, Fenglong Song, Lei Zhu<sup>✉️</sup>.
          <br>  
          <em>Conference on Neural Information Processing Systems <strong>(NeurIPS)</strong></em>, 2024
          <br>
          <a href="https://arxiv.org/abs/2407.18035" class="custom-link—paper">[Paper]</a>
          <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
          <a href="https://haoyuchen.com/RestoreAgent" class="custom-link—project">[Project]</a>
      </td>
    </tr>

<table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
    <tr>
      <td style="margin:5px;padding:5px;width:35%;max-width:90%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/aglldiff.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
          <papertitle>
            <strong>
              AGLLDiff: Guiding Diffusion Models Towards Unsupervised Training-free Real-world Low-light Image Enhancement
            </strong>
          </papertitle>
          <br>
          Yunlong Lin* ,Tian Ye*, <strong><u>Sixiang Chen*</u></strong> ,Zhenqi Fu, Yingying Wang, Wenhao Chai, Zhaohu Xing, Lei Zhu, Xinghao Ding<sup>✉️</sup>.
          <br>  
          <em><strong>Arxiv (Under review)</strong></em>, 2024
          <br>
          <a href="https://arxiv.org/abs/2407.14900" class="custom-link—paper">[Paper]</a>
          <a href="https://aglldiff.github.io/" class="custom-link—code">[Code]</a>
          <a href="https://aglldiff.github.io/" class="custom-link—project">[Project]</a>
      </td>
    </tr>

<table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
    <tr>
      <td style="margin:5px;padding:5px;width:35%;max-width:90%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/eccv_24/eccv_adverse.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
          <papertitle>
            <strong>
              Teaching Tailored to Talent: Adverse Weather Restoration via Prompt Pool and Depth-Anything Constraint
            </strong>
          </papertitle>
          <br>
          <strong><u>Sixiang Chen</u></strong>, Tian Ye, Kai Zhang, Zhaohu Xing, Yunlong Lin, Lei Zhu<sup>✉️</sup>.
          <br>  
          <em>European Conference on Computer Vision <strong>(ECCV)</strong></em>, 2024
          <br>
          <a href="https://arxiv.org/abs/2409.15739" class="custom-link—paper">[Paper]</a>
          <a href="https://github.com/Ephemeral182/ECCV24_T3-DiffWeather" class="custom-link—code">[Code]</a>
          <a href="https://ephemeral182.github.io/T3-DiffWeather/" class="custom-link—project">[Project]</a>
      </td>
    </tr>

<table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
    <tr>
      <td style="margin:5px;padding:5px;width:35%;max-width:90%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/eccv_snow.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
          <papertitle>
            <strong>
              Semi-Supervised Video Desnowing Network via Temporal Decoupling Experts and Distribution-Driven Contrastive Regularization
            </strong>
          </papertitle>
          <br>
          Hongtao Wu, Yijun Yang, Angelica Aviles-Rivero, Jingjing Ren, <strong><u>Sixiang Chen</u></strong>, Haoyu Chen, Lei Zhu<sup>✉️</sup>.
          <br>  
          <em>European Conference on Computer Vision <strong>(ECCV)</strong></em>, 2024
          <br>
          <a href="https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/01500.pdf" class="custom-link—paper">[Paper]</a>
          <a href="https://github.com/TonyHongtaoWu/SemiVDN
          " class="custom-link—code">[Code]</a>
      </td>
    </tr>

<table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
    <tr>
      <td style="margin:5px;padding:5px;width:35%;max-width:90%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/miccai24.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
          <papertitle>
            <strong>
              Cross-conditioned Diffusion Model for medical image-to-image translation
            </strong>
          </papertitle>
          <br>
          Zhaohu Xing, Sicheng Yang, <strong><u>Sixiang Chen</u></strong>, Tian Ye, Lei Zhu<sup>✉️</sup>.
          <br>  
          <em>Medical Image Computing and Computer Assisted Intervention <strong>(MICCAI)</strong></em>, 2024
          <br>
          <a href="https://link.springer.com/chapter/10.1007/978-3-031-72104-5_20" class="custom-link—paper">[Paper]</a>
          <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
    </tr>

<table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
    <tr>
      <td style="margin:5px;padding:5px;width:35%;max-width:90%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/CVPR24.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
          <papertitle>
            <strong>
              Learning Diffusion Texture Priors for Image Restoration
            </strong>
          </papertitle>
          <br>
          Tian Ye, <strong><u>Sixiang Chen</u></strong>, Wenhao Chai, Zhaohu Xing, Jing Qin, Ge Lin, Lei Zhu<sup>✉️</sup>.
          <br>  
          <em>Computer Vision and Pattern Recognition <strong>(CVPR Highlight)</strong></em>, 2024
          <br>
          <a href="https://openaccess.thecvf.com/content/CVPR2024/html/Ye_Learning_Diffusion_Texture_Priors_for_Image_Restoration_CVPR_2024_paper.html" class="custom-link—paper">[Paper]</a>
          <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
    </tr>

<table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
    <tr>
      <td style="margin:5px;padding:5px;width:35%;max-width:90%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/udrs2former.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
          <papertitle>
            <strong>
              Sparse Sampling Transformer with Uncertainty-Driven Ranking for Unified Removal of Raindrops and Rain Streaks
            </strong>
          </papertitle>
          <br>
          <strong><u>Sixiang Chen*</u></strong>, Tian Ye*, Jinbin Bai, Jun Shi, Erkang Chen, Lei Zhu<sup>✉️</sup>.
          <br>  
          <em>International Conference on Computer Vision <strong>(ICCV)</strong></em>, 2023
          <br>
          <a href="https://arxiv.org/abs/2308.14153" class="custom-link—paper">[Paper]</a>
          <a href="https://github.com/Ephemeral182/UDR-S2Former_deraining" class="custom-link—code">[Code]</a>
          <a href="https://ephemeral182.github.io/UDR_S2Former_deraining/" class="custom-link—project">[Project]</a>
      </td>
    </tr>



 <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
          <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/AWRCP_framework.jpg" alt="dise"> 
        </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
        Adverse Weather Removal with Codebook Priors
        </strong>
        </papertitle>
        <br>
        Tian Ye*,<strong><u>Sixiang Chen*</u></strong>, Jinbin Bai, Jun Shi, Chenghao Xue, Jingjia Jiang, Junjie Yin, Erkang Chen, Yun Liu<sup>✉️</sup>.
        <br>  
        <em>International Conference on Computer Vision <strong>(ICCV)</strong></em>, 2023
        <br>
        <a href="Ephemeral182.github.io" class="custom-link—paper">[Paper]</a>
        <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
      </tr>

      

  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/Uncertainty_MM.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          Uncertainty-Driven Dynamic Degradation Perceiving and Background Modeling for Efficient Single Image Desnowing
        </strong>
        </papertitle>
        <br>
        <strong><u>Sixiang Chen*</u></strong>, Tian Ye*, Chenghao Xue*, Haoyu Chen, Yun Liu, Erkang Chen, Lei Zhu<sup>✉️</sup>.
        <br>  
        <em>ACM Multimedia <strong>(ACM MM)</strong></em>, 2023
        <br>
        <a href="Ephemeral182.github.io" class="custom-link—paper">[Paper]</a>
        <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
      </tr>



  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/cpl.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          CPLFormer: Cross-scale Prototype Learning Transformer for Image Snow Removal
        </strong>
        </papertitle>
        <br>
        <strong><u>Sixiang Chen*</u></strong>, Tian Ye*, Yun Liu, Jinbin Bai, Haoyu Chen, Yunlong Lin, Jun Shi, Erkang Chen<sup>✉️</sup>.
        <br>  
        <em>ACM Multimedia <strong>(ACM MM)</strong></em>, 2023
        <br>
        <a href="Ephemeral182.github.io" class="custom-link—paper">[Paper]</a>
       <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
      </tr>



  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/video.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          Sequential Affinity Learning for Video Restoration
        </strong>
        </papertitle>
        <br>
        Tian Ye*,<strong><u>Sixiang Chen*</u></strong>, Yun Liu<sup>✉️</sup>, Wenhao Chai, Jinbin Bai, Wenbin Zou, Yunchen Zhang, jiang mingchao, Erkang Chen, Chenghao Xue.
        <br>  
        <em>ACM Multimedia <strong>(ACM MM)</strong></em>, 2023
        <br>
        <a href="Ephemeral182.github.io" class="custom-link—paper">[Paper]</a>
        <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
      </tr>



  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/Nightformer.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          NightHazeFormer: Single Nighttime Haze Removal Using Prior Query Transformer
        </strong>
        </papertitle>
        <br>
        Yun Liu, Zhongsheng Yan, <strong><u>Sixiang Chen</u><sup>✉️</sup></strong>, Tian Ye<sup>✉️</sup>, Wenqi Ren, Erkang Chen.
        <br>  
        <em>ACM Multimedia <strong>(ACM MM)</strong></em>, 2023
        <br>
        <a href="http://export.arxiv.org/abs/2305.09533#:~:text=propose%20an%20end-to-end%20transformer-based%20framework%20for%20nighttime%20haze,we%20introduce%20two%20powerful%20priors%20into%20the%20transformer" class="custom-link—paper">[Paper]</a>
        <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
      </tr>



  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/BMVC.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          Five A+ Network: You Only Need 9K Parameters for Underwater Image Enhancement
        </strong>
        </papertitle>
        <br>
        Jingxia Jiang*, Tian Ye*, Jinbin Bai*, <strong><u>Sixiang Chen</u></strong>, Wenhao Chai, Jun Shi, Yun Liu, Erkang Chen<sup>✉️</sup>.
        <br>  
        <em>British Machine Vision Conference (BMVC)</em>, 2023
        <br>
        <a href="https://arxiv.org/abs/2305.08824#:~:text=In%20this%20work%2C%20we%20propose%20the%20Five%20A,The%20FA%20Net%20employs%20a%20two-stage%20enhancement%20structure." class="custom-link—paper">[Paper]</a>
        <a href="https://github.com/Owen718/FiveAPlus-Network" class="custom-link—code">[Code]</a>
      </td>
      </tr>



  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/dehrformer_00.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          DEHRFormer: Real-time Transformer for Depth Estimation and Haze Removal from Varicolored Haze Scenes
        </strong>
        </papertitle>
        <br>
        <strong><u>Sixiang Chen*</u></strong>, Tian Ye*, Jun Shi, Yun Liu, JingXia Jiang, Erkang Chen, Peng Chen<sup>✉️</sup>.
        <br>  
        <em>International Conference on Acoustics, Speech, and Signal Processing <strong>(ICASSP)</strong></em>, 2023
        <br>
        <a href="https://ieeexplore.ieee.org/abstract/document/10096828" class="custom-link—paper">[Paper]</a>
        <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
      </tr>



  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/MSP-Former_00.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          MSP-Former: Multi-Scale Projection Transformer for Single Image Desnowing
        </strong>
        </papertitle>
        <br>
        <strong><u>Sixiang Chen*</u></strong>, Tian Ye*, Yun Liu, Taodong Liao, Jingxia Jiang, Erkang Chen, Peng Chen<sup>✉️</sup>.
        <br>  
        <em>International Conference on Acoustics, Speech, and Signal Processing <strong>(ICASSP)</strong></em>, 2023
        <br>
        <a href="https://ieeexplore.ieee.org/abstract/document/10095605" class="custom-link—paper">[Paper]</a>
        <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
      </tr>



  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/snowformer.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          SnowFormer: Context Interaction Transformer with Scale-awareness for Single Image Desnowing
        </strong>
        </papertitle>
        <br>
        <strong><u>Sixiang Chen*</u></strong>, Tian Ye*, Yun Liu, Erkang Chen<sup>✉️</sup>.
        <br>  
        <em>Arxiv (Under review)</em>, 2022
        <br>
        <a href="https://arxiv.org/abs/2208.09703#:~:text=SnowFormer%3A%20Context%20Interaction%20Transformer%20with%20Scale-awareness%20for%20Single,image%20desnowing%20is%20a%20challenging%20image%20restoration%20task." class="custom-link—paper">[Paper]</a>
        <a href="https://github.com/Ephemeral182/SnowFormer" class="custom-link—code">[Code]</a>
      </td>
      </tr>



  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/ACCV.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          Towards Real-time High-Definition Image Snow Removal: Efficient Pyramid Network with Asymmetrical Encoder-decoder Architecture
        </strong>
        </papertitle>
        <br>
        Tian Ye*, <strong><u>Sixiang Chen*</u></strong>, Yun Liu, Yi Ye, Erkang Chen<sup>✉️</sup>.
        <br>  
        <em>Asian Conference on Computer Vision <strong>(ACCV)</strong></em>, 2022
        <br>
        <a href="Ephemeral182.github.io" class="custom-link—paper">[Paper]</a>
        <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
      </tr>



  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/dualformer.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          Dual-former: Hybrid Self-attention Transformer for
          Efficient Image Restoration
        </strong>
        </papertitle>
        <br>
        <strong><u>Sixiang Chen</u></strong>, Tian Ye, Yun Liu, Erkang Chen<sup>✉️</sup>.
        <br>  
        <em>Digital Signal Processing</em>, 2024
        <br>
        <a href="https://www.sciencedirect.com/science/article/pii/S1051200424001106" class="custom-link—paper">[Paper]</a>
        <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
      </td>
      </tr>



  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/ECCV.png" alt="dise"> 
      </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          Perceiving and Modeling Density for Image Dehazing
        </strong>
        </papertitle>
        <br>
        Tian Ye*, Mingchao Jiang*, Yunchen Zhang*, Liang Chen, Yun Liu, <strong><u>Sixiang Chen</u></strong>, Erkang Chen<sup>✉️</sup>.
        <br>  
        <em>European Conference on Computer Vision <strong>(ECCV Oral)</strong></em>, 2022
        <br>
        <a href="https://link.springer.com/chapter/10.1007/978-3-031-19800-7_8" class="custom-link—paper">[Paper]</a>
        <a href="https://github.com/Owen718/ECCV22-Perceiving-and-Modeling-Density-for-Image-Dehazing" class="custom-link—code">[Code]</a>
      </td>
      </tr>


  <tr>
        <td style="margin:5px;padding:5px;width:35%;max-width:40%" align="center" class="image-wrapper">
        <img style="margin:1px;padding-right:20px;width:100%;max-width:100%" src="https://ephemeral182.github.io/images/CVPRW.png" alt="dise"> 
        </td>
      <td width="75%" valign="center" class="text-wrapper"> 
        <papertitle>
        <strong>
          Underwater Light Field Retention: Neural Rendering for Underwater Imaging
        </strong>
        </papertitle>
        <br>
        Tian Ye*, <strong><u>Sixiang Chen*</u></strong>, Yun Liu, Yi Ye, Erkang Chen<sup>✉️</sup>, Yuche Li.
        <br>  
        <em>Conference on Computer Vision and Pattern Recognition Workshop <strong>(CVPRW)</strong></em>, 2022
        <br>
        <a href="https://ieeexplore.ieee.org/document/9857150" class="custom-link—paper">[Paper]</a>
        <a href="https://github.com/Ephemeral182/UWNR" class="custom-link—code">[Code]</a>
      </td>
      </tr>
  </tbody>
</table>

<!-- =================================================================================== -->



---


