# 🏛️ Vigyan AI: Sovereign STEM Foundation Model Zoo
### 1-Click Google Colab Demos & Open-Weight Research Releases (1.5B to 32B)

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
[![Hugging Face Org](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-shreyansh12183-yellow)](https://huggingface.co/shreyansh12183)
[![Founder](https://img.shields.io/badge/Architect-Shreyansh%20Singh-blue)](https://github.com/shreyansh001boy-tech)
[![GitHub Stars](https://img.shields.io/github/stars/shreyansh001boy-tech/vigyan-7b-demo?style=social)](https://github.com/shreyansh001boy-tech/vigyan-7b-demo)

---

## 🌟 Executive Overview

**Vigyan AI** is India's sovereign scientific and mathematical foundation model ecosystem architected and developed by **Shreyansh Singh**. 

Designed to out-reason generalized commercial LLMs on high-stakes STEM domains (JEE Mains/Advanced, CBSE 12/10 Boards, Olympiad MATH, synthesizable Verilog HDL, and molecular chemistry), the Vigyan AI model zoo spans from **1.5B on-device models** to **32B frontier reasoning engines**.

Every model listed below is released for **free non-commercial educational and academic research use** under the **Creative Commons CC BY-NC 4.0** license, with **1-click interactive Google Colab notebooks** that launch on free Tesla T4 GPUs in under 60 seconds.

---

## 🚀 1-Click Google Colab Interactive Launch Matrix

Every notebook below runs on Google Colab's **free tier (Tesla T4 GPU)** with **zero setup**, **zero local GPU requirements**, and includes an embedded **Gradio WebUI**:

| Model Tier | Model Name & Architecture | Primary Domain / Specialty | 1-Click Colab Launch |
| :--- | :--- | :--- | :---: |
| **Flagship 7B MoE** | `vigyan-olmoe-1b-7b-masterpiece` (64 Sparse Experts, Top-8 Routing) | **Sovereign Exam Core:** JEE Mains, CBSE, Olympiad Math (~85 tok/s) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_7b_moe_flagship_demo.ipynb) |
| **Frontier 32B Titan** | `Vigyan-AI-32B-Titan-v1` (32B Heavy STEM Reasoner) | **PhD Research:** Multi-hop theorems & deep scientific proofs | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_32b_titan_demo.ipynb) |
| **Frontier 7B Unified** | `Vigyan-7B-STEM-DPO-v1` (OLMo-2 7B Dense) | **Deterministic Physics & Circuits:** Multi-step derivations | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_7b_demo.ipynb) |
| **2B Policy RL (GRPO)**| [`vigyan-2b-reasoning-grpo`](https://huggingface.co/shreyansh12183/vigyan-2b-reasoning-grpo) | **Reinforcement Learning:** Autonomous `<think>` scratchpad reasoning | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_2b_grpo_reasoning_demo.ipynb) |
| **2B DUS + CPT Healed**| [`Shreyansh-STEM-AI-2B-v3`](https://huggingface.co/shreyansh12183/Shreyansh-STEM-AI-2B-v3) | **22-Layer DUS:** Spliced layer expansion + CPT seam-healed manifold | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_2b_dus_cpt_healed_demo.ipynb) |
| **Edge 1.5B 4x-MoE** | [`Vigyan-1.5B-4x-MoE`](https://huggingface.co/shreyansh12183/Vigyan-1.5B-4x-MoE) | **Compact Edge MoE:** Sub-1GB RAM, standalone Q4_K_M GGUF | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_1_5b_moe_demo.ipynb) |
| **Multi-Expert 3B MoE**| `Vigyan-3B-4x-MoE` (Qwen 2.5 3B, 4 Experts) | **Balanced Code & Math:** Fast student tutor for laptops | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_3b_moe_demo.ipynb) |
| **Universal Edge 2B** | `Vigyan-2B-STEM-Instruct-v1` (OLMo-2 2B) | **Edge SLM:** Rapid homework solver (boots in 15s, 1.8GB VRAM) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_2b_demo.ipynb) |
| **Specialist: Silicon RTL**| `olmo2-7b-silicon-rtl-eda` | **Chip Architecture:** Synthesizable Verilog HDL & ASIC timing | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/domain_demos/silicon_rtl_eda_demo.ipynb) |
| **Specialist: Pure Math** | `olmo2-7b-phd-pure-math` | **Advanced Proofs:** Differential geometry, algebraic topology | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/domain_demos/phd_pure_math_demo.ipynb) |
| **Specialist: Bio-Chem** | `olmo2-7b-biomed-chem` | **Molecular Informatics:** Organic pathways, crystal field spin | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/domain_demos/biomed_chem_demo.ipynb) |
| **Specialist: Astro-Logic**| `olmo2-7b-astro-logic` | **Astrophysics:** Orbital mechanics, relativistic calculations | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/domain_demos/astro_logic_demo.ipynb) |
| **Specialist: Legal** | `Vidhi-AI-Instruct` | **Indian Law:** IPC / BNS statutory interpretation, case law | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/domain_demos/vidhi_ai_legal_demo.ipynb) |

