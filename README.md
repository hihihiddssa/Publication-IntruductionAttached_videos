# Research On Flexible Object Grasping Method Based on Visual Enhancement and Multi-Stage Collaboration
# 基于视觉增强与多阶段协作的柔性物体抓取研究

## 📌 项目简介 | Project Introduction

**🇨🇳 中文** 本项目针对高反光、低纹理的柔性物体（如透明塑料袋）抓取难题，提出了一套结合 **视觉增强 (Visual Enhancement)** 与 **多阶段协作 (Multi-Stage Collaboration)** 的机器人抓取框架。通过“展开-抓取”的精准阶段转换，显著提升了服务机器人在复杂环境下的操作稳定性。

**🇬🇧 English** This project addresses the challenge of grasping reflective, low-texture flexible objects (e.g., plastic bags) by proposing a framework that combines **Visual Enhancement** and **Multi-Stage Collaboration**. By enabling accurate "unfolding-grasping" transitions, it significantly improves the stability of service robots in complex scenarios.

---

## 🚀 核心亮点 | Key Contributions

| 模块 / Module | 描述 / Description |
| :--- | :--- |
| **多阶段协作框架**<br>Multi-Stage Collaboration | **CN:** 将任务分解为基于模仿学习的“展开阶段”和基于视觉伺服的“抓取阶段”。<br>**EN:** Decomposes the task into an imitation learning-based "Unfolding Stage" and a visual servoing-based "Grasping Stage". |
| **视觉增强流水线**<br>Visual Enhancement Pipeline | **CN:** 通过高斯平滑、对比度调整和形态学处理，将边缘检测准确率提升至 **90%** 以上。<br>**EN:** Improves edge detection accuracy to over **90%** via Gaussian smoothing, contrast adjustment, and morphological processing. |
| **精准转换机制**<br>Phase Transition | **CN:** 采用三级触发系统，实时监控机械臂关节数据，确保各阶段无缝衔接。<br>**EN:** Adopts a three-level trigger system monitoring joint data in real-time to ensure seamless transitions. |
| **性能提升**<br>Performance Boost | **CN:** 实验证明，本框架的抓取成功率达到 **83%**，较传统方法提升了 **35%**。<br>**EN:** Experiments show a grasping success rate of **83%**, a **35%** improvement over traditional methods. |

---

## 🎥 演示视频 | Demo Video

> **Note:** 以下视频展示了从展开到抓取的完整流程及算法的鲁棒性测试。
> The following videos demonstrate the full process from unfolding to grasping and robustness tests.

### 1. 阶段 1 与阶段 2 转换 (Phase Transition)
**CN:** 展示了系统通过实时监测机械臂关节角度（高精度），在完成袋子展开后自动触发从“模仿学习”到“视觉伺服抓取”的平滑转换。  
**EN:** Demonstrates the smooth transition from Stage 1 (imitation learning) to Stage 2 (visual servoing) triggered by real-time joint angle monitoring with high precision.

https://github.com/user-attachments/assets/4603b509-eaeb-4aa5-a8ca-4bf48f7e3d74

https://github.com/user-attachments/assets/dd9c6639-5c8a-4a28-a563-27a95cc84f63

https://github.com/user-attachments/assets/b4c0b1f5-3735-443a-9ce6-d556ef0892df

### 2. 全流程演示 (Full Task: From Unfolding to Placement)
**CN:** 演示了从双臂协作展开反光塑料袋到最终精准放入物品（如泰迪熊）的完整闭环控制过程。  
**EN:** Illustrates the complete closed-loop control from dual-arm unfolding of reflective bags to the precise placement of objects (e.g., a teddy bear).

https://github.com/user-attachments/assets/84d46608-2374-4f60-b5bf-87ac89c7346e

### 3. 多样化颜色适配 (Color Generalization)
**CN:** 验证了视觉增强算法对不同颜色、高反光柔性物体的稳健性，通过参数优化显著抑制了光影干扰。  
**EN:** Validates the robustness of visual enhancement algorithms across different colors and highly reflective flexible objects by suppressing lighting interference.

https://github.com/user-attachments/assets/7d8bd20f-4a2c-40ec-834e-5635cf33dba4

https://github.com/user-attachments/assets/3c84b179-5823-441b-bf56-33200c4242fa

### 4. 通用性测试：刚性物体抓取 (Generalization: Rigid Object)
**CN:** 证明了该框架在处理非结构化柔性物体的同时，同样具备对普通刚性物体的稳定抓取能力。  
**EN:** Demonstrates that the framework maintains stable grasping capabilities for rigid objects while excelling at unstructured flexible object manipulation.

https://github.com/user-attachments/assets/134cfb46-261f-4229-b06f-ba3fa7a28b49

### 5. 数据采集过程 (Data Collection & Training)
**CN:** 展示了用于训练 Transformer 行为克隆模型的专家演示数据采集过程，为模仿学习提供高质量输入。  
**EN:** Shows the expert demonstration data collection process used to train the Transformer-based behavioral cloning model.

https://github.com/user-attachments/assets/c1db5af7-147a-4636-ae44-fd71ac63577b

---

## 🛠️ 系统构成 | System Setup

| 组件 / Component | 规格 / Specification |
| :--- | :--- |
| **机械臂** (Robots) | 2 × DOBOT Nova5 (6-DOF) |
| **传感器** (Sensors) | 4 × Intel RealSense D405 Depth Cameras |
| **末端执行器** (Gripper) | Custom 3D-printed dual-finger soft gripper (3D 打印双指软胶抓取手) |
| **控制算法** (Algorithms)| Transformer-based Behavioral Cloning & YOLO v8 |

---

## 📖 引用 | Citation

If you find this work helpful, please consider citing:

```bibtex
@article{aga2025research,
  title={Research On Flexible Object Grasping Method Based on Visual Enhancement and Multi-Stage Collaboration},
  author={Aga, Cila and Cao, Zhijun and Chi, Junchen and Liu, Jin and Wang, Chaoqun and Fu, Tianyu and Song, Rui},
  journal={Procedia Computer Science},
  volume={271},
  pages={7--13},
  year={2025}
}
