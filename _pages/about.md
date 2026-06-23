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

I have one paper accepted at **ICML 2026 (CCF-A)** as the first author, one paper under review at **npj Computational Materials** as the first author, and one paper to be submitted to **AAAI 2027 (CCF-A)** as the primary author.

📫 **Contact:** `rhliu25 [at] m.fudan.edu.cn`


# 🔥 News
- *2026.06*: &nbsp;✍️ Manuscript **"From Extraction to Publication: EviPGCE, an Evidence-Governed Harness for Scientific Database Curation"** to be submitted to **AAAI 2027** (CCF-A).
- *2026.02*: &nbsp;🎉🎉 Our paper **"Equivariant Covariance Tensors: Guaranteed SPD Uncertainty for Tensor-Valued Geometric Learning"** has been accepted to **ICML 2026** as a **Poster**.
- *2026.01*: &nbsp;📨 Our paper **"Topology-aware E(3)-equivariant learning for physically consistent piezoelectric tensor prediction"** has been submitted to **npj Computational Materials** (IF 11.9).
- *2025.09*: &nbsp;🎓 Started Ph.D. study at Fudan University.
- *2025.06*: &nbsp;🎓 Received B.Eng. in Automation from Beijing Institute of Technology.


# 📝 Publications 

<div class='paper-box'>
<div class='paper-box-image'><div><div class="badge">AAAI 2027</div><img src='images/evipgce_architecture.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**From Extraction to Publication: EviPGCE, an Evidence-Governed Harness for Scientific Database Curation**

**Ruihan Liu**, et al.

*To be submitted to AAAI 2027* (CCF-A)

- Reframes literature curation as **open-world candidate proposal → closed-world deterministic publication**, separating LLM candidate generation from publication authority.
- A deterministic harness binds candidates to immutable evidence, independently verifies property–value–unit tuples, applies DomainPack policies, resolves conflicts, and materializes only **verified-strong** observations.
- Evaluated on three **Gold-50** benchmarks (**150 DOIs**, **1,956** records) across piezoelectric, thermoelectric, and superconducting domains; compiled evidence improves published-observation F1 in all domains (piezo **0.675→0.760**, thermo **0.285→0.363**, SC **0.494→0.519**).

</div>
</div>


<div class='paper-box'>
<div class='paper-box-image'><div><div class="badge">ICML 2026</div><img src='images/eqcov_thumbnail.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[**Equivariant Covariance Tensors: Guaranteed SPD Uncertainty for Tensor-Valued Geometric Learning**](https://icml.cc/virtual/2026/poster/62008)

**Ruihan Liu**, Yu Ji, Jianbo Yu, Shifu Yan, Qingchao Jiang

*International Conference on Machine Learning* (**ICML 2026**, Poster, CCF-A) &nbsp;|&nbsp; [Paper](files/eqcov_icml2026.pdf) &nbsp;|&nbsp; [Poster page](https://icml.cc/virtual/2026/poster/62008)

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

**EviPGCE / Piepaper: Evidence-Governed Scientific Database Curation** &nbsp;·&nbsp; *to be submitted to AAAI 2027, primary author* &nbsp;·&nbsp; *2026.02 – 2026.05*

Reframes scientific extraction as open-world candidate proposal followed by closed-world deterministic publication. The LLM proposes structured candidates from evidence packets; a deterministic harness binds, verifies, and gates records before materialization.

- Designed a **publication-authority layer** where the harness enforces Schema / Domain / Bound / Verified / Valid / ConflictFree checks and materializes only **verified-strong** observations.
- Implemented **evidence compilation and independent content verification**: parses immutable evidence blocks into bounded packets and verifies property–value–unit, material, and condition co-localization.
- Built a **swappable DomainPack policy surface** covering piezoelectric, thermoelectric, and superconducting domains.
- Validated on three **Gold-50** benchmarks (**150 DOIs**, **1,956** records): compiled evidence improves published-observation F1 (piezo **0.675→0.760**, thermo **0.285→0.363**, SC **0.494→0.519**).


# 🎖 Honors and Awards
- *Undergrad*: Four-semester university-level First-class Scholarship (Top 5%).
- *2023*: Diwen Scholarship (迪文奖学金, 45 recipients university-wide).
- *Competitions*: National First Prize, China Intelligent Robot Combat and Skills Competition; National Second Prize, China Undergraduate Mathematical Contest in Modeling; MCM Meritorious Winner.


# 📖 Education
- *2025.09 – 2030.07 (expected)*, **Ph.D.**, Computer Science and Technology, **Fudan University**, Shanghai, China.
- *2021.09 – 2025.06*, **B.Eng.**, Automation, **Beijing Institute of Technology**, Beijing, China.


# 💻 Technical Skills
- **AI for Science / Deep Learning:** PyTorch, e3nn, GNN, E(3)-equivariant networks, uncertainty quantification, tensor prediction.
- **LLM / Agent:** multi-agent orchestration, LLM extraction, evidence grounding.
