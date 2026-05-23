---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<span class='anchor' id='about-me'></span>

Hi, I am **Ruihan Liu (刘睿涵)**, a first-year Ph.D. student in Computer Science and Technology at **Fudan University**, supervised by Prof. Jianbo Yu. Before that, I received my B.Eng. degree in Automation from **Beijing Institute of Technology** in 2025.

My research lies at the intersection of **AI for Science** and **geometric deep learning**. I focus on building physically consistent models for crystalline materials and tensor-valued properties, with particular interest in:

- **E(3)-equivariant neural networks** for tensor property prediction (piezoelectric, dielectric, elasticity).
- **Uncertainty quantification** on the SPD manifold under exact symmetry constraints.
- **LLM agents and data infrastructure** for scientific literature mining and curated dataset construction.

I have one paper accepted at **ICML 2026 (CCF-A)** as the first author, and one paper under review at **npj Computational Materials** as the first author.

📫 **Contact:** `rhliu25 [at] m.fudan.edu.cn`


# 🔥 News
- *2026.05*: &nbsp;✍️ Manuscript of **Piepaper** (Physics-Guided Agentic Data Infrastructure) under preparation.
- *2026.02*: &nbsp;🎉🎉 Our paper **"Equivariant Covariance Tensors: Guaranteed SPD Uncertainty for Tensor-Valued Geometric Learning"** has been accepted to **ICML 2026** as a **Poster**.
- *2026.01*: &nbsp;📨 Our paper **"Topology-aware E(3)-equivariant learning for physically consistent piezoelectric tensor prediction"** has been submitted to **npj Computational Materials** (IF 11.9).
- *2025.09*: &nbsp;🎓 Started Ph.D. study at Fudan University.
- *2025.06*: &nbsp;🎓 Received B.Eng. in Automation from Beijing Institute of Technology.


# 📝 Publications 

<div class='paper-box'>
<div class='paper-box-image'><div><div class="badge">ICML 2026</div><img src='images/eqcov_thumbnail.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Equivariant Covariance Tensors: Guaranteed SPD Uncertainty for Tensor-Valued Geometric Learning**

**Ruihan Liu**, Yu Ji, Jianbo Yu, Shifu Yan, Qingchao Jiang

*International Conference on Machine Learning* (**ICML 2026**, Poster, CCF-A)

- We propose an E(3)-equivariant full-covariance UQ framework that, in the Kelvin–Mandel basis, jointly predicts the tensor mean and a complete 6×6 covariance matrix.
- A representation-theoretic SPD covariance head with 21 d.o.f. is constructed via the matrix exponential, simultaneously guaranteeing positive definiteness and rotational equivariance.
- Achieves MAE **0.078** on ModelNet40 inertia tensors and MAE **1.55** on Materials Project dielectric tensors, with extensive ablation on Gaussian NLL / Energy Score / Log-Euclidean equivariant scoring objectives.

</div>
</div>


<div class='paper-box'>
<div class='paper-box-image'><div><div class="badge">npj CM (under review)</div><img src='images/topotenet_thumbnail.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Topology-aware E(3)-equivariant learning for physically consistent piezoelectric tensor prediction**

**Ruihan Liu**, Jianbo Yu, Yu Ji, Hang Ruan, Xiaofeng Yang

Submitted to ***npj Computational Materials*** (Q1 top, IF 11.9)  &nbsp;|&nbsp;  [Code](https://github.com/future3317/TopoTENet)

- Proposes a **topology-conditioned equivariant attention** that injects SLICES periodic-topology labels and space-group priors into E(3)-equivariant message passing via topology bias, MoE-gated key/value, and edge-to-node FiLM modulation.
- Designs a differentiable point-group projection that suppresses symmetry-forbidden tensor components by about **8 orders of magnitude**.
- Reaches MAE **0.132** and RMSE **0.302** on 369 test crystals, reducing RMSE by **22.4%** over the SOTA EATGNN baseline; ablating all topology degrades MAE by **49.2%**.

</div>
</div>


# 🛠 Selected Projects

**Piepaper: Physics-Guided Agentic Data Infrastructure** &nbsp;·&nbsp; *manuscript in preparation, primary author* &nbsp;·&nbsp; *2026.02 – 2026.05*

LLM multi-agent orchestration that turns scientific literature end-to-end into datasets with evidence binding and physics validation, unifying extraction, validation, repair, materialization, and strict export under a single quality gate.

- Led the development of a **literature-to-database LLM data pipeline**, covering XML/HTML parsing, evidence-block construction, agentic extraction, physics validation, automatic repair, materialization, and strict export.
- Designed a **PGCE quality-gating mechanism** that couples material priors, evidence binding, schema validation, and publication gates with multi-agent orchestration, isolating orphan, legacy, low-confidence, and physics-inconsistent records.
- Curated and unified **671** DOIs, **7,707** evidence blocks, and **2,872** materialized records, distilling **500** SFT-ready strict records and **505** RAG-ready observations.


# 🎖 Honors and Awards
- *Undergrad*: Four-semester university-level First-class Scholarship (Top 5%).
- *2023*: Difan Scholarship (45 recipients university-wide).
- *Competitions*: National First Prize, China Intelligent Robot Combat and Skills Competition; National Second Prize, China Undergraduate Mathematical Contest in Modeling; MCM Meritorious Winner.


# 📖 Education
- *2025.09 – 2030.07 (expected)*, **Ph.D.**, Computer Science and Technology, **Fudan University**, Shanghai, China.
- *2021.09 – 2025.06*, **B.Eng.**, Automation, **Beijing Institute of Technology**, Beijing, China.


# 💻 Technical Skills
- **AI for Science / Deep Learning:** PyTorch, e3nn, GNN, E(3)-equivariant networks, uncertainty quantification, tensor prediction.
- **LLM / Agent:** multi-agent orchestration, LLM extraction, evidence grounding.
