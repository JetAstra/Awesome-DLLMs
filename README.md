# Diffusion Language Models (DLMs)

A survey-style paper list for **Diffusion Language Models (DLMs)** and related topics (discrete/continuous diffusion for language, hybrid AR–diffusion, and multimodal diffusion(-language) models).

**Organization:** **Paradigm → Training (Pre/Post, incl. RL) → Inference/Acceleration → Multimodal & Applications**

---

## How I categorize papers

### 1) Paradigm
- **Discrete-space DLMs** (token-level / masked / transition-matrix / DFM-style)
- **Continuous-space DLMs** (embedding/latent diffusion; continuous-time views)
- **Hybrid AR–Diffusion** (e.g., block diffusion, AR init + diffusion refinement)
- **Unified / Multimodal Paradigms** (shared representations across modalities)

---

### 2) Training
#### 2.1 Pre-training
- Objective / formulation (e.g., masked diffusion, DFM, continuous-time discrete denoising)
- Training recipe (mask/noise schedule, loss weighting, curriculum)
- Scaling / data / architecture recipe

#### 2.2 Post-training
- **SFT / instruction tuning**
- **RL / policy optimization**
- **Distillation / compression** post-training (step distillation, teacher–student)

---

### 3) Inference & Acceleration
- Unmasking / remasking policies
- Parallel decoding (heuristic or learned)
- Guidance / constraints
- Caching & reuse (KV/feature cache, adaptive refresh/eviction)
- Distillation / quantization / systems optimizations

---

### 4) Multimodal & Applications
#### 4.1 Multimodal Understanding
Multimodal input → mainly **text output** (VQA, DocVQA/OCR reasoning, video QA, audio understanding).

#### 4.2 Unified Multimodal Understanding & Generation
Unifies understanding + generation; can output **non-text modalities** (t2i/t2v, editing, any-to-any).

#### 4.3 Applications & Benchmarks
Domain tasks, evaluation suites, analysis papers.

---

## Paper List

### Surveys / Reading Guides

| Date   | Title | Paper | Repo|
|:------:|:------|:-----:|:-----:|
| 2025.6 | Discrete Diffusion in Large Language and Multimodal Models: A Survey | [paper](https://arxiv.org/abs/2506.13759) | [github](https://github.com/LiQiiiii/DLLM-Survey)|
| 2025.8 | A Survey of Diffusion Language Models | [paper](https://arxiv.org/pdf/2508.10875) | [github](https://github.com/VILA-Lab/Awesome-DLMs) |
| 2026.1 | Efficient Diffusion Language Models: A Comprehensive Survey | [paper](https://www.authorea.com/users/1021451/articles/1381451-efficient-diffusion-language-models-a-comprehensive-survey) | [github](https://github.com/FelixMessi/Awesome-Efficient-dLLMs)|
---

### Paradigm
#### Discrete-space


#### Continuous-space


#### Hybrid AR–Diffusion / Block Diffusion


#### Unified / Multimodal Paradigms


---

### Training
#### Pre-training


#### Post-training
##### SFT / Instruction Tuning
##### RL / Policy Optimization
| Date    | Paper | Code | Venue |Summary |
|:------:|:------|:-----:|:----:|:-----:|
| 2025.4 | [[**D1**] d1: Scaling Reasoning in Diffusion Large Language Models via Reinforcement Learning](https://arxiv.org/pdf/2504.12216)  | [[code]](https://github.com/dllm-reasoning/d1) |  | |
|2025.5 | [[**VRPO**] LLaDA 1.5: Variance-Reduced Preference Optimization for Large Language Diffusion Models](https://arxiv.org/abs/2505.19223) | [[code]](https://github.com/ML-GSAI/LLaDA-1.5) |  | |
| 2025.6 | [[**Coupled-GRPO**] Coupled-GRPO: Enhancing Diffusion Language Models with Coupled Generative Reinforcement Policy Optimization](https://arxiv.org/abs/2506.20639) | [[code]](https://github.com/apple/ml-diffucoder) |  | |
| 2025.8  | [[**MDPO**] MDPO: Overcoming the Training-Inference Divide of Masked Diffusion Language Models](https://arxiv.org/abs/2509.06949) | [[code]](https://github.com/autonomousvision/mdpo) |  | |
| 2025.9  | [[**TraceRL**] TraceRL: Revolutionizing Reinforcement Learning Framework for Diffusion Large Language Models](https://arxiv.org/abs/2509.06949) | [[code]](https://github.com/Gen-Verse/dLLM-RL) | ICLR 2026 | |
| 2025.10 | [[**BGPO**] Boundary-Guided Policy Optimization for Memory-efficient RL of Diffusion Large Language Models](https://arxiv.org/pdf/2510.11683) | [[code]](https://github.com/THU-KEG/BGPO) |  | |
|2025.10 | [[**SPG**] Sandwiched Policy Gradient for Masked Diffusion Language Models](https://arxiv.org/abs/2510.09541) | [[code]](https://github.com/facebookresearch/SPG) | NeurIPS 2025 | |
| 2025.12 | [[**ESPO**] Principled RL for Diffusion LLMs Emerges from a Sequence-Level Perspective](https://arxiv.org/pdf/2512.03759) | [[code]](https://github.com/FelixMessi/Awesome-Efficient-dLLMs) |  | |

##### Distillation / Compression
---

### Inference & Acceleration


---

### Multimodal & Applications
#### Multimodal Understanding


#### Unified Multimodal Understanding & Generation


#### Applications & Benchmarks


