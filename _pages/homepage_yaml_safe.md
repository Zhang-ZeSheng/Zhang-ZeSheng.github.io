---
permalink: "/"
title: "Homepage"
excerpt: "Zesheng Zhang is an undergraduate AI researcher at Anhui University of Science and Technology working on evolutionary computation, intelligent optimization, and feature selection."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
/* 👇 全局平滑滚动 👇 */
html {
  scroll-behavior: smooth;
  scroll-padding-top: 80px;
}

#about,
#education,
#publications,
#awards,
#contact {
  scroll-margin-top: 80px;
}

/* 👇 导航栏高亮联动样式 👇 */
a[href^="#"] {
  transition: all 0.3s ease;
}
a[href^="#"].active {
  color: #2563eb !important;
  font-weight: 800 !important;
  border-bottom: 2px solid #2563eb; 
  padding-bottom: 2px;
}

/* 👇 页面元素样式 👇 */
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
  font-size: 1.45rem;
  font-weight: 850;
  margin-bottom: 20px;
  color: #111827;
  letter-spacing: -0.02em;
}

h2.home-title,
h3.pub-title,
h3.award-name,
h3.project-title {
  margin: 0;
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

.highlight-row {
  margin-top: 16px;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.highlight {
  display: inline-block;
  padding: 7px 13px;
  border-radius: 999px;
  background: #f0fdf4;
  color: #047857;
  font-size: 0.88rem;
  font-weight: 700;
  border: 1px solid #bbf7d0;
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

.action-btn:hover {
  border-color: #2563eb;
  color: #2563eb !important;
  box-shadow: 0 4px 12px rgba(37, 99, 235, 0.14);
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
  font-size: 1.38rem;
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

.pub-status {
  display: inline-block;
  margin-top: 4px;
  padding: 4px 9px;
  border-radius: 999px;
  background: #fee2e2;
  color: #b91c1c;
  font-size: 0.84rem;
  font-weight: 750;
  font-style: normal;
}

.pub-status.muted {
  background: #f1f5f9;
  color: #475569;
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

.view-hint {
  display: block;
  margin-top: 9px;
  color: #2563eb;
  font-size: 0.88rem;
  font-weight: 700;
}

.contact-card {
  border: 1px solid #e5e7eb;
  border-radius: 18px;
  padding: 26px 30px;
  background: linear-gradient(135deg, #ffffff 0%, #eff6ff 100%);
  box-shadow: 0 8px 24px rgba(15, 23, 42, 0.045);
}

.contact-lead {
  margin: 0 0 18px;
  color: #374151;
  line-height: 1.85;
}

@media (max-width: 768px) {
  .bio-card,
  .info-card,
  .pub-card,
  .project-card {
    padding: 20px 18px;
  }
}

@media (prefers-reduced-motion: reduce) {
  html {
    scroll-behavior: auto;
  }
  .award-cert img {
    transition: none;
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
  <h2 class="home-title" data-icon="🎓">Education</h2>

  <div class="info-card soft">
    <div class="edu-head">
      <img class="edu-logo" src="{{ '/images/aust-logo.png' | relative_url }}" alt="Anhui University of Science and Technology" width="76" height="76" loading="lazy" decoding="async">

      <div>
        <div class="edu-name">Anhui University of Science and Technology</div>
        <div class="edu-meta">B.Eng. in Artificial Intelligence &nbsp; | &nbsp; Sep. 2023 – 2027</div>
      </div>
    </div>

    <div class="edu-grid">
      <div class="edu-item">
        <strong>GPA</strong><br>
        4.36 / 5.00
      </div>

      <div class="edu-item">
        <strong>Ranking</strong><br>
        1 / 157, top 1%
      </div>

      <div class="edu-item">
        <strong>English</strong><br>
        CET-4
      </div>
    </div>
  </div>

  <div class="info-card soft">
    <div class="edu-head">
      <img class="edu-logo" src="{{ '/images/SE.png' | relative_url }}" alt="Southeast University" width="76" height="76" loading="lazy" decoding="async">

      <div>
        <div class="edu-name">Southeast University</div>
        <div class="edu-meta">M.Eng. in Artificial Intelligence &nbsp; | &nbsp; Sep. 2027 – 2030</div>
      </div>
    </div>

    <div class="edu-grid">
      <div class="edu-item">
        <strong>GPA</strong><br>
        4.36 / 5.00
      </div>

      <div class="edu-item">
        <strong>Ranking</strong><br>
        1 / 157, top 1%
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
  <h2 class="home-title" data-icon="📚">Publications</h2>

  <div class="pub-card rs">
    <div class="pub-label rs">Evolutionary Computation · Feature Selection</div>

    <h3 class="pub-title">
      Learning-Assisted Evolutionary Feature Selection via Age-Reinforced Reduction and Expansion for High-Dimensional Classification
    </h3>

    <div class="pub-authors">
      <strong>Zesheng Zhang</strong>, Shoufei Han*, Xiaojing Liu, Changhe Li, Kaixiang Yang and Qianlong Dang
    </div>

    <div class="pub-venue">
      <em>IEEE Transactions on Evolutionary Computation</em><br>
      <span class="pub-status">CAS Q1 Top · CCF-B · IF: 15.9</span>
    </div>

    <div class="pub-short">
      An RL-assisted evolutionary feature selection framework (EFSARE) that combines a <strong>feature-level encoding strategy</strong>, reinforcement learning, and age-guided reduction and expansion for high-dimensional classification.
    </div>

    <div class="pub-figure">
      <img src="{{ '/images/framer.png' | relative_url }}" alt="Overall framework of the EFSARE" width="1800" height="773" loading="lazy" decoding="async">
    </div>

    <div class="metric-row">
      <span class="metric">Feature-level Encoding</span>
      <span class="metric">RL-driven Adjustment</span>
      <span class="metric">Age-guided Strategy</span>
    </div>

    <details>
      <summary>Read more</summary>
      <div class="detail-box">
        EFSARE addresses the challenges of high-dimensional individual representation and slow search efficiency in evolutionary computation. It introduces a novel encoding scheme where each individual corresponds to a single feature and the population collectively represents the entire feature space. Guided by reinforcement learning (Q-learning) and historical age information, it adaptively switches between feature reduction and expansion. Comprehensive experiments on 22 high-dimensional public datasets and 2 gene engineering datasets demonstrate that it achieves state-of-the-art performance in terms of average classification accuracy, number of selected features, and computational time.
        <div class="pub-figure">
          <img src="{{ '/images/EFSARE_Encode.png' | relative_url }}" alt="Experiments on 22 high-dimensional datasets" width="1200" height="593" loading="lazy" decoding="async">
        </div>
      </div>
    </details>
  </div>

  <div class="pub-card rs">
    <div class="pub-label rs">Evolutionary Computation · Feature Selection · IIoT</div>

    <h3 class="pub-title">
      Evolutionary Feature Selection via Cosine Similarity Initialization and Manifold Contracting for Sparse IIoT Data
    </h3>

    <div class="pub-authors">
      <strong>Zesheng Zhang</strong>, Shoufei Han*, Xiaojing Liu, Yongbiao Gao*, Kun Zhu, Zhi Liu, and Liang Zhao
    </div>

    <div class="pub-venue">
      <em>IEEE Internet of Things Journal</em><br>
      <span class="pub-status">CAS Q1 Top · CCF-C · IF: 8.9</span>
    </div>

    <div class="pub-short">
      An adaptive decision-space contraction framework (ADSC) that initializes diverse solutions with <strong>cosine similarity</strong> and greedily contracts the feature space for sparse IIoT data.
    </div>

    <div class="pub-figure">
      <img src="{{ '/images/ADSC_frame.png' | relative_url }}" alt="Overall framework of the ADSC" width="1800" height="876" loading="lazy" decoding="async">
    </div>

    <div class="metric-row">
      <span class="metric">Cosine Similarity Initialization</span>
      <span class="metric">Adaptive Space Contraction</span>
      <span class="metric">Sparse IIoT Data</span>
    </div>

    <details>
      <summary>Read more</summary>
      <div class="detail-box">
        ADSC addresses the challenges of uneven initial population distribution and redundant features in high-dimensional industrial data. It introduces a Cosine Similarity Initialization Method (CSIM) to ensure a highly diverse initial population by measuring the angles between solution vectors. Furthermore, it employs a greedy strategy to transform the static feature search space into a dynamically contracting manifold system, achieving an exponential reduction in the decision space. Comprehensive experiments on representative real-world industrial datasets (SECOM and TEP) and 12 high-dimensional benchmark datasets demonstrate that ADSC achieves top-tier performance across classification accuracy, feature subset size, and computational efficiency.
        <div class="pub-figure">
          <img src="{{ '/images/ADSC_times.png' | relative_url }}" alt="Experiments on industrial and benchmark datasets" width="2453" height="2118" loading="lazy" decoding="async">
        </div>
      </div>
    </details>
  </div>

  <div class="pub-card rs">
    <div class="pub-label rs">Evolutionary Computation · Multi-UAV Trajectory Planning · LAE</div>

    <h3 class="pub-title">
      WQAD-RIME: A Convergence-Enhanced Metaheuristic Framework for Multi-UAV Trajectory Planning in Low-Altitude Mobile Environments
    </h3>

    <div class="pub-authors">
      Kaiyuan Zheng, Xiangyu Li, Yiming Huang, Liu Zhang, Wei Deng, <strong>Zesheng Zhang</strong>, and Xiong Wang*
    </div>

    <div class="pub-venue">
      <em>IEEE Transactions on Mobile Computing</em> (Under review)<br>
      <span class="pub-status muted">CAS Q1 Top · CCF-A · IF: 8.8</span>
    </div>

    <div class="pub-short">
      A convergence-enhanced metaheuristic framework (WQAD-RIME) that couples <strong>four complementary mechanisms</strong> to improve multi-UAV trajectory planning in low-altitude mobile environments.
    </div>

    <div class="pub-figure">
      <img src="{{ '/images/WQAD_framework.png' | relative_url }}" alt="Overall framework of WQAD-RIME" width="1800" height="1260" loading="lazy" decoding="async">
    </div>

    <div class="metric-row">
      <span class="metric">Weierstrass-Harmonic Initialization</span>
      <span class="metric">Adaptive Bidirectional Drift</span>
      <span class="metric">Dynamic Centroid Learning</span>
    </div>

    <details>
      <summary>Read more</summary>
      <div class="detail-box">
        WQAD-RIME addresses the limitations of existing metaheuristic trajectory planners, such as poor population initialization and premature convergence, in high-dimensional nonconvex spaces. It utilizes a Weierstrass-harmonic initialization module for diverse dispersion, a quotient-based dynamic equilibrium for exploration-exploitation balance, an adaptive bidirectional rime-drift strategy to accelerate local refinement, and a dynamic centroid-based reverse-learning mechanism to improve search diversity. Extensive experiments on 42 high-dimensional benchmark functions and real-world multi-UAV scenarios demonstrate that it effectively shortens total flight trajectories and reduces associated operational costs.
        <div class="pub-figure">
          <img src="{{ '/images/WQAD_Experiment.png' | relative_url }}" alt="Experiments on multi-UAV trajectory planning" width="1800" height="1437" loading="lazy" decoding="async">
        </div>
      </div>
    </details>
  </div>

  <div class="pub-card rs">
    <div class="pub-label rs">Remote Sensing · Low-light Enhancement</div>

    <h3 class="pub-title">
      Towards High-quality Low-Light Remote Sensing Image Enhancement via Geometric and Semantic Prior Guidance
    </h3>

    <div class="pub-authors">
      Kang Yang, Jiaqi Zhang, Changqiu Xu, Longfei Xiao, Tong Liang and <strong>Zesheng Zhang*</strong>
    </div>

    <div class="pub-venue">
      <em>International Conference on Neural Information Processing (ICONIP), Melbourne, Australia, 2026</em><br>
      <span class="pub-status">Conference paper · EI · CCF-C</span>
    </div>

    <div class="pub-short">
      A geometry- and semantics-guided enhancement network (GSPNet) that recovers brightness and color from low-light remote sensing images using <strong>HVI-based dual-branch design</strong> and adaptive sparse refinement.
    </div>

    <div class="pub-figure">
      <img src="{{ '/images/Pipline.jpg' | relative_url }}" alt="Pipeline of GSPNet" width="1800" height="885" loading="lazy" decoding="async">
    </div>

    <div class="metric-row">
      <span class="metric">HVI Dual-branch</span>
      <span class="metric">DINOv2 + Depth Priors</span>
      <span class="metric">Adaptive Sparse Refinement</span>
    </div>

    <details>
      <summary>Read more</summary>
      <div class="detail-box">
        GSPNet addresses illumination degradation, chromatic distortion, and dark-region noise in remote sensing images. It decouples brightness restoration from color recovery in the HVI space, injects semantic and geometric priors from frozen vision foundation models, and uses adaptive sparse refinement to suppress unreliable feature interactions while preserving land-cover structures.
        <div class="pub-figure">
          <img src="{{ '/images/Figure1.jpg' | relative_url }}" alt="Qualitative results on iSAID-darks" width="1200" height="1088" loading="lazy" decoding="async">
        </div>
      </div>
    </details>
  </div>


  <div class="pub-card rs">
  <div class="pub-label rs">Evolutionary Computation · Numerical Optimization</div>

  <h3 class="pub-title">
    High-Precision Numerical Optimization via ISSA: Manifold Weighting and Heavy-tailed Mutation
  </h3>

  <div class="pub-authors">
    <strong>Zesheng Zhang*</strong>, Kaiyuan Zheng, and Kang Yang
  </div>

  <div class="pub-venue">
    <em>2026 9th International Conference on Advanced Algorithms and Control Engineering (ICAACE)</em><br>
    <span class="pub-status">Conference paper · EI</span>
  </div>

  <div class="pub-short">
    An Improved Sparrow Search Algorithm (ISSA) that integrates a <strong>Sigmoid-based manifold weight</strong>, Lévy flight strategy, and Cauchy mutation to overcome premature convergence and achieve extreme optimization precision.
  </div>

  <!-- 👇 修改为直接跳转至 IEEE Xplore 的按钮 👇 -->
  <div class="action-row" style="margin-top: 12px; margin-bottom: 16px;">
    <a href="https://doi.org/10.1109/ICAACE69793.2026.11508895" target="_blank" class="action-btn">
      🔗 IEEE Xplore
    </a>

    <a href="javascript:void(0)" class="action-btn" onclick="navigator.clipboard.writeText(this.dataset.bibtex); const originalText = this.innerText; this.innerText='✅ Copied!'; setTimeout(() => this.innerText=originalText, 2000);" data-bibtex="@INPROCEEDINGS{11508895,
  author={Zhang, Zesheng and Zheng, Kaiyuan and Yang, Kang},
  booktitle={2026 9th International Conference on Advanced Algorithms and Control Engineering (ICAACE)}, 
  title={High-Precision Numerical Optimization via ISSA: Manifold Weighting and Heavy-Tailed Mutation}, 
  year={2026},
  volume={},
  number={},
  pages={1767-1771},
  keywords={Optimization;Algorithms;Equations;Convergence;Modeling;Printing;Tagging;Standards;Tail;Manifolds;Sparrow Search Algorithm (SSA);Sigmoid Weight;Lévy Flight;Cauchy Mutation;Numerical Optimization},
  doi={10.1109/ICAACE69793.2026.11508895}}">
      📝 BibTeX
    </a>

  </div>

  <div class="pub-figure">
    <img src="{{ '/images/ISSA_framework.png' | relative_url }}" alt="Flowchart of the ISSA" width="1800" height="885" loading="lazy" decoding="async">
  </div>

  <div class="metric-row">
    <span class="metric">Sigmoid Manifold Weight</span>
    <span class="metric">Lévy Flight Strategy</span>
    <span class="metric">Cauchy Mutation</span>
  </div>

  <details>
    <summary>Read more</summary>
    <div class="detail-box">
      ISSA mitigates the limitations of standard SSA (premature convergence and loss of population diversity) in high-dimensional optimization tasks. By integrating Ergodic Refractive Mapping (ERM) initialization, Sigmoid-based adaptive manifold weights, Lévy flight, and Cauchy mutation, the algorithm dynamically balances global exploration and local exploitation. Statistical evaluation across 12 benchmark functions demonstrates that ISSA achieves extreme convergence precision up to $10^{-124}$, significantly outperforming standard SSA, PSO, GA, and SA in complex numerical optimization environments.
      <div class="pub-figure">
        <img src="{{ '/images/ISSA_Experiment.png' | relative_url }}" alt="Convergence Analysis on Benchmark Functions" width="1200" height="1088" loading="lazy" decoding="async">
      </div>
    </div>
  </details>
</div>

<div class="pub-card rs">
  <div class="pub-label rs">Particle Swarm Optimization · Multi-objective Optimization<!--[cite: 4] --></div>

  <h3 class="pub-title">
    Research on Relocation Compensation and Whole Hospital Optimization Decision of Old Town Based on Particle Swarm Optimization Algorithm<!--[cite: 4] -->
  </h3>

  <div class="pub-authors">
    <strong>Zesheng Zhang</strong><!--[cite: 4] -->
  </div>

  <div class="pub-venue">
    <em>Mathematical Modeling and Algorithm Application</em><br><!--[cite: 4] -->
    <span class="pub-status">Journal Article</span>
  </div>

  <div class="pub-short">
    A multi-objective optimization framework that utilizes a <strong>Logit model and Particle Swarm Optimization (PSO)</strong> to solve complex relocation compensation and decision-making challenges in old city renewals<!--[cite: 4] -->.
  </div>

  <!-- 👇 直接跳转至官方 DOI 的按钮 👇 -->
  <div class="action-row" style="margin-top: 12px; margin-bottom: 16px;">
    <a href="https://doi.org/10.54097/bvjpmf68" target="_blank" class="action-btn">
      🔗 Publisher
    </a>

    <a href="javascript:void(0)" class="action-btn" onclick="navigator.clipboard.writeText(this.dataset.bibtex); const originalText = this.innerText; this.innerText='✅ Copied!'; setTimeout(() => this.innerText=originalText, 2000);" data-bibtex="@article{Zhang_2025, title={Research on Relocation Compensation and Whole Hospital Optimization Decision of Old Town Based on Particle Swarm Optimization Algorithm}, volume={5}, url={https://drpress.org/ojs/index.php/mmaa/article/view/31393}, DOI={10.54097/bvjpmf68},number={2}, journal={Mathematical Modeling and Algorithm Application}, author={Zhang, Zesheng}, year={2025}, month={Jun.}, pages={41–46} }">
      📝 BibTeX
    </a>

  </div>

  <div class="metric-row">
    <span class="metric">PSO Algorithm<!--[cite: 4] --></span>
    <span class="metric">Fuzzy Comprehensive Evaluation<!--[cite: 4] --></span>
    <span class="metric">Heuristic Search<!--[cite: 4] --></span>
  </div>

  <details>
    <summary>Read more</summary>
    <div class="detail-box">
      This study addresses the "translational replacement" strategy in old city bungalow renovations by establishing a Logit model to quantify residents' relocation probabilities based on spatial, lighting, and psychological factors<!--[cite: 4] -->. Furthermore, it employs a two-stage heuristic algorithm combining greedy search and PSO to maximize the number and area of vacant complete courtyards while strictly adhering to compensation rules and cost constraints<!--[cite: 4] -->.
    </div>
  </details>
</div>

</div>

<!-- Awards Section -->
<div class="home-section" id="awards">
  <h2 class="home-title" data-icon="🏆">Awards</h2>

  <div class="award-grid">
    <div class="award-card">
      <h3 class="award-name">National Scholarship</h3>
      <div class="award-meta">
        Ministry of Education of the People's Republic of China<br>
        2023-2024 school year
      </div>

      <div class="award-cert">
        <a href="{{ '/images/2023-2024.jpg' | relative_url }}" target="_blank" rel="noopener" aria-label="View 2023-2024 National Scholarship certificate">
          <img src="{{ '/images/2023-2024.jpg' | relative_url }}" alt="Certificate of National Scholarship" width="1200" height="1691" loading="lazy" decoding="async">
        </a>
        <span class="view-hint">View certificate</span>
      </div>
    </div>

    <div class="award-card">
      <h3 class="award-name">National Scholarship</h3>
      <div class="award-meta">
        Ministry of Education of the People's Republic of China<br>
        2024-2025 school year
      </div>

      <div class="award-cert">
        <a href="{{ '/images/2024-2025.jpg' | relative_url }}" target="_blank" rel="noopener" aria-label="View 2024-2025 National Scholarship certificate">
          <img src="{{ '/images/2024-2025.jpg' | relative_url }}" alt="Certificate of National Scholarship" width="1200" height="1626" loading="lazy" decoding="async">
        </a>
        <span class="view-hint">View certificate</span>
      </div>
    </div>

    <div class="award-card">
      <h3 class="award-name">Honorable Mention</h3>
      <div class="award-meta">
        Mathematical Contest in Modeling (MCM/ICM)<br>
        2026 | Team Leader
      </div>

      <div class="award-cert">
        <a href="{{ '/images/MCM_Honorable_Mention.png' | relative_url }}" target="_blank" rel="noopener" aria-label="View MCM/ICM Honorable Mention certificate">
          <img src="{{ '/images/MCM_Honorable_Mention.png' | relative_url }}" alt="Certificate of MCM/ICM Honorable Mention" width="1600" height="1236" loading="lazy" decoding="async">
        </a>
        <span class="view-hint">View certificate</span>
      </div>
    </div>

    <div class="award-card">
      <h3 class="award-name">National Second Prize</h3>
      <div class="award-meta">
        RoboCom Robot Developer Competition<br>
        2025 | Team Leader
      </div>

      <div class="award-cert">
        <a href="{{ '/images/RoboCom_National_Second.jpg' | relative_url }}" target="_blank" rel="noopener" aria-label="View RoboCom National Second Prize certificate">
          <img src="{{ '/images/RoboCom_National_Second.jpg' | relative_url }}" alt="Certificate of RoboCom National Second Prize" width="1000" height="707" loading="lazy" decoding="async">
        </a>
        <span class="view-hint">View certificate</span>
      </div>
    </div>

    <div class="award-card">
  <h3 class="award-name">National Third Prize</h3>
  <div class="award-meta">
    Asia and Pacific Mathematical Contest in Modeling (APMCM)<br>
    2024 | Team Leader
  </div>

  <div class="award-cert">
    <!-- 图片路径已替换为您提供的文件名 -->
    <a href="{{ '/images/Asia and Pacific Mathmatical Contest in Modeling_1.png' | relative_url }}" target="_blank" rel="noopener" aria-label="View 2024 APMCM Third Prize certificate">
      <img src="{{ '/images/Asia and Pacific Mathmatical Contest in Modeling_1.png' | relative_url }}" alt="Certificate of APMCM Third Prize" width="1200" height="850" loading="lazy" decoding="async">
    </a>
    <span class="view-hint">View certificate</span>
  </div>
</div>


  </div>
</div>

<!-- 👇 终极版 JavaScript：处理滑动高亮与点击平滑跳转 👇 -->
<!-- Contact Section -->
<div class="home-section" id="contact">
  <h2 class="home-title" data-icon="✉️">Contact</h2>

  <div class="contact-card">
    <p class="contact-lead">
      I am open to research collaborations on evolutionary computation, intelligent optimization, and applied machine learning. If you are interested in my work, feel free to get in touch.
    </p>

    <div class="action-row">
      <a class="action-btn" href="mailto:zesheng_zhang@163.com">Email me</a>
      <a class="action-btn" href="https://github.com/Zhang-ZeSheng" target="_blank" rel="noopener">GitHub</a>
      <a class="action-btn" href="https://orcid.org/0009-0007-9358-9086" target="_blank" rel="noopener">ORCID</a>
    </div>
  </div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function() {
  // 1. 获取所有带有 ID 的正文板块
  const sections = document.querySelectorAll('.home-section, .bio-card');
  
  // 2. 暴力获取所有可能跳转到这几个板块的导航链接（模糊匹配）
  const navLinks = document.querySelectorAll('#site-nav a[href^="#"]');

  // 3. --- 处理滑动高亮逻辑 ---
  const observerOptions = {
    root: null,
    rootMargin: '-30% 0px -70% 0px', 
    threshold: 0
  };

  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        const currentId = entry.target.getAttribute('id');
        
        navLinks.forEach(link => {
          link.classList.remove('active');
          // 使用 link.hash 获取真实的锚点后缀，无视前面的域名和斜杠
          if (currentId && link.hash === '#' + currentId) {
            link.classList.add('active');
          }
        });
      }
    });
  }, observerOptions);

  sections.forEach(section => {
    if (section.getAttribute('id')) {
      observer.observe(section);
    }
  });

  // 4. --- 处理点击平滑跳转逻辑（接管浏览器的默认跳转） ---
  navLinks.forEach(link => {
    link.addEventListener('click', function(e) {
      if (this.hash !== "") {
        // 阻止浏览器的默认瞬间跳转（或刷新）行为
        e.preventDefault(); 

        // 找到目标板块
        const targetId = this.hash.substring(1);
        const targetElement = document.getElementById(targetId);

        if (targetElement) {
          // 计算目标位置，减去 80 像素的高度（防止导航栏遮挡标题）
          const topPosition = targetElement.getBoundingClientRect().top + window.scrollY - 80;
          
          // 强制平滑滚动
          window.scrollTo({
            top: topPosition,
            behavior: 'smooth'
          });
        }
      }
    });
  });
});
</script>
<!-- 👆 终极版 JavaScript 结束 👆 -->
