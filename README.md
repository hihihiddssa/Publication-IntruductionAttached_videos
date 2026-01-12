README.md
📌 项目简介 | Project Introduction

中文： 本项目针对高反光、低纹理的柔性物体（如透明塑料袋）抓取难题，提出了一套结合视觉增强与多阶段协作的机器人抓取框架 。通过“展开-抓取”的精准阶段转换，显著提升了服务机器人在复杂环境下的操作稳定性 。

English: This project addresses the challenge of grasping reflective, low-texture flexible objects (e.g., plastic bags) by proposing a framework that combines visual enhancement and multi-stage collaboration. By enabling accurate "unfolding-grasping" transitions, it significantly improves the stability of service robots in complex scenarios.

🎥 演示视频 | Demo Video
视频简述 | Video Description

    中文： 视频展示了双臂协作系统如何先通过模仿学习算法展开反光的黄色塑料袋 ，随后触发阶段转换机制 ，利用视觉增强算法（Canny 边缘检测、形态学闭运算等）精准定位并完成抓取 。

English: The video demonstrates how the dual-arm system first unfolds a reflective yellow plastic bag using imitation learning , then triggers the phase transition mechanism to accurately locate and grasp the object using visual enhancement algorithms (Canny edge detection, morphological closing, etc.).

🚀 核心亮点 | Key Contributions

    多阶段协作框架 (Multi-Stage Collaboration): 将任务分解为基于模仿学习的“展开阶段”和基于视觉伺服的“抓取阶段” 。

视觉增强流水线 (Visual Enhancement Pipeline): 通过高斯平滑、对比度调整和形态学处理，将边缘检测准确率提升至 90% 以上 。

精准转换机制 (Phase Transition): 采用三级触发系统，实时监控机械臂关节数据 (±0.01rad 精度)，确保各阶段无缝衔接 。

性能提升 (Performance Boost): 实验证明，本框架的抓取成功率达到 83%，较传统方法提升了 35% 。

🛠️ 系统构成 | System Setup

    机械臂 (Robots): 2 × DOBOT Nova5 (6-DOF).

传感器 (Sensors): 4 × Intel RealSense D405 深度相机.

末端执行器 (Gripper): 3D 打印双指软胶抓取手.

控制算法 (Algorithms): Transformer-based Behavioral Cloning & YOLO v8.
