
# README.md

## 📌 项目简介 | Project Introduction

**中文：** 本项目针对高反光、低纹理的柔性物体（如透明塑料袋）抓取难题，提出了一套结合视觉增强与多阶段协作的机器人抓取框架 。通过“展开-抓取”的精准阶段转换，显著提升了服务机器人在复杂环境下的操作稳定性 。

**English:** This project addresses the challenge of grasping reflective, low-texture flexible objects (e.g., plastic bags) by proposing a framework that combines visual enhancement and multi-stage collaboration. By enabling accurate "unfolding-grasping" transitions, it significantly improves the stability of service robots in complex scenarios.

---

## 🎥 演示视频 | Demo Video

### 视频简述 | Video Description


**中文：** 视频展示了双臂协作系统如何先通过模仿学习算法展开反光的黄色塑料袋 ，随后触发阶段转换机制 ，利用视觉增强算法（Canny 边缘检测、形态学闭运算等）精准定位并完成抓取 。
  
**English:** The video demonstrates how the dual-arm system first unfolds a reflective yellow plastic bag using imitation learning , then triggers the phase transition mechanism to accurately locate and grasp the object using visual enhancement algorithms (Canny edge detection, morphological closing, etc.).
根据您提供的视频素材内容，我为您优化了 GitHub 仓库的 **README.md** 结构。我将视频描述分为五个部分，以便访问者能够清晰地理解您论文中的核心贡献，特别是**多阶段协作框架** 和**视觉增强算法**的有效性 。

---

## 🎥 演示视频 | Demo Video

[在这里拖拽上传您的视频文件]

### 视频章节说明 | Video Chapters

1. **阶段 1 与阶段 2 转换 (Phase Transition between Stage 1 & 2)**
**中文：** 展示了系统如何通过实时监测机械臂关节角度（精度 ），在完成袋子展开后自动触发从模仿学习到视觉伺服抓取的平滑转换 。
**English:** Demonstrates the smooth transition from Stage 1 (imitation learning) to Stage 2 (visual servoing) triggered by real-time joint angle monitoring with  accuracy.

https://github.com/user-attachments/assets/69d3a051-84e8-462a-a789-3946e666350d

https://github.com/user-attachments/assets/8f990473-794e-4285-8830-a99c92ead5f1

https://github.com/user-attachments/assets/f9e5c091-d8fa-4fea-9f2c-61677d207b16



3. **全流程演示 (Full Task: From Unfolding to Placement)**
**中文：** 演示了从双臂协作展开反光塑料袋到最终精准放入物品（如泰迪熊）的完整闭环控制过程 。
**English:** Illustrates the complete closed-loop control from dual-arm unfolding of reflective bags to the precise placement of objects (e.g., a teddy bear).

https://github.com/user-attachments/assets/af45aed8-5e69-463d-8f5b-8f0b0d240590



5. **多样化颜色适配 (Color Generalization)**
**中文：** 验证了视觉增强算法对不同颜色、高反光柔性物体的稳健性，通过参数优化显著抑制了光影干扰 。
**English:** Validates the robustness of visual enhancement algorithms across different colors and highly reflective flexible objects by suppressing lighting interference.

https://github.com/user-attachments/assets/e1748f5d-90e4-4696-8075-e0af6c7c4764

https://github.com/user-attachments/assets/f99730ad-c81a-4c68-baa6-01464b582d3d



7. **通用性测试：刚性物体抓取 (Generalization: Rigid Object Grasping)**
**中文：** 证明了该框架在处理非结构化柔性物体的同时，同样具备对普通刚性物体的稳定抓取能力 。
**English:** Demonstrates that the framework maintains stable grasping capabilities for rigid objects while excelling at unstructured flexible object manipulation.

https://github.com/user-attachments/assets/deb15ee3-3496-4c6b-a028-7a19e1695124



9. **数据采集过程 (Data Collection & Training)**
**中文：** 展示了用于训练 Transformer 行为克隆模型的专家演示数据采集过程，为模仿学习提供高质量输入 。
**English:** Shows the expert demonstration data collection process used to train the Transformer-based behavioral cloning model.

https://github.com/user-attachments/assets/b6c3feca-4183-4a53-904e-61421c79edec



---

## 🚀 核心亮点 | Key Contributions

**多阶段协作框架 (Multi-Stage Collaboration):** 将任务分解为基于模仿学习的“展开阶段”和基于视觉伺服的“抓取阶段” 。

**视觉增强流水线 (Visual Enhancement Pipeline):** 通过高斯平滑、对比度调整和形态学处理，将边缘检测准确率提升至 90% 以上 。

**精准转换机制 (Phase Transition):** 采用三级触发系统，实时监控机械臂关节数据 ( 精度)，确保各阶段无缝衔接 。

**性能提升 (Performance Boost):** 实验证明，本框架的抓取成功率达到 **83%**，较传统方法提升了 **35%** 。


---

## 🛠️ 系统构成 | System Setup

**机械臂 (Robots):** 2 × DOBOT Nova5 (6-DOF).

**传感器 (Sensors):** 4 × Intel RealSense D405 深度相机.

**末端执行器 (Gripper):** 3D 打印双指软胶抓取手.

**控制算法 (Algorithms):** Transformer-based Behavioral Cloning & YOLO v8.

---

## 📖 引用 | Citation

```bibtex
@article{aga2025research,
  title={Research On Flexible Object Grasping Method Based on Visual Enhancement and Multi-Stage Collaboration},
  author={Aga, Cila and Cao, Zhijun and Chi, Junchen and Liu, Jin and Wang, Chaoqun and Fu, Tianyu and Song, Rui},
  journal={Procedia Computer Science},
  volume={271},
  pages={7--13},
  year={2025}
}

```

