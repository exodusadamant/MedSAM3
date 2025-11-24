# MedSAM3
MedSAM3: Delving into Segment Anything with Medical Concepts

**🚧 Code, model, paper, and guides will be released progressively! 🚧**

## Overview
MedSAM-3 is a text-promptable medical segmentation foundation model that enables **Promptable Concept Segmentation (PCS)** across diverse medical imaging modalities (X-ray, MRI, Ultrasound, CT, OCT, Fundus, Dermoscopy, Histopathology, and video).

### Key Features
- 🔤 **Text-Driven Segmentation**: Segment using natural language (e.g., "breast tumor", "pulmonary artery")
- 🎯 **Multi-Modal Support**: Works across diverse medical imaging modalities
- 🤖 **MedSAM-3 Agent**: Integrates MLLMs for complex reasoning
- 📈 **SOTA Performance**: Outperforms existing models

## Overview
<div align="center">
  <img src="assets/overview.png" alt="MedSAM-3 Overview" width="800"/>
  <p><i>Concept-driven medical segmentation across multiple modalities</i></p>
</div>

## Architecture
<div align="center">
  <img src="assets/architecture.png" alt="MedSAM-3 Architecture" width="700"/>
</div>

## MedSAM-3 Agent
<div align="center">
  <img src="assets/agent.png" alt="MedSAM-3 Architecture" width="400"/>
</div>

## Performance
| Dataset | U-Net | MedSAM | SAM 3 | **MedSAM-3** |
|---------|-------|--------|-------|--------------|
| BUSI | 0.7618 | 0.7514 | 0.7110 | **0.7772** |
| RIM-ONE | 0.8480 | 0.8479 | 0.8303 | **0.8977** |
| ISIC 2018 | 0.8760 | **0.9177** | 0.8178 | 0.9058 |
| Kvasir-SEG | 0.8244 | 0.7657 | 0.7671 | **0.8831** |

## TODO List
- [ ] Release paper on arXiv
- [ ] Release MedSAM-3 model weights
- [ ] Release training code
- [ ] Release inference code
- [ ] Provide inference demo (Gradio/Colab)
- [ ] Release evaluation scripts
- [ ] Publish comprehensive documentation
- [ ] Create tutorial notebooks
- [ ] Expand to more medical imaging modalities
- [ ] Release MedSAM-3 Agent code

## Tips and Future Directions
We are continuously working to improve MedSAM-3:
- 📊 **Scaling Up**: We are progressively expanding the training data scale to cover more medical concepts and imaging modalities
- 🔧 **Method Updates**: The model architecture and training strategies will be iteratively refined based on community feedback and new research findings
- 🌐 **Towards Universal Medical Segmentation**: Our ultimate goal is to develop a universal medical image segmentation foundation model that can handle any anatomical structure or pathological finding across all medical imaging modalities

## Discussion: SAM 3 Limitations on Medical Data
While SAM 3 shows impressive performance on natural images, we observed several failure cases on medical imaging data:

<div align="center">
  <img src="assets/sam3_failures.png" alt="SAM 3 Failure Cases" width="800"/>
</div>

**Example Failure Cases:**

1. **Low-Contrast Structures**: SAM 3 struggles with low-contrast anatomical structures common in medical images (e.g., soft tissue boundaries in ultrasound, subtle lesions in X-ray)

2. **Domain-Specific Concepts**: The model fails to understand medical-specific concepts without specialized training (e.g., differentiating between benign and malignant tumors, identifying specific pathological patterns)

3. **Small Object Segmentation**: Fine-grained structures such as small lesions, blood vessels, or cellular structures are often missed or poorly segmented

4. **Multi-Modal Adaptation**: SAM 3 shows inconsistent performance across different medical imaging modalities, particularly struggling with modalities that differ significantly from natural images (e.g., OCT, histopathology)

5. **Ambiguous Boundaries**: Medical images often contain ambiguous or fuzzy boundaries that require domain expertise, which general-purpose models like SAM 3 cannot handle effectively

These limitations motivate the development of MedSAM-3, which incorporates medical domain knowledge and is specifically trained on diverse medical imaging data.

## Coming Soon
- 📄 Paper
- 💻 Code
- 💾 Model weights
- 📦 Installation guide
- 📚 Documentation

## Contact
For questions, please contact:
- Jintai Chen: jintaiCHEN@hkust-gz.edu.cn
- Xu Cao: xucao2@illinois.edu

---
<div align="center">
Made with ❤️ by the MedSAM-3 Team
</div>
