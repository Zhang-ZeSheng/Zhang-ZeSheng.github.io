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

  <div class="action-row">
    <a class="action-btn" href="https://orcid.org/0009-0007-9358-9086">ORCID</a>
    <a class="action-btn" href="https://github.com/Zhang-ZeSheng">GitHub</a>
  </div>
</div>

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

<div class="home-section" id="publications">
  <div class="home-title" data-icon="📚">Publications</div>

<div class="pub-card rs">
  <!-- 标签可以根据你的喜好修改，这里我换成了演化计算和特征选择 -->
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

  <!-- Pipeline Figure -->
  <div class="pub-figure">
    <!-- 请确保在 assets/images/ 文件夹下放入对应的流程图，并修改图片名称 -->
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
        <!-- 可以在这里放图表，比如 22 个数据集的实验对比图 -->
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

  <!-- Pipeline Figure -->
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
  <div class="pub-label rs">Remote Sensing · Low-light Enhancement</div>

  <div class="pub-title">
    Towards High-quality Low-Light Remote Sensing Image Enhancement via Geometric and Semantic Prior Guidance
  </div>

  <div class="pub-authors">
    Kang Yang, Jiaqi Zhang, Changqiu Xu, Longfei Xiao, Tong Liang and <strong>Zesheng Zhang*</strong>
  </div>

  <div class="pub-venue">
    International Conference on Neural Information Processing (ICONIP), Melbourne, Australia, 2026</em><br>
    <span style="font-size: 0.9em; font-weight: 600; color: #c0392b;">🏆 CCF-C </span>
  </div>

  <div class="pub-short">
    A low-light remote sensing image enhancement framework that combines an <strong>HVI-based dual-branch design</strong>, geometric-semantic prior guidance, and adaptive sparse refinement.
  </div>

  <!-- Pipeline Figure -->
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



<div class="home-section" id="research-project">
  <div class="home-title" data-icon="🔬">Research Project</div>

  <div class="project-card">
    <div class="project-title">
      Government Question Answering and Retrieval Agent Based on RAG and React
    </div>

    <div class="project-meta">
      Project Leader &nbsp; | &nbsp; Oct. 2025 - Jan. 2026
    </div>

    <div style="line-height: 1.9; color: #374151;">
      Technology stack: Python / LLM / BGE-base-en/ FAISS / BM25 / Prompt Engineer / ReAct Agent<br>
·Build RAG knowledge base in government domain, clean and process 1,529 policy texts +7,625 question and answer pairs, generate 30,833 retrieval chunks by multi-strategy segmentation<br>
·FAISS vector index database is constructed by BGE-base-zh model coding knowledge base, and the inverted keyword index database is constructed. The two-way hybrid retrieval scheme based on cosine similarity (30,000 chunk delay <50ms) and BM25 keyword retrieval (delay <10ms) is adopted, and the problem of insufficient semantic recall of government proper nouns is solved by RRF fusion sorting.<br>
·System Prompt integrates output format constraints, reference annotation rules and reject fabrication instructions, combined with RAG retrieval constraints to effectively alleviate large model illusion and improve the accuracy and authenticity of Q & A.<br>
·Design ReAct reasoning Agent, autonomous scheduling policy retrieval and question-answer matching tool, total reasoning time <5s, WebUI based on Streamlit development, support streaming output and Agent reasoning process visualization
    </div>
  </div>
</div>

<div class="home-section" id="awards">
  <div class="home-title" data-icon="🏆">Awards</div>

  <div class="award-grid">
    <div class="award-card">
  <div class="award-name">National Second Prize</div>
  <div class="award-meta">
    AICOMP Object Detection 2025<br>
    2025 | Team Leader
  </div>

  <div class="award-cert">
    <a href="{{ '/images/SAR.jpg' | relative_url }}" target="_blank">
      <img src="{{ '/images/SAR.jpg' | relative_url }}" alt="Certificate of AICOMP Object Detection 2025">
    </a>
  </div>
</div>

<div class="award-card">
  <div class="award-name">National Second Prize</div>
  <div class="award-meta">
    AICOMP Image Classification 2025<br>
    2025 | Team Leader
  </div>

  <div class="award-cert">
    <a href="{{ '/images/imc.jpg' | relative_url }}" target="_blank">
      <img src="{{ '/images/imc.jpg' | relative_url }}" alt="Certificate of AICOMP Image Classification 2025">
    </a>
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
  </div>
</div>
