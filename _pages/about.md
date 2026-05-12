{---
permalink: /
title: "Homepage"
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---}


<style>
.home-section {
  margin: 34px 0 44px 0;
}
.pub-figure {
  margin: 16px 0 14px;
  text-align: center;
}

.pub-figure img {
  width: 100%;
  max-width: 850px;
  border-radius: 12px;
  border: 1px solid #e5e7eb;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
}
.home-title {
  display: flex;
  align-items: center;
  gap: 12px;
  font-size: 1.55rem;
  font-weight: 850;
  margin-bottom: 20px;
  color: #111827;
  letter-spacing: -0.02em;
}

.home-title::before {
  content: attr(data-icon);
  width: 36px;
  height: 36px;
  border-radius: 12px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg, #eef2ff 0%, #e0f2fe 100%);
  border: 1px solid #dbeafe;
  box-shadow: 0 4px 12px rgba(15, 23, 42, 0.06);
  font-size: 1.05rem;
  flex: 0 0 auto;
}

.home-title::after {
  content: "";
  height: 1px;
  flex: 1;
  background: linear-gradient(90deg, #e5e7eb 0%, rgba(229, 231, 235, 0) 100%);
  margin-left: 4px;
}

.bio-card {
  border: 1px solid #e5e7eb;
  border-radius: 18px;
  padding: 26px 30px;
  background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
  box-shadow: 0 8px 22px rgba(15, 23, 42, 0.05);
  margin-bottom: 30px;
}

.bio-main {
  font-size: 1.08rem;
  line-height: 1.9;
  color: #374151;
}

.tag-row {
  margin-top: 18px;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.tag {
  display: inline-block;
  padding: 7px 13px;
  border-radius: 999px;
  background: #eef2ff;
  color: #3730a3;
  font-size: 0.88rem;
  font-weight: 650;
  border: 1px solid #e0e7ff;
}

.action-row {
  margin-top: 22px;
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}

.action-btn {
  display: inline-block;
  padding: 9px 15px;
  border-radius: 10px;
  text-decoration: none !important;
  font-weight: 700;
  font-size: 0.92rem;
  border: 1px solid #d1d5db;
  background: #ffffff;
  color: #374151 !important;
  box-shadow: 0 2px 6px rgba(15, 23, 42, 0.04);
}

.info-card {
  border: 1px solid #e5e7eb;
  border-radius: 16px;
  padding: 22px 26px;
  background: #ffffff;
  box-shadow: 0 6px 18px rgba(15, 23, 42, 0.04);
}

.info-card.soft {
  background: #fafafa;
}

.edu-head {
  display: flex;
  align-items: center;
  gap: 18px;
  flex-wrap: wrap;
}

.edu-logo {
  width: 76px;
  height: 76px;
  object-fit: contain;
  border-radius: 14px;
  background: #ffffff;
  padding: 8px;
  border: 1px solid #e5e7eb;
  box-shadow: 0 3px 10px rgba(15, 23, 42, 0.06);
}

.edu-name {
  font-size: 1.18rem;
  font-weight: 800;
  color: #111827;
  margin-bottom: 6px;
}

.edu-meta {
  color: #4b5563;
  margin-bottom: 14px;
  font-size: 0.98rem;
}

.edu-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
  gap: 12px;
  margin-top: 18px;
}

.edu-item {
  padding: 12px 14px;
  border-radius: 12px;
  background: #f8fafc;
  border: 1px solid #eef2f7;
}

.pub-card {
  border-radius: 18px;
  padding: 24px 28px;
  margin: 22px 0;
  background: #f8fafc;
  box-shadow: 0 8px 24px rgba(15, 23, 42, 0.055);
  border: 1px solid #e5e7eb;
  position: relative;
  overflow: hidden;
}

.pub-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 6px;
  height: 100%;
}

.pub-card.seg::before {
  background: #4f46e5;
}

.pub-card.rs::before {
  background: #0ea5e9;
}

.pub-card.med::before {
  background: #10b981;
}

.pub-label {
  display: inline-block;
  padding: 5px 10px;
  border-radius: 999px;
  font-size: 0.78rem;
  font-weight: 800;
  margin-bottom: 12px;
}

.pub-label.seg {
  background: #eef2ff;
  color: #3730a3;
}

.pub-label.rs {
  background: #e0f2fe;
  color: #0369a1;
}

.pub-label.med {
  background: #dcfce7;
  color: #047857;
}

.pub-title {
  font-size: 1.18rem;
  font-weight: 850;
  color: #111827;
  line-height: 1.45;
  margin-bottom: 10px;
}

.pub-authors {
  line-height: 1.75;
  color: #374151;
  margin-bottom: 6px;
}

.pub-venue {
  font-style: italic;
  color: #4b5563;
  margin-bottom: 14px;
}

.pub-short {
  line-height: 1.85;
  color: #374151;
}

.metric-row {
  margin-top: 14px;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.metric {
  display: inline-block;
  padding: 6px 11px;
  border-radius: 10px;
  font-size: 0.86rem;
  font-weight: 800;
  background: #ffffff;
  border: 1px solid #e5e7eb;
  color: #374151;
}

details {
  margin-top: 14px;
}

summary {
  cursor: pointer;
  font-weight: 800;
  color: #2563eb;
  margin-top: 10px;
}

.detail-box {
  margin-top: 12px;
  padding: 15px 18px;
  border-radius: 12px;
  background: #ffffff;
  border: 1px solid #e5e7eb;
  line-height: 1.85;
  color: #374151;
}

.project-card {
  border: 1px solid #e5e7eb;
  border-radius: 18px;
  padding: 24px 28px;
  background: #ffffff;
  box-shadow: 0 8px 24px rgba(15, 23, 42, 0.045);
}

.project-title {
  font-size: 1.16rem;
  font-weight: 850;
  margin-bottom: 8px;
  color: #111827;
}

.project-meta {
  color: #4b5563;
  font-style: italic;
  margin-bottom: 14px;
}

.award-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(285px, 1fr));
  gap: 14px;
  margin-top: 18px;
}

