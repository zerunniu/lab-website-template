---
title: WaSeCom – Wasserstein Distributionally Robust Wireless Semantic Communication with Large AI Models
description: A research project on enhancing the robustness of wireless semantic communication using large AI models and Wasserstein distributionally robust optimization
layout: project
permalink: /semcom/
group: featured
image: images/research.jpg
tags:
  - semantic communication
  - large AI models
  - wireless communication
  - distributionally robust optimization
  - uncertainty
  - robustness
authors:
  - Long Tan Le
  - Senura Hansaja Wanasekara
  - Zerun Niu
  - Yansong Shi
  - Nguyen H. Tran, Senior Member, IEEE
  - Phuong Vo
  - Walid Saad, Fellow, IEEE
  - Dusit Niyato, Fellow, IEEE
  - Zhu Han, Fellow, IEEE
  - Choong Seon Hong, Fellow, IEEE
  - H. Vincent Poor, Life Fellow, IEEE
published: true
---

# WaSeCom – Wasserstein Distributionally Robust Wireless Semantic Communication with Large AI Models

**WaSeCom** is a novel, model-agnostic framework that enhances the reliability and adaptability of wireless semantic communication (SemCom) systems against both **semantic-level** and **channel-level** uncertainties. Leveraging **large AI models** and **Wasserstein distributionally robust optimization (WDRO)**, WaSeCom ensures that semantic fidelity is preserved even under adversarial perturbations, distributional shifts, and challenging wireless channel conditions.

## ✍️ Authors
- **Long Tan Le**  
- **Senura Hansaja Wanasekara**  
- **Zerun Niu**  
- **Yansong Shi**  
- **Nguyen H. Tran**, Senior Member, IEEE  
- **Phuong Vo**  
- **Walid Saad**, Fellow, IEEE  
- **Dusit Niyato**, Fellow, IEEE  
- **Zhu Han**, Fellow, IEEE  
- **Choong Seon Hong**, Fellow, IEEE  
- **H. Vincent Poor**, Life Fellow, IEEE  

{% include alert.html type="info" content="🚀 **Project Status**: Active research with peer-reviewed publications and experimental validation across multiple modalities." %}

{% include section.html %}

## 🎯 Research Focus

This project addresses core challenges in next-generation semantic communication:

- **Robust Semantic Encoding & Decoding**: Extracting and reconstructing meaning with resilience to semantic noise, adversarial perturbations, and input distribution shifts.
- **Robust Channel Encoding & Decoding**: Ensuring reliable transmission under unpredictable wireless channel variations (AWGN, Rayleigh fading, interference).
- **Bi-level WDRO Framework**: Formulating robustness at both semantic and physical layers through Wasserstein ambiguity sets.
- **Model-Agnostic Integration**: Applying the framework to large AI architectures such as BERT, Vision Transformers, and multimodal encoders.

{% include section.html %}

## 🔬 Research Methodology

### 1. Semantic Communication with Large AI Models
- Uses **transformer-based encoders** (e.g., BERT, ViT, wav2vec) to produce compact semantic representations.
- Supports multiple modalities — text, images, audio, video — without modality-specific constraints.

### 2. Bi-level WDRO Optimization
- **Inner Level**: Optimizes semantic encoder/decoder for worst-case input shifts within a semantic Wasserstein ball.
- **Outer Level**: Optimizes channel encoder/decoder for worst-case channel perturbations.
- Decouples semantic robustness from channel robustness for better generalization.

### 3. Dual Reformulation & Efficient Training
- Employs **Kantorovich duality** to transform intractable min–max problems into scalable saddle-point optimizations.
- Uses **log-sum-exp smoothing** to make worst-case optimization differentiable and compatible with deep learning.

{% include section.html %}

## 📚 Key Contributions

- **WaSeCom Framework**: First WDRO-based bi-level optimization for wireless semantic communication.
- **Formal Robustness Guarantees**: Theoretical generalization bounds for both semantic and channel levels under distributional shifts.
- **Model-Agnostic Design**: Applicable to various large AI model architectures and modalities.
- **Dual Robustness**: Simultaneously addresses semantic and physical-layer uncertainties.
- **Empirical Validation**: Outperforms state-of-the-art baselines in image and text SemCom tasks under both clean and noisy conditions.

{% include citation.html lookup="Distributionally Robust Wireless Semantic Communication with Large AI Models" style="rich" show_image=false %}

{% include section.html %}

## 📊 Experimental Highlights

- **Datasets**: CIFAR-10 (images) & Europarl (multilingual text).
- **Channels**: AWGN and Rayleigh fading, across wide SNR ranges.
- **Baselines**: Compared with DeepJSCC, DeepSC, and DeepSC-RI.
- **Results**:
  - Maintains high PSNR/SSIM for images under FGSM noise and channel fading.
  - Achieves consistently higher BLEU scores in text transmission, especially under adversarial and low-SNR conditions.
  - Demonstrates minimal performance loss in clean conditions while substantially improving robustness in noisy scenarios.

{% include section.html %}

## 🏆 Research Impact

The WaSeCom framework benefits:

- **6G and Beyond**: Supports efficient, robust semantic-aware communication in next-gen wireless networks.
- **Mission-Critical Applications**: Ensures reliable meaning transmission in autonomous driving, remote surgery, and industrial automation.
- **AI-Powered Systems**: Enhances generalization across tasks and modalities for AI-driven communication.
- **Bandwidth Optimization**: Reduces unnecessary data transmission by focusing on task-relevant semantics.

{% include section.html %}

## 👥 Research Team

Collaboration between researchers from:
- **University of Sydney**
- **Kyung Hee University**
- **Virginia Tech**
- **Nanyang Technological University**
- **University of Houston**
- **Princeton University**

{% include section.html %}

## 📧 Contact

For more information about WaSeCom, please contact the **DUAL research group** or the project leads.
