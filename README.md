# ⚛️ Vigyan AI: Sovereign STEM Models (Non-Commercial Research Suite)

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
&nbsp;[![Hugging Face Org](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Vigyan--Models-yellow)](https://huggingface.co/shreyansh12183)
&nbsp;[![GitHub](https://img.shields.io/badge/GitHub-Vigyan--AI-blue?logo=github)](https://github.com/shreyansh001boy-tech)

> **Vigyan AI — Varanasi, Uttar Pradesh, India**  
> *Sovereign Deep-Tech AI for STEM Education, Semiconductor VLSI EDA, Circuit Physics & Aerospace Engineering*

---

## 🚀 1-Click Interactive Google Colab Demos

Experience India's sovereign STEM models live with **zero local installation**. Click either badge below to launch an interactive Gradio web interface running on free Google Colab hardware:

| Model Tier | Parameter Size | Primary Use Case | 1-Click Google Colab Launch Badge |
| :--- | :---: | :--- | :---: |
| **Vigyan-7B-STEM-DPO** | **7 Billion** | Frontier Deep STEM Reasoning & DPO Alignment | [![Open 7B in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_7b_demo.ipynb) |
| **Vigyan-2B-STEM-Instruct** | **2.4 Billion** | Ultra-Fast Edge AI, On-Device Tutoring (<2GB VRAM) | [![Open 2B in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_2b_demo.ipynb) |

---

## 📊 Dual-Model Architectural Comparison

```
+-------------------------------------------------------------------------------------------------------------+
|                                    VIGYAN AI DUAL MODEL ARCHITECTURE                                        |
+--------------------------+---------------------------------------+------------------------------------------+
| Feature                  | Vigyan-2B-STEM-Instruct-v1 (Edge)     | Vigyan-7B-STEM-DPO-v1 (Frontier)         |
+--------------------------+---------------------------------------+------------------------------------------+
| Base Architecture        | OLMo-2 2B (~2.4 Billion Parameters)   | OLMo-2 7B (~7.0 Billion Parameters)      |
| Alignment Technique      | STEM Instruction Tuning + Tool Tags   | Direct Preference Optimization (DPO)     |
| VRAM Footprint (4-bit)   | ~1.8 GB VRAM                          | ~5.5 GB VRAM                             |
| Target Deployment        | Raspberry Pi, Laptops, Edge Devices   | Cloud Servers, Workstations, Colab T4    |
| Generation Throughput    | 50–65 tokens / second                 | 18–25 tokens / second                    |
| Primary Specialty        | Rapid circuit math, algebra, tutoring | Multi-step derivations, VLSI, aerospace  |
+--------------------------+---------------------------------------+------------------------------------------+
```

---

## 📦 Quickstart Code Snippets

### 1. Load Vigyan-7B (Frontier DPO Model)
```python
import torch
from transformers import AutoTokenizer, AutoModelForCausalLM, BitsAndBytesConfig
from peft import PeftModel

BASE_MODEL = "shreyansh12183/Shreyansh-STEM-AI-7B-Final"
ADAPTER = "shreyansh12183/Vigyan-7B-STEM-DPO-v1"

tokenizer = AutoTokenizer.from_pretrained(ADAPTER, trust_remote_code=True)
bnb_config = BitsAndBytesConfig(load_in_4bit=True, bnb_4bit_quant_type="nf4", bnb_4bit_compute_dtype=torch.float16)

base = AutoModelForCausalLM.from_pretrained(BASE_MODEL, quantization_config=bnb_config, device_map="auto")
model = PeftModel.from_pretrained(base, ADAPTER).eval()

prompt = "<|im_start|>user\nCalculate the Thevenin maximum power deliverable if Vth = 24V and Rth = 6 ohms.<|im_end|>\n<|im_start|>assistant\n"
outputs = model.generate(**tokenizer(prompt, return_tensors="pt").to("cuda"), max_new_tokens=300, do_sample=False)
print(tokenizer.decode(outputs[0], skip_special_tokens=True))
```

### 2. Load Vigyan-2B (Ultra-Fast Edge Model)
```python
import torch
from transformers import AutoTokenizer, AutoModelForCausalLM, BitsAndBytesConfig
from peft import PeftModel

BASE_MODEL = "shreyansh12183/Shreyansh-STEM-AI-2B-v3"
ADAPTER = "shreyansh12183/Vigyan-2B-STEM-Instruct-v1"

tokenizer = AutoTokenizer.from_pretrained(ADAPTER, trust_remote_code=True)
bnb_config = BitsAndBytesConfig(load_in_4bit=True, bnb_4bit_quant_type="nf4", bnb_4bit_compute_dtype=torch.float16)

base = AutoModelForCausalLM.from_pretrained(BASE_MODEL, quantization_config=bnb_config, device_map="auto")
model = PeftModel.from_pretrained(base, ADAPTER).eval()

prompt = "<|im_start|>user\nCalculate the equivalent resistance of 150 ohms and 300 ohms in parallel.<|im_end|>\n<|im_start|>assistant\n"
outputs = model.generate(**tokenizer(prompt, return_tensors="pt").to("cuda"), max_new_tokens=200, do_sample=False)
print(tokenizer.decode(outputs[0], skip_special_tokens=True))
```

---

## 📜 Non-Commercial License Notice

Both models and their associated weights are released under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license.

- **Permitted Free Use:** Academic research, educational exploration, university coursework, and personal non-commercial experimentation.
- **Commercial Restrictions:** Any commercial deployment, commercial tutoring platform integration, defense contractor use, or proprietary API hosting requires an explicit enterprise commercial license from **Vigyan AI**.
- **Commercial & Enterprise Inquiries:** Contact Vigyan AI Founder at IIT BHU / Varanasi.
