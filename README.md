# ⚛️ Vigyan-7B: Frontier STEM Reasoning Model (Non-Commercial Demo)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_7b_demo.ipynb)
&nbsp;[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
&nbsp;[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Vigyan--7B--STEM--DPO-yellow)](https://huggingface.co/shreyansh12183/Vigyan-7B-STEM-DPO-v1)

> **Vigyan AI — Varanasi, Uttar Pradesh, India**  
> *Sovereign Deep-Tech AI for STEM, Semiconductor EDA, Circuit Physics & Aerospace Engineering*

---

## 🚀 1-Click Interactive Google Colab Demo

Experience **Vigyan-7B-STEM-DPO-v1** live with **zero local installation**. Click the badge below to launch an interactive Gradio web interface running on a free Google Colab T4 GPU:

👉 **[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyansh001boy-tech/vigyan-7b-demo/blob/main/vigyan_7b_demo.ipynb)**

### What You Can Test in the Demo:
- **Circuit Physics & RF:** Parallel/series resistor networks, Thevenin equivalent maximum power transfer, transmission line impedance ($Z_0 = \sqrt{L/C}$), and reflection coefficients ($\Gamma$).
- **VLSI EDA & Silicon Systems:** Inverter propagation delay ($t_p$), interconnect sheet resistance ($R_s \cdot L/W$), CMOS dynamic power dissipation ($C_L V_{DD}^2 f$), and pipeline clock timing slack.
- **Aerospace & Orbital Dynamics:** Circular Low Earth Orbit (LEO) velocity, escape velocity, Tsiolkovsky rocket equation ($\Delta v$), and Hohmann orbital transfers.
- **Advanced Mathematics:** Definite integration, matrix determinants, quadratic optimization, and eigenvalues.

---

## 📦 Local Usage Snippet (Hugging Face)

```python
import torch
from transformers import AutoTokenizer, AutoModelForCausalLM, BitsAndBytesConfig
from peft import PeftModel

BASE_MODEL = "shreyansh12183/Shreyansh-STEM-AI-7B-Final"
ADAPTER = "shreyansh12183/Vigyan-7B-STEM-DPO-v1"

# 1. Load Tokenizer
tokenizer = AutoTokenizer.from_pretrained(ADAPTER, trust_remote_code=True)

# 2. 4-bit Quantization Config (Fits in 6 GB VRAM)
bnb_config = BitsAndBytesConfig(
    load_in_4bit=True,
    bnb_4bit_quant_type="nf4",
    bnb_4bit_compute_dtype=torch.float16,
    bnb_4bit_use_double_quant=True
)

# 3. Load Base Model & Attach DPO LoRA Adapter
base_model = AutoModelForCausalLM.from_pretrained(
    BASE_MODEL,
    quantization_config=bnb_config,
    device_map="auto",
    torch_dtype=torch.float16
)
model = PeftModel.from_pretrained(base_model, ADAPTER)
model.eval()

# 4. Run Inference
prompt = "<|im_start|>user\nCalculate the Thevenin maximum power deliverable if Vth = 24V and Rth = 6 ohms.<|im_end|>\n<|im_start|>assistant\n"
inputs = tokenizer(prompt, return_tensors="pt").to("cuda")

with torch.no_grad():
    outputs = model.generate(**inputs, max_new_tokens=256, do_sample=False)

print(tokenizer.decode(outputs[0], skip_special_tokens=True))
```

---

## 📜 Non-Commercial License Notice

This model and its associated weights are released under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license.

- **Permitted Free Use:** Academic research, educational exploration, university coursework, and personal non-commercial experiments.
- **Commercial Restrictions:** Any commercial deployment, monetization, commercial tutoring platform integration, defense contractor use, or proprietary API hosting requires an explicit enterprise commercial license from **Vigyan AI**.
- **Commercial Inquiries:** Contact Vigyan AI Founder at IIT BHU / Varanasi.
