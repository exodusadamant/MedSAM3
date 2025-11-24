# MedSAM3
MedSAM3: Delving into Segment Anything with Medical Concepts

<div align="center">

[![Paper](https://img.shields.io/badge/Paper-arXiv-red)](your-arxiv-link)
[![Code](https://img.shields.io/badge/Code-GitHub-green)](https://github.com/Joey-SLiu/MedSAM3)
[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)

</div>

## 📋 Overview

MedSAM-3 is a text-promptable medical segmentation foundation model that enables **Promptable Concept Segmentation (PCS)** across diverse medical imaging modalities. By fine-tuning SAM 3 architecture on medical images with semantic conceptual labels, MedSAM-3 allows precise targeting of anatomical structures via open-vocabulary text descriptions.

### Key Features

- 🔤 **Text-Driven Segmentation**: Segment medical images using natural language descriptions (e.g., "pulmonary artery", "breast tumor")
- 🎯 **Multi-Modal Support**: Works across X-ray, MRI, Ultrasound, CT, OCT, Fundus, Dermoscopy, Histopathology, and video
- 🤖 **MedSAM-3 Agent**: Integrates MLLMs for complex reasoning and iterative refinement
- 📈 **SOTA Performance**: Outperforms existing specialist and foundation models

## 🎬 Demo

<!-- 建议在这里放一张概览图，展示多模态分割效果 -->
<div align="center">
  <img src="assets/overview.png" alt="MedSAM-3 Overview" width="800"/>
  <p><i>Concept-driven medical image segmentation across multiple modalities</i></p>
</div>

<!-- 可以添加一个动图展示交互式分割 -->
<!-- <img src="assets/demo.gif" alt="Interactive Segmentation" width="600"/> -->

## 🏗️ Architecture

<div align="center">
  <img src="assets/architecture.png" alt="MedSAM-3 Architecture" width="700"/>
</div>

MedSAM-3 features a dual encoder-decoder transformer design with:
- **Detector**: For image-level capabilities
- **Tracker**: With memory module for video tasks
- **Text & Image Encoders**: For aligned vision-language inputs

## 🚀 Installation
```bash
