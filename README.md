# LEG-SLAM: Real-Time Language-Enhanced Gaussian Splatting for SLAM

![Graphical Abstract](https://github.com/user-attachments/assets/a3b034b9-96ea-4695-b42a-59785103993a)

## Overview

LEG-SLAM is an **open-vocabulary** 3D SLAM system that integrates **3D Gaussian Splatting**, **DINOv2 feature extraction**, and **Talk2DINO language grounding** to enable real-time **semantic 3D scene understanding**. Unlike existing methods, LEG-SLAM allows **text-driven** interactive exploration of reconstructed environments **without predefined object categories**.

### 🔹 Key Features:
- **Real-time 3D Reconstruction:** High-fidelity scene reconstruction with **Gaussian Splatting**.
- **Open-Vocabulary Understanding:** Uses **DINOv2** features and **Talk2DINO** to match text queries to visual features.
- **Efficient Feature Compression:** **PCA-based embedding compression** enables low-latency inference.
- **Interactive Scene Queries:** Retrieve **semantic masks** in real-time by specifying objects via text.
- **High-Speed Performance:** Achieves **10 FPS** on **Replica** and **18 FPS** on **ScanNet**, significantly faster than prior methods.

## 🔬 Methodology

1. **DINOv2 Feature Extraction**: Extracts rich, self-supervised embeddings from RGB frames.
2. **Talk2DINO Language Alignment**: Transforms **text queries** into DINOv2-compatible feature space.
3. **PCA Compression**: Reduces embeddings from **768D → 64D**, enabling real-time processing.
4. **3D Gaussian Splatting**: Constructs a continuous, high-resolution 3D scene representation.
5. **Semantic Querying**: Computes **cosine similarity** between scene embeddings and textual queries, generating **semantic heatmaps**.

## 📜 Paper

If you find this work useful, please cite:

```bibtex
@article{LEG-SLAM,
  title={LEG-SLAM: Open-Vocabulary 3D Gaussian Splatting for SLAM},
  author={Anonymous Authors},
  journal={Under Review at ICCV 2025},
  year={2025}
}
```
## ⏳ Code Availability

🔹 Code will be released upon paper acceptance. Stay tuned for updates! 🚀