.award-card {
  border: 1px solid #e5e7eb;
  border-radius: 16px;
  padding: 17px 18px;
  background: #fafafa;
  box-shadow: 0 5px 14px rgba(15, 23, 42, 0.035);
}

.award-name {
  font-weight: 850;
  color: #111827;
  margin-bottom: 6px;
}

.award-meta {
  color: #4b5563;
  line-height: 1.7;
}

@media (max-width: 768px) {
  .bio-card,
  .info-card,
  .pub-card,
  .project-card {
    padding: 20px 18px;
  }
}
</style>
  <div>
    <div class="edu-name">Anhui University of Science and Technology</div>
    <div class="edu-meta">B.Eng. in Computer Science and Technology &nbsp; | &nbsp; Sep. 2023 - Present</div>
  </div>
</div>

<div class="edu-grid">
  <div class="edu-item">
    <strong>GPA</strong><br>
    4.20 / 5.00
  </div>

  <div class="edu-item">
    <strong>Ranking</strong><br>
    12/ 402, top 3%
  </div>

  <div class="edu-item">
    <strong>English</strong><br>
    CET-4, CET-6
  </div>
</div>



<div class="pub-title">
  StructMamba-Seg: Boundary-Context Guided Deformable Scan for Semantic Segmentation
</div>

<div class="pub-authors">
 Longfei Xiao, Linlin Zhang,  <strong>Kang Yang</strong>, Changqiu Xu, Shuyu Liu, Jianfang Wang
</div>

<div class="pub-venue">
  Submitted to International Conference on Neural Information Processing (ICONIP), 2026
</div>

<div class="pub-short">
  A structure-sensitive Mamba-based semantic segmentation framework that introduces <strong>Boundary-Context Guided Deformable Scan</strong> to adapt scan control to boundaries, small objects, thin structures, and ambiguous regions.
</div>

<div class="metric-row">
  <span class="metric">Cityscapes: 82.12% mIoU</span>
  <span class="metric">ADE20K: 50.20% mIoU</span>
  <span class="metric">Boundary-aware Optimization</span>
</div>

<details>
  <summary>Show details</summary>
  <div class="detail-box">
    StructMamba-Seg bridges the gap between generic scan decisions and segmentation-specific structural requirements. Its BCG-DefScan module incorporates local geometry, boundary prompts, and multi-scale context to jointly predict spatial offsets, local ordering offsets, and gating signals. The framework also introduces an IoU-boundary joint optimization objective to improve regional consistency and boundary details during training.
  </div>
</details>



<div class="pub-title">
  PDAO-Net: A Physics-Constrained Dual-Domain Alternating Optimization Network for Sparse-View 3D-DSA Reconstruction
</div>

<div class="pub-authors">
  Changqiu Xu, Xi Wang, Yujia Li, Tong Liang, <strong>Kang Yang</strong>, Longfei Xiao, Yikun Zhang, Yang Chen
</div>

<div class="pub-venue">
  Submitted to International Conference on Neural Information Processing (ICONIP), 2026
</div>

<div class="pub-short">
  A physics-constrained reconstruction framework for sparse-view 3D-DSA that alternates between <strong>projection-domain correction</strong> and <strong>image-domain refinement</strong>.
</div>

<div class="metric-row">
  <span class="metric">Dual-domain Optimization</span>
  <span class="metric">Measured-view Consistency</span>
  <span class="metric">Vascular Recovery</span>
</div>

<details>
  <summary>Show details</summary>
  <div class="detail-box">
    PDAO-Net initializes reconstruction in both the image and projection domains using a pre-trained restoration network and forward projection. It unfolds the reconstruction process into an N-stage alternating optimization framework, where corrected projections and refined volumes mutually constrain each other. A measured-view replacement mechanism preserves acquired sparse-view measurements during missing-view projection estimation.
  </div>
</details>

<div class="project-meta">
  Project Leader &nbsp; | &nbsp; Oct. 2025 - Dec. 2025
</div>

<div style="line-height: 1.9; color: #374151;">
  This project investigates the robustness degradation and high-confidence misclassification of ConvNeXt under real-world corrupted inputs. Based on <strong>ConvNeXt</strong> and <strong>Tiny-ImageNet-200</strong>, I built a hierarchical evaluation protocol covering clean validation, fixed-degradation validation, and degradation-grid testing. The project further introduced degradation augmentation, consistency regularization, sample mixing, and exponential moving average to improve robustness under noise, blur, and JPEG compression.
</div>

<div class="award-card">
  <div class="award-name">National Second Prize</div>
  <div class="award-meta">
    AICOMP Object Detection 2025<br>
    2025 | Team Leader
  </div>
</div>

<div class="award-card">
  <div class="award-name">National Second Prize</div>
  <div class="award-meta">
    AICOMP Image Classification 2025<br>
    2025 | Team Leader
  </div>
</div>

<div class="award-card">
  <div class="award-name">Provincial First Prize</div>
  <div class="award-meta">
    AICOMP Object Detection 2025<br>
    2025 | Team Leader
  </div>
</div>

<div class="award-card">
  <div class="award-name">Provincial First Prize</div>
  <div class="award-meta">
    AICOMP Image Classification 2025<br>
    2025 | Team Leader
  </div>
</div>

