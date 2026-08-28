---
permalink: "/"
title: "Homepage"
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---


<style>
/* 👇 加上这一段开启平滑滚动 👇 */
html {
  scroll-behavior: smooth;
  scroll-padding-top: 80px; 
}
/* 👆 ======================= 👆 */

.home-section {
  margin: 34px 0 44px 0;
}
.pub-figure {
  margin: 16px 0 14px;
  text-align: center;
}


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
.award-cert {
  margin-top: 12px;
}

.award-cert img {
  width: 100%;
  max-height: 220px;
  object-fit: cover;
  border-radius: 12px;
  border: 1px solid #e5e7eb;
  box-shadow: 0 4px 12px rgba(15, 23, 42, 0.06);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.award-cert img:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 18px rgba(15, 23, 42, 0.10);
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
  font-size: 1.58rem;
  font-weight: 850;
  color: #111827;
  line-height: 2;
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

<!-- About Me Section -->
<div class="bio-card" id="about">
  <div class="bio-main">
    I am <strong>Zesheng Zhang</strong>, an undergraduate student majoring in <strong>Artificial Intelligence</strong> at <strong>Anhui University of Science and Technology</strong>. My research interests lie in <strong>Evolutionary Computation</strong>, <strong>Intelligent Optimization</strong>, <strong>Data Mining</strong>, <strong>Machine Learning</strong>, <strong>Reinforcement Learning</strong> and <strong>Pattern Recognition</strong>. I aim to refine the mathematical theory of evolutionary computation using fundamental mathematical principles and to use this framework to explain the field, thereby thoroughly breaking open the "black box" of artificial intelligence and achieving explainable AI.
  </div>

  <div class="tag-row">
    <span class="tag">Evolutionary Computation</span>
    <span class="tag">Data Mining</span>
    <span class="tag">Pattern Recognition</span>
    <span class="tag">Artificial Intelligence</span>
    <span class="tag">Machine Learning</span>
    <span class="tag">Reinforcement Learning</span>
  </div>
</div>

<!-- Education Section -->
<div class="home-section" id="education">
  <div class="home-title" data-icon="🎓">Education</div>

  <div class="info-card soft">
    <div class="edu-head">
      <img class="edu-logo" src="{{ '/images/aust-logo.png' | relative_url }}" alt="Anhui University of Science and Technology">

      <div>
        <div class="edu-name">Anhui University of Science and Technology</div>
        <div class="edu-meta">B.Eng. in Artificial Intelligence &nbsp; | &nbsp; Sep. 2023 - Present</div>
      </div>
    </div>

    <div class="edu-grid">
      <div class="edu-item">
        <strong>GPA</strong><br>
        4.36 / 5.00
      </div>

      <div class="edu-item">
        <strong>Ranking</strong><br>
        1/ 157, top 1%
      </div>

      <div class="edu-item">
        <strong>English</strong><br>
        CET-4
      </div>
    </div>
  </div>
</div>

<!-- Publications Section -->
<div class="home-section" id="publications">
  <div class="home-title" data-icon="📚">Publications</div>

  <div class="pub-card rs">
    <div class="pub-label rs">Evolutionary Computation · Feature Selection</div>

    <div class="pub-title">
      Learning-Assisted Evolutionary Feature Selection via Age-Reinforced Reduction and Expansion for High-Dimensional Classification
    </div>

    <div class="pub-authors">
      <strong>Zesheng Zhang</strong>, Shoufei Han*, Xiaojing Liu, Changhe Li, Kaixiang Yang and Qianlong Dang
    </div>

    <div class="pub-venue">
      <em>IEEE Transactions on Evolutionary Computation</em><br>
      <span style="font-size: 0.9em; font-weight: 600; color: #c0392b;">🏆 CAS Q1 Top | CCF-B | IF: 15.9</span>
    </div>

    <div class="pub-short">
      A learning-assisted feature selection framework (EFSARE) that combines a <strong>novel feature-level encoding strategy</strong>, reinforcement learning, and an age-driven reduction-and-expansion mechanism for high-dimensional data classification.
    </div>

    <div class="pub-figure">
      <img src="{{ '/images/framer.png' | relative_url }}" alt="Overall framework of the EFSARE">
    </div>

    <div class="metric-row">
      <span class="metric">Feature-level Encoding</span>
      <span class="metric">RL-driven Adjustment</span>
      <span class="metric">Age-guided Strategy</span>
    </div>

    <details>
      <summary>Show details</summary>
      <div class="detail-box">
        EFSARE addresses the challenges of high-dimensional individual representation and slow search efficiency in evolutionary computation. It introduces a novel encoding scheme where each individual corresponds to a single feature and the population collectively represents the entire feature space. Guided by reinforcement learning (Q-learning) and historical age information, it adaptively switches between feature reduction and expansion. Comprehensive experiments on 22 high-dimensional public datasets and 2 gene engineering datasets demonstrate that it achieves state-of-the-art performance in terms of average classification accuracy, number of selected features, and computational time.
        <div class="pub-figure">
          <img src="{{ '/images/EFSARE_Encode.png' | relative_url }}" alt="Experiments on 22 High-dimensional Datasets">
        </div>
      </div>
    </details>
  </div>

  <div class="pub-card rs">
    <div class="pub-label rs">Evolutionary Computation · Feature Selection · IIoT</div>

    <div class="pub-title">
      Evolutionary Feature Selection via Cosine Similarity Initialization and Manifold Contracting for Sparse IIoT Data
    </div>

    <div class="pub-authors">
      <strong>Zesheng Zhang</strong>, Shoufei Han*, Xiaojing Liu, Yongbiao Gao*, Kun Zhu, Zhi Liu, and Liang Zhao
    </div>

    <div class="pub-venue">
      <em>IEEE Internet of Things Journal</em><br>
      <span style="font-size: 0.9em; font-weight: 600; color: #c0392b;">🏆 CAS Q1 Top | CCF-C | IF: 8.9</span>
    </div>

    <div class="pub-short">
      An innovative framework termed Adaptive Decision Space Contraction (ADSC) that combines a <strong>Cosine Similarity Initialization Method (CSIM)</strong> and a dynamically contracting manifold system to address high-dimensional sparse IIoT data.
    </div>

    <div class="pub-figure">
      <img src="{{ '/images/ADSC_frame.png' | relative_url }}" alt="Overall framework of the ADSC">
    </div>

    <div class="metric-row">
      <span class="metric">Cosine Similarity Initialization</span>
      <span class="metric">Adaptive Space Contraction</span>
      <span class="metric">Sparse IIoT Data</span>
    </div>

    <details>
      <summary>Show details</summary>
      <div class="detail-box">
        ADSC addresses the challenges of uneven initial population distribution and redundant features in high-dimensional industrial data. It introduces a Cosine Similarity Initialization Method (CSIM) to ensure a highly diverse initial population by measuring the angles between solution vectors. Furthermore, it employs a greedy strategy to transform the static feature search space into a dynamically contracting manifold system, achieving an exponential reduction in the decision space. Comprehensive experiments on representative real-world industrial datasets (SECOM and TEP) and 12 high-dimensional benchmark datasets demonstrate that ADSC achieves top-tier performance across classification accuracy, feature subset size, and computational efficiency.
        <div class="pub-figure">
          <img src="{{ '/images/ADSC_times.png' | relative_url }}" alt="Experiments on Industrial and Benchmark Datasets">
        </div>
      </div>
    </details>
  </div>

  <div class="pub-card rs">
    <div class="pub-label rs">Evolutionary Computation · Multi-UAV Trajectory Planning · LAE</div>

    <div class="pub-title">
      WQAD-RIME: A Convergence-Enhanced Metaheuristic Framework for Multi-UAV Trajectory Planning in Low-Altitude Mobile Environments
    </div>

    <div class="pub-authors">
      Kaiyuan Zheng, Xiangyu Li, Yiming Huang, Liu Zhang, Wei Deng, <strong>Zesheng Zhang</strong>, and Xiong Wang*
    </div>

    <div class="pub-venue">
      <em>IEEE Transactions on Mobile Computing</em> (Under review)<br>
      <span style="font-size: 0.9em; font-weight: 600; color: #c0392b;">🏆 CAS Q1 Top | CCF-A | IF: 8.8 </span>
    </div>

    <div class="pub-short">
      A convergence-enhanced evolutionary framework (WQAD-RIME) that incorporates <strong>four complementary mechanisms (WHI, QDE, ABRD, DCRL)</strong> to address high-dimensional, nonconvex multi-UAV trajectory planning in low-altitude environments.
    </div>

    <div class="pub-figure">
      <img src="{{ '/images/WQAD_framework.png' | relative_url }}" alt="Overall framework of WQAD">
    </div>

    <div class="metric-row">
      <span class="metric">Weierstrass-Harmonic Initialization</span>
      <span class="metric">Adaptive Bidirectional Drift</span>
      <span class="metric">Dynamic Centroid Learning</span>
    </div>

    <details>
      <summary>Show details</summary>
      <div class="detail-box">
        WQAD-RIME addresses the limitations of existing metaheuristic trajectory planners, such as poor population initialization and premature convergence, in high-dimensional nonconvex spaces. It utilizes a Weierstrass-harmonic initialization module for diverse dispersion, a quotient-based dynamic equilibrium for exploration-exploitation balance, an adaptive bidirectional rime-drift strategy to accelerate local refinement, and a dynamic centroid-based reverse-learning mechanism to improve search diversity. Extensive experiments on 42 high-dimensional benchmark functions and real-world multi-UAV scenarios demonstrate that it effectively shortens total flight trajectories and reduces associated operational costs.
        <div class="pub-figure">
          <img src="{{ '/images/WQAD_Experiment.png' | relative_url }}" alt="Experiments on Multi-UAV Trajectory Planning">
        </div>
      </div>
    </details>
  </div>

  <div class="pub-card rs">
    <div class="pub-label rs">Remote Sensing · Low-light Enhancement</div>

    <div class="pub-title">
      Towards High-quality Low-Light Remote Sensing Image Enhancement via Geometric and Semantic Prior Guidance
    </div>

    <div class="pub-authors">
      Kang Yang, Jiaqi Zhang, Changqiu Xu, Longfei Xiao, Tong Liang and <strong>Zesheng Zhang*</strong>
    </div>

    <div class="pub-venue">
      <em>International Conference on Neural Information Processing (ICONIP), Melbourne, Australia, 2026</em><br>
      <span style="font-size: 0.9em; font-weight: 600; color: #c0392b;">🏆 CCF-C </span>
    </div>

    <div class="pub-short">
      A low-light remote sensing image enhancement framework that combines an <strong>HVI-based dual-branch design</strong>, geometric-semantic prior guidance, and adaptive sparse refinement.
    </div>

    <div class="pub-figure">
      <img src="{{ '/images/Pipline.jpg' | relative_url }}" alt="Pipeline of GSPNet">
    </div>

    <div class="metric-row">
      <span class="metric">HVI Dual-branch</span>
      <span class="metric">DINOv2 + Depth Priors</span>
      <span class="metric">Adaptive Sparse Refinement</span>
    </div>

    <details>
      <summary>Show details</summary>
      <div class="detail-box">
        GSPNet addresses illumination degradation, chromatic distortion, and dark-region noise in remote sensing images. It decouples brightness restoration from color recovery in the HVI space, injects semantic and geometric priors from frozen vision foundation models, and uses adaptive sparse refinement to suppress unreliable feature interactions while preserving land-cover structures.
        <div class="pub-figure">
          <img src="{{ '/images/Figure1.jpg' | relative_url }}" alt="Experiment On iSAID-darks">
        </div>
      </div>
    </details>
  </div>
</div>

<!-- Awards Section -->
<div class="home-section" id="awards">
  <div class="home-title" data-icon="🏆">Awards</div>

  <div class="award-grid">
    <div class="award-card">
      <div class="award-name">National Scholarship</div>
      <div class="award-meta">
        Ministry of Education of the People's Republic of China<br>
        2023-2024 school year
      </div>

      <div class="award-cert">
        <a href="{{ '/images/2023-2024.jpg' | relative_url }}" target="_blank">
          <img src="{{ '/images/2023-2024.jpg' | relative_url }}" alt="Certificate of National Scholarship">
        </a>
      </div>
    </div>

    <div class="award-card">
      <div class="award-name">National Scholarship</div>
      <div class="award-meta">
        Ministry of Education of the People's Republic of China<br>
        2024-2025 school year
      </div>

      <div class="award-cert">
        <a href="{{ '/images/2024-2025.jpg' | relative_url }}" target="_blank">
          <img src="{{ '/images/2024-2025.jpg' | relative_url }}" alt="Certificate of National Scholarship">
        </a>
      </div>
    </div>

    <div class="award-card">
      <div class="award-name">Honorable Mention</div>
      <div class="award-meta">
        Mathematical Contest in Modeling (MCM/ICM)<br>
        2026 | Team Leader
      </div>

      <div class="award-cert">
        <a href="{{ '/images/MCM_Honorable_Mention.png' | relative_url }}" target="_blank">
          <img src="{{ '/images/MCM_Honorable_Mention.png' | relative_url }}" alt="Certificate of MCM/ICM Honorable Mention">
        </a>
      </div>
    </div>

    <div class="award-card">
      <div class="award-name">National Second Prize</div>
      <div class="award-meta">
        RoboCom Robot Developer Competition<br>
        2026 | Team Leader
      </div>

      <div class="award-cert">
        <a href="{{ '/images/RoboCom_National_Second.jpg' | relative_url }}" target="_blank">
          <img src="{{ '/images/RoboCom_National_Second.jpg' | relative_url }}" alt="Certificate of RoboCom National Second Prize">
        </a>
      </div>
    </div>
  </div>
</div>