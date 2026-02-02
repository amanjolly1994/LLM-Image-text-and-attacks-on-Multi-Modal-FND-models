# LLM-Image-text-and-attacks-on-Multi-Modal-FND-models

# A Rigorous Interrogation of Multimodal Fake News Detection Paradigms: Adversarial Robustness and Modality Dependence

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Paper](https://img.shields.io/badge/Paper-Cluster%20Computing-blue)](https://link.to.your.paper.if.available)

This repository contains the official source code and experimental pipeline for the paper **"A Rigorous Interrogation of Multimodal Fake News Detection Paradigms: Adversarial Robustness and Modality Dependence"**, published in *Cluster Computing*.

## 📄 Abstract
This work presents a comprehensive evaluation of canonical and modern Multimodal Fake News Detection (MFND) architectures. We assess the feasibility and robustness of five diverse architectures (**LongBERT-VGG, CNN-VGG, LSTM-VGG, BERT-CLIP, and ViLBERT**) across three benchmark datasets (**D1, RECOVERY, and PolitiFact**). Our analysis subjects these models to an extensive battery of **17 adversarial perturbations**, including 10 image-based attacks and 7 text-based attacks. Crucially, we introduce novel adversarial textual manipulations generated via instruction-tuned **Llama 3 8B** and **DeepSeek-LLM 7B Chat** models.

## 🚀 Key Features
* [cite_start]**5 Architectures Implemented:** Standard VGG-based late fusion models (with LongBERT/CNN/LSTM) and modern baselines (BERT-CLIP, End-to-End ViLBERT)[cite: 8].
* **17 Adversarial Attacks:**
    * [cite_start]**Image:** FGSM, PGD (L2/Linf), MIFGSM, NIFGSM, DIFGSM, Pixle, etc.[cite: 9].
    * **Text:** TextFooler, TextBugger, HotFlip.
    * [cite_start]**LLM-Generated:** Novel Semantic and Grammar attacks using fine-tuned **Llama 3** and **DeepSeek**[cite: 10].
* **Advanced Analysis:**
    * [cite_start]**Modality Ablation:** Scripts to test model reliance on text-only vs. image-only inputs[cite: 12].
    * [cite_start]**Black-Box Transferability:** Evaluation of attack transfer between different architectures[cite: 11].
    * [cite_start]**Explainability:** Grad-CAM visualization scripts to diagnose failure modes (e.g., artifact reliance)[cite: 18].

## 📂 Repository Structure