# Attached-videos-demo-of-my-publication-FlexGrasp-Visual-Collaboration
中文： 基于视觉增强与多阶段协作的柔性物体（如塑料袋）抓取框架。相比 Mobile ALOHA 成功率提升 35%。 English: A flexible object grasping framework (e.g., plastic bags) combining visual enhancement and multi-stage collaboration. Improves success rate by 35% over Mobile ALOHA.
# Research On Flexible Object Grasping Method Based on Visual Enhancement and Multi-Stage Collaboration
# 基于视觉增强与多阶段协作的柔性物体抓取研究

[![License](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)
[![Venue](https://img.shields.io/badge/Venue-ICBIR%202025-blue)](https://www.elsevier.com/locate/procedia)

[cite_start]This repository contains the implementation and demo for the paper: **"Research On Flexible Object Grasping Method Based on Visual Enhancement and Multi-Stage Collaboration"**, published in *Procedia Computer Science 271 (2025) 7-13*[cite: 5, 9, 10].

---

## 🎥 Demo Video / 演示视频

[Drop your demo video file here]

> [cite_start]**Highlights:** The video demonstrates the transition from **Stage 1 (Unfolding)** using imitation learning to **Stage 2 (Grasping)** using visual localization[cite: 81, 82, 83].

---

## ✨ Key Features / 核心功能

* [cite_start]**Visual Enhancement Pipeline / 视觉增强流水线:** * Addresses challenges of reflective, low-texture flexible objects[cite: 14].
    * [cite_start]Includes contrast adjustment, Gaussian smoothing, Canny edge detection, and morphological operations[cite: 112, 125].
    * [cite_start]Maintains over 90% edge detection accuracy[cite: 131].
* **Multi-Stage Collaboration / 多阶段协作:**
    * [cite_start]**Stage 1:** Transformer-based behavioral cloning for stable unfolding[cite: 82].
    * [cite_start]**Stage 2:** YOLO v8-based detection and 3D coordinate mapping for precise grasping[cite: 83, 98].
* **Phase Transition Mechanism / 阶段转换机制:**
    * [cite_start]A three-level trigger system based on real-time joint angle data ($\pm0.01rad$ accuracy)[cite: 84, 85].
    * [cite_start]Ensures accurate "unfolding-to-grasping" transitions[cite: 15].

---

## 📊 Performance / 实验表现

[cite_start]Compared to the traditional Mobile ALOHA framework, our method significantly improves the success rate in handling transparent plastic bags[cite: 16, 160]:

| Method | Success Rate | 95% CI |
| :--- | :---: | :---: |
| [cite_start]Mobile ALOHA [cite: 173] | 48% | ±9.8% |
| [cite_start]**Proposed Framework [cite: 173]** | **83%** | **±7.37%** |

---

## 🛠️ System Setup / 系统设置

* [cite_start]**Robots:** 2 × 6-DOF DOBOT Nova5 robotic arms[cite: 153].
* [cite_start]**Sensors:** 4 × Intel RealSense D405 cameras[cite: 154].
* [cite_start]**Grippers:** 3D-printed two-finger soft rubber grippers[cite: 117, 153].
* [cite_start]**Base:** EPP foam anti-vibration base[cite: 122, 153].

---

## 📝 Citation / 引用

If you find this work helpful, please cite our paper:

```bibtex
@article{aga2025research,
  title={Research On Flexible Object Grasping Method Based on Visual Enhancement and Multi-Stage Collaboration},
  author={Aga, Cila and Cao, Zhijun and Chi, Junchen and Liu, Jin and Wang, Chaoqun and Fu, Tianyu and Song, Rui},
  journal={Procedia Computer Science},
  volume={271},
  pages={7--13},
  year={2025},
  publisher={Elsevier}
}
