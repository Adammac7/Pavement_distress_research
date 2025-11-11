# 🛣️ Pavement Distress Classification with VMamba

**Author:** Adam Macfarlane  
**Institution:** San Diego State University  
**Project:** AI4Business Research Lab – Pavement Distress Detection  
**Date:** 2024  

---

## 📘 Overview
This repository documents my research project on **pavement distress classification using Vision Mamba (VMamba)** — a modern vision architecture that improves image-based infrastructure inspection.  
The project focuses on replicating and analyzing **knowledge distillation** techniques in machine learning for classifying cracked pavement with high accuracy and computational efficiency.

> ⚠️ **Note:** The original source code and trained models are no longer available. This repository serves as a **research and methodology archive** summarizing my work and findings.

---

## 🧠 Research Background

Pavement distress detection is crucial for maintaining safe transportation infrastructure.  
Traditional deep learning models such as **PicT**, **Swin Transformer**, and **EfficientNet-B3** have achieved strong accuracy in this domain. However, they often come at high computational costs.

VMamba introduces an innovative **visual state space model** that processes images with 74.5% fewer parameters than comparable transformers, enabling higher resolution analysis with lower compute requirements.

---

## ⚙️ Methodology

### Knowledge Distillation Setup
To explore the power of **teacher–student learning**, I designed a distillation framework using:
- **Teacher Model:** `EfficientNet-B7`  
- **Student Model:** `ResNet-50`  
- **Dataset:** *Pavement Dataset 2* (derived from ImageNet)  
- **Training Epochs:** 10  
- **Distillation Loss:** Combined cross-entropy and feature-based transfer loss

### Results
After 10 epochs, the distilled student model achieved:
> 🎯 **Top-1 Accuracy:** ~82%

This demonstrates that distillation learning is an effective technique for simplifying complex pavement distress models while maintaining robust accuracy.

---

## 🧩 Key Models Referenced
| Model | Description | Reference |
|--------|--------------|------------|
| **PicT** | Weakly supervised Vision Transformer for pavement distress | Zhang et al., 2022 |
| **Swin Transformer** | Hierarchical transformer with shifted windows | Liu et al., 2021 |
| **EfficientNet-B7** | Efficiently scaled CNN architecture | Tan & Le, 2019 |
| **VMamba** | Visual state space model with low parameter count | Liu et al., 2024 |

---

## 📈 Findings
- VMamba architecture provides **high efficiency** and **state-of-the-art accuracy** for vision tasks.  
- **Distillation learning** significantly reduces computational cost without severe loss in performance.  
- Combining these two ideas shows strong promise for **real-world road condition monitoring** systems.

---

## 📄 References
This project cites several key works in computer vision and knowledge distillation, including:
- PicT (Zhang et al., 2022)
- Swin Transformer (Liu et al., 2021)
- EfficientNet (Tan & Le, 2019)
- VMamba (Liu et al., 2024)
- Knowledge Distillation Review (Wang & Yoon, 2022)

Full reference list is available in the [📄 Research Paper PDF](./Pavement%20final%20paper%20(1).pdf).

---

## 💬 Acknowledgments
Special thanks to the **AI4Business Research Lab at San Diego State University** for providing resources and mentorship during this project.

---

> *“By teaching small models to think like big ones, we pave the way for smarter, faster, and safer roads.”*
