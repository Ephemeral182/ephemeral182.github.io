---
layout: page
permalink: /publications/index.html #/publications.html
title: Publications
---

<style>
/* 整体背景色 */
body {
  background-color: #f0f5fa;  /* 非常淡的蓝色背景 */
}

/* 摘要部分样式 */
.summary-section {
  background: rgba(255, 255, 255, 0.9);
  padding: 30px;
  border-radius: 16px;
  margin-bottom: 40px;
  box-shadow: 0 4px 15px rgba(0,0,0,0.05);
}

.summary-stats {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin: 20px 0;
}

.stat-item {
  background: #fff;
  padding: 15px 25px;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
}

/* 年份分隔样式 */
.year-section {
  margin: 50px 0;
}

.year-divider {
  display: flex;
  align-items: center;
  margin: 40px 0;
}

.year-2024 { color: #2196F3; }  /* 蓝色 */
.year-2023 { color: #00BCD4; }  /* 青色 */
.year-2022 { color: #4CAF50; }  /* 绿色 */

.year-divider::after {
  content: '';
  flex: 1;
  height: 2px;
  margin-left: 20px;
  background: linear-gradient(90deg, currentColor, transparent);
}

/* 论文类型标签样式优化 */
.paper-tag {
  display: inline-block;
  padding: 4px 12px;
  border-radius: 12px;
  font-size: 12px;
  margin: 5px;
}

.tag-top { 
  background: rgba(33,150,243,0.1);
  color: #2196F3;
}

.tag-conference {
  background: rgba(0,188,212,0.1);
  color: #00BCD4;
}

.tag-workshop {
  background: rgba(76,175,80,0.1);
  color: #4CAF50;
}

/* 添加图片容器悬停效果 */
.image-wrapper {
  position: relative;
  overflow: hidden;
  border-radius: 12px;
  transition: all 0.3s ease;
}

.image-wrapper:hover {
  transform: scale(1.02);
}

.image-wrapper:hover::before {
  content: attr(data-description);
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: rgba(0, 0, 0, 0.8);
  color: white;
  padding: 15px;
  font-size: 14px;
  opacity: 0;
  transform: translateY(100%);
  animation: slideUp 0.3s forwards;
}

@keyframes slideUp {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* 论文条目样式优化 */
.publication-item {
  background: white;
  border-radius: 16px;
  margin-bottom: 25px;
  transition: all 0.3s ease;
  box-shadow: 0 4px 15px rgba(0,0,0,0.05);
}

.publication-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0,0,0,0.1);
}

/* 链接样式美化 */
.custom-link {
  display: inline-block;
  padding: 6px 12px;
  border-radius: 6px;
  text-decoration: none;
  margin: 0 5px;
  transition: all 0.3s ease;
}

.custom-link—paper {
  color: #2196F3;
  background: rgba(33,150,243,0.1);
}

.custom-link—code {
  color: #4CAF50;
  background: rgba(76,175,80,0.1);
}

.custom-link—project {
  color: #9C27B0;
  background: rgba(156,39,176,0.1);
}

.custom-link:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

/* 更新摘要统计部分的样式 */
.stat-item {
  background: #fff;
  padding: 20px 30px;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
  position: relative;
  transition: all 0.3s ease;
  cursor: pointer;
}

.stat-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0,0,0,0.1);
}