---

## 🔬 Specialized Qwen-Family STEM Adapters (1.5B & 3B)

Dedicated 1-click Google Colab notebooks for each fine-tuned domain adapter in the Qwen family, calibrated across Science, Technology, Engineering, and Mathematics:

### ⚡ 1.5B Class: DeepSeek-R1 Distill Qwen Adapters (with Reasoning Tokens)
*Base Model:* `deepseek-ai/DeepSeek-R1-Distill-Qwen-1.5B` | *Colab Footprint:* ~1.5 GB VRAM in 4-bit NF4

| Domain | Model Adapter | Primary Specialties | 1-Click Colab Launch |
| :--- | :--- | :--- | :---: |
| **Science** | [`vigyan-1.5b-adapter-science`](https://huggingface.co/shreyansh12183/vigyan-1.5b-adapter-science) | Chemistry equilibrium, wave optics, cellular ATP synthesis | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/qwen_stem_demos/1_5b_science_colab.ipynb) |
| **Technology** | [`vigyan-1.5b-adapter-technology`](https://huggingface.co/shreyansh12183/vigyan-1.5b-adapter-technology) | B-Tree vs LSM storage, TCP congestion dynamics, cycle detection | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/qwen_stem_demos/1_5b_technology_colab.ipynb) |
| **Engineering** | [`vigyan-1.5b-adapter-engineering`](https://huggingface.co/shreyansh12183/vigyan-1.5b-adapter-engineering) | RLC resonance, cantilever deflection, PID control overshoot | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/qwen_stem_demos/1_5b_engineering_colab.ipynb) |
| **Mathematics** | [`vigyan-1.5b-adapter-mathematics`](https://huggingface.co/shreyansh12183/vigyan-1.5b-adapter-mathematics) | King's rule integrals, Fermat's Little Theorem, AP sequences | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/qwen_stem_demos/1_5b_mathematics_colab.ipynb) |

### 🔬 3B Class: Qwen 2.5 Instruct Adapters (High-Fidelity Engineering)
*Base Model:* `Qwen/Qwen2.5-3B-Instruct` | *Colab Footprint:* ~2.5 GB VRAM in 4-bit NF4

| Domain | Model Adapter | Primary Specialties | 1-Click Colab Launch |
| :--- | :--- | :--- | :---: |
| **Science** | [`vigyan-3b-adapter-science`](https://huggingface.co/shreyansh12183/vigyan-3b-adapter-science) | Crystal Field splitting, apex angular momentum, Gibbs free energy | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/qwen_stem_demos/3b_science_colab.ipynb) |
| **Technology** | [`vigyan-3b-adapter-technology`](https://huggingface.co/shreyansh12183/vigyan-3b-adapter-technology) | Raft consensus, lock-free ring buffer atomics, MESI cache coherence | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/qwen_stem_demos/3b_technology_colab.ipynb) |
| **Engineering** | [`vigyan-3b-adapter-engineering`](https://huggingface.co/shreyansh12183/vigyan-3b-adapter-engineering) | Sallen-Key filter transfer functions, inverted pendulum, FFT | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/qwen_stem_demos/3b_engineering_colab.ipynb) |
| **Mathematics** | [`vigyan-3b-adapter-mathematics`](https://huggingface.co/shreyansh12183/vigyan-3b-adapter-mathematics) | Linear differential equations, matrix diagonalization, modular proofs | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/qwen_stem_demos/3b_mathematics_colab.ipynb) |

---


---

## 🧬 7-Pillar Modern Post-Training & Architecture Methodology

Rather than relying on basic supervised fine-tuning, the Vigyan AI models were developed through an institutional multi-stage lifecycle:

```
[Standard Base SLM]
       │
       ▼  1. Depth Up-Scaling (DUS)
[22-Layer Spliced Architecture]  -->  (Interface Discontinuity / Layer Shock)
       │
       ▼  2. Continual Pre-Training (CPT) Seam Healing (2,400+ Parquet Shards)
[CPT-Healed Manifold: shreyansh-1B-SLM-pretrain-stem-english]
       │
       ▼  3. All-Module Linear SFT (7 Projections, Dynamic Early-Stop @ Loss 0.1335)
[Cured 0.048 Collapse --> Generalizing STEM Model]
       │
       ├──────────────────────────────────────────┐
       ▼  4. GRPO Policy Gradient RL              ▼  5. DPO Preference Alignment
[vigyan-2b-reasoning-grpo]                 [Vigyan-7B-STEM-DPO-v1]
(Native <think> Reasoning Tokens)          (Deterministic Physics & Calculus)
       │                                          │
       └────────────────────┬─────────────────────┘
                            ▼  6. Sparse MoE Upcycling (Top-1 / Top-8)
       [Vigyan 1.5B 4x-MoE & Vigyan OLMoE 1B-7B (64 Experts)]
                            │
                            ▼  7. Sovereign Edge Delivery (Q4_K_M GGUF + SymPy AST)
       [Vigyan-Models-GGUF & C++ KùzuDB GraphRAG Engine]
```

1. **Depth Up-Scaling (DUS):** SOLAR-style layer expansion scaling depth to 22 layers without full pretraining compute.
2. **CPT Seam Healing:** Continual Pre-Training across 13.14 GB of raw STEM literature (`shreyansh-1B-SLM-pretrain-stem-english`) to re-align query-key subspaces across spliced layers.
3. **All-Module Linear SFT:** Full-projection targeting (`q, k, v, o, gate, up, down`) with dynamic early-stopping at loss 0.1335, completely eliminating the historical 0.048 overfit collapse.
4. **Group Relative Policy Optimization (GRPO):** DeepSeek-R1 style reinforcement learning eliciting self-directed step-by-step reasoning tokens (`<think>`).
5. **Direct Preference Optimization (DPO):** Preference modeling for verifiable calculus and circuit derivations.
6. **Sparse MoE Upcycling:** Top-1 (1.5B) and Top-8 (7B) routing with contrasting negative prompt router calibration.
7. **Sovereign GGUF & Neuro-Symbolic Grounding:** Standalone Q4_K_M quantizations coupled with exact SymPy AST symbolic engines (+162.5% accuracy gain over unassisted baselines).

## 💻 Hardware Compatibility & Local Execution Options

Users can run Vigyan AI models across virtually any device:

```
  [Mobile / WebGPU]            [Budget Laptops]            [Consumer RTX / Macs]         [Workstations / Servers]
   Vigyan 1.5B MoE             Vigyan 2B SLM               Vigyan 7B MoE (3.8GB)          Vigyan 32B Titan (14-19GB)
   < 1 GB RAM (Chrome)         4-8 GB RAM (Ollama)         8-16 GB RAM (LM Studio)        24 GB VRAM / Multi-GPU
```

### 1. Run Locally via Ollama (1 Command)
```bash
# Run 2B Edge STEM Model
ollama run hf.co/shreyansh12183/Vigyan-Models-GGUF:vigyan-2b-stem-q4_k_m.gguf

# Run 2B Reasoning Model with <think> steps
ollama run hf.co/shreyansh12183/Vigyan-Models-GGUF:vigyan-2b-reasoning-q4_k_m.gguf
```

### 2. Run with Python `transformers` (4-bit NF4 Acceleration)
```python
import torch
from transformers import AutoTokenizer, AutoModelForCausalLM, BitsAndBytesConfig

MODEL_ID = "shreyansh12183/olmo2-7b-silicon-rtl-eda"

bnb_config = BitsAndBytesConfig(load_in_4bit=True, bnb_4bit_quant_type="nf4", bnb_4bit_compute_dtype=torch.float16)
tokenizer = AutoTokenizer.from_pretrained(MODEL_ID)
model = AutoModelForCausalLM.from_pretrained(MODEL_ID, quantization_config=bnb_config, device_map="auto")

prompt = "<|user|>\nWrite a synthesizable 8-bit pipelined accumulator in Verilog with synchronous reset.\n<|assistant|>\n"
inputs = tokenizer(prompt, return_tensors="pt").to("cuda")
outputs = model.generate(**inputs, max_new_tokens=300)
print(tokenizer.decode(outputs[0], skip_special_tokens=True))
```

---

## ⚙️ Free Online Quantization (GGUF Conversion)

To quantize any model in this repository into standalone `.gguf` for free without a local GPU:
1. Visit Hugging Face's official [**ggml-org/gguf-my-repo Space**](https://huggingface.co/spaces/ggml-org/gguf-my-repo).
2. Enter the Hugging Face model repository ID (e.g. `shreyansh12183/olmo2-7b-silicon-rtl-eda`).
3. Select your desired quantization format: **`Q4_K_M`** (recommended for laptops) or **`Q5_K_M`** (high fidelity).
4. Click **Convert**. The space builds the GGUF file on free cloud compute and commits it directly to your Hugging Face account at **$0.00 cost**.
5. For LoRA adapters, use the sister space [**ggml-org/gguf-my-lora**](https://huggingface.co/spaces/ggml-org/gguf-my-lora).

---

## 📜 Non-Commercial License & Sovereign Attribution

All models, adapters, datasets, and demonstration notebooks in this repository are released under the:
**Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license.

### ✅ Permitted Free Use:
* University coursework, academic research, and classroom teaching.
* High school & competitive exam study preparation (JEE, CBSE, Olympiads).
* Independent developer exploration and personal learning.

### 🚫 Commercial Restrictions:
* Any commercial deployment, proprietary SaaS wrapper, commercial tutoring platform, defense contractor use, or paid API hosting requires an explicit enterprise commercial license.
* For enterprise licensing, bespoke domain fine-tuning, or institutional partnerships, contact:
  * **Founder & Chief Architect:** Shreyansh Singh
  * **Organization:** Vigyan AI / ExperimentLab
  * **GitHub:** [@shreyansh001boy-tech](https://github.com/shreyansh001boy-tech)