.stat-number {
  font-size: 2.5em;
  font-weight: 700;
  background: linear-gradient(135deg, #2196F3, #00BCD4);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin-bottom: 5px;
}

.stat-label {
  font-size: 0.9em;
  color: #666;
}

/* 统计项悬浮提示 */
.stat-tooltip {
  position: absolute;
  bottom: 100%;
  left: 50%;
  transform: translateX(-50%) translateY(-10px);
  background: rgba(0, 0, 0, 0.8);
  color: white;
  padding: 15px;
  border-radius: 8px;
  font-size: 0.9em;
  opacity: 0;
  visibility: hidden;
  transition: all 0.3s ease;
  width: max-content;
  max-width: 300px;
  box-shadow: 0 4px 15px rgba(0,0,0,0.2);
  z-index: 1000;
}

.stat-item:hover .stat-tooltip {
  opacity: 1;
  visibility: visible;
  transform: translateX(-50%) translateY(0);
}

/* 添加动画效果 */
@keyframes countUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

.stat-number {
  animation: countUp 1s ease-out forwards;
}

/* 论文标签样式优化 */
.paper-tag {
  display: inline-flex;
  align-items: center;
  padding: 6px 12px;
  margin: 4px;
  font-size: 0.85em;
  font-weight: 500;
  border-radius: 20px;
  transition: all 0.3s ease;
  cursor: default;
}

/* 不同类型的标签使用不同的颜色主题 */
.tag-method {
  background: linear-gradient(135deg, rgba(33,150,243,0.1), rgba(33,150,243,0.2));
  color: #2196F3;
  border: 1px solid rgba(33,150,243,0.3);
}

.tag-domain {
  background: linear-gradient(135deg, rgba(156,39,176,0.1), rgba(156,39,176,0.2));
  color: #9C27B0;
  border: 1px solid rgba(156,39,176,0.3);
}

.tag-application {
  background: linear-gradient(135deg, rgba(76,175,80,0.1), rgba(76,175,80,0.2));
  color: #4CAF50;
  border: 1px solid rgba(76,175,80,0.3);
}

/* 悬停效果 */
.paper-tag:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

/* 添加图标支持 */
.paper-tag::before {
  content: '';
  display: inline-block;
  width: 16px;
  height: 16px;
  margin-right: 6px;
  background-size: contain;
  background-repeat: no-repeat;
  vertical-align: middle;
  opacity: 0.7;
}

.tag-method::before {
  background-image: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="%232196F3"><path d="M12 3L1 9l11 6l11-6z"/></svg>');
}

.tag-domain::before {
  background-image: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="%239C27B0"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10s10-4.48 10-10S17.52 2 12 2z"/></svg>');
}

.tag-application::before {
  background-image: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="%234CAF50"><path d="M3 13h8V3H3v10zm0 8h8v-6H3v6zm10 0h8V11h-8v10zm0-18v6h8V3h-8z"/></svg>');
}

/* 研究方向专用标签样式 */
.research-tag {
  display: inline-flex;
  align-items: center;
  padding: 8px 16px;
  margin: 5px;
  font-size: 0.9em;
  font-weight: 500;
  border-radius: 25px;
  transition: all 0.4s ease;
  position: relative;
  overflow: hidden;
}

/* 核心领域标签 */
.tag-core {
  background: linear-gradient(135deg, #1a237e10, #1a237e20);
  color: #1a237e;
  border: 1.5px solid #1a237e40;
}

/* 技术方法标签 */
.tag-tech {
  background: linear-gradient(135deg, #00695c10, #00695c20);
  color: #00695c;
  border: 1.5px solid #00695c40;
}

/* 应用领域标签 */
.tag-focus {
  background: linear-gradient(135deg, #bf360c10, #bf360c20);
  color: #bf360c;
  border: 1.5px solid #bf360c40;
}

/* 发光效果 */
.research-tag::before {
  content: '';
  position: absolute;
  top: -2px;
  left: -2px;
  right: -2px;
  bottom: -2px;
  background: inherit;
  filter: blur(10px);
  opacity: 0;
  transition: opacity 0.3s ease;
  z-index: -1;
}

.research-tag:hover {
  transform: translateY(-2px);
}

.research-tag:hover::before {
  opacity: 0.7;
}

/* 标签组容器 */
.research-tags-container {
  margin: 25px 0;
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  justify-content: flex-start;
}
</style>

<!-- 添加摘要部分 -->
<div class="summary-section">
  <h1>Publications</h1>
  <p>My research focuses on computer vision and deep learning, with particular emphasis on image restoration and enhancement under real-world conditions. I am also actively exploring AIGC technology and efficient neural architectures like ViTs and Diffusion Models for low-level vision tasks.</p>
  
  <div class="research-tags-container">
    <!-- <span class="research-tag tag-core">Computer Vision</span>
    <span class="research-tag tag-core">Deep Learning</span> -->
    <span class="research-tag tag-tech">Diffusion Models</span>
    <span class="research-tag tag-tech">Vision Transformer</span>
    <span class="research-tag tag-tech">AIGC</span>
    <span class="research-tag tag-focus">Image Restoration</span>
    <span class="research-tag tag-focus">Image Enhancement</span>
    <span class="research-tag tag-focus">Low-level Vision</span>
  </div>

  
<div class="summary-stats">
    <div class="stat-item">
      <div class="stat-number">7</div>
      <div class="stat-label">CVPR/ICCV/ECCV/NeurIPS</div>
      <div class="stat-tooltip">
        <strong>Main list:</strong><br>
        • CVPR'24 (Highlight)<br>
        • ECCV'24 (2 papers)<br>
        • NeurIPS'24<br>
        • ICCV'23 (2 papers)<br>
        • ECCV'22 (Oral)
      </div>
    </div>
    <div class="stat-item">
      <div class="stat-number">5</div>
      <div class="stat-label">AAAI/IJCAI/ACM MM</div>
      <div class="stat-tooltip">
        <strong>Main list:</strong><br>
        • ACM MM'23 (4 papers)<br>
        • MICCAI'24
      </div>
    </div>
     <div class="stat-item">
      <div class="stat-number">4</div>
      <div class="stat-label">Other Conferences</div>
      <div class="stat-tooltip">
        <strong>Main list:</strong><br>
        • BMVC'23<br>
        • ACCV'22<br>
        • ICASSP'23 (2 papers)
      </div>
    </div>
  </div>
</div>

<!-- 2024年论文 -->
<div class="year-section">
  <div class="year-divider">
    <h2 class="year-2024">2024</h2>
  </div>
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
          <span class="paper-tag tag-method">MLLM for Image Restoration</span>
          <span class="paper-tag tag-application">Intelligent Agent</span>
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
    </tbody>
  </table>
<!-- </div> -->

<!-- 2023年论文 -->
<div class="year-section">
  <div class="year-divider">
    <h2 class="year-2023">2023</h2>
  </div>
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


  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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

      
  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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


  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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


  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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


  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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


  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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


  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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


  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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
    </tbody>
  </table>
<!-- </div> -->

<!-- 2022年论文 -->
<div class="year-section">
  <div class="year-divider">
    <h2 class="year-2022">2022</h2>
  </div>
    <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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


  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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


  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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


  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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

  <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
  <tbody>
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
<!-- </div> -->

<!-- <div class="content-wrapper"> -->
  

<!-- # Publications -->

<!-- 7&nbsp; ***CVPR*** / ***ICCV*** / ***ECCV*** /  ***NeurIPS*** &nbsp;&nbsp;&nbsp;5&nbsp; ***AAAI*** / ***IJCAI*** / ***ACM MM*** &nbsp;&nbsp;&nbsp; 1&nbsp; ***MICCAI*** &nbsp;&nbsp;&nbsp; 1&nbsp; ***CVPRW*** / ***ICCVW*** / ***ECCVW*** &nbsp;&nbsp;&nbsp;2&nbsp; ***ACCV*** / ***BMVC*** &nbsp;&nbsp;&nbsp;2&nbsp; ***ICME*** / ***ICASSP*** &nbsp;&nbsp;&nbsp; -->

<!-- =================================================================================== -->







<!-- =================================================================================== -->



<!-- --- -->


