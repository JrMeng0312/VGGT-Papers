# VGGT & Feed-Forward 3D Reconstruction Papers

[![更新日志](https://img.shields.io/badge/💡-更新日志-informational.svg?style=flat)](Changelog.md)
[![发现错误](https://img.shields.io/badge/🐛-发现错误-yellow.svg?style=flat)](https://github.com/JrMeng0312/VGGT-Papers/issues)
[![提交修改](https://img.shields.io/badge/👐-提交修改-brightgreen.svg?style=flat)](https://github.com/JrMeng0312/VGGT-Papers/pulls)

> 收集 VGGT（Visual Geometry Grounded Transformer）及相关前馈式三维重建论文，持续更新，欢迎交流讨论。

---

#### **📚 会议期刊**

- **2024**

  - [[CVPR](./2024/CVPR.md)] (1 篇)
    [[ECCV](./2024/ECCV.md)] (1 篇)
    [[NeurIPS](./2024/NeurIPS.md)] (1 篇)
    [[Preprint](./2024/Preprint.md)] (2 篇)

- **2025**

  - [[CVPR](./2025/CVPR.md)] (3 篇)
    [[ICLR](./2025/ICLR.md)] (1 篇)
    [[Preprint](./2025/Preprint.md)] (11 篇)
    [[Other](./2025/Other.md)] (1 篇)

- **2026**

  - [[ICLR](./2026/ICLR.md)] (1 篇)
    [[Preprint](./2026/Preprint.md)] (9 篇)
    [[Other](./2026/Other.md)] (4 篇)

#### **📂 分类索引**

| 分类 | 说明 |
|------|------|
| [VGGT 核心](#vggt-核心) | VGGT 原始论文及官方扩展 |
| [VGGT 变体与加速](#vggt-变体与加速) | SwiftVGGT, FastVGGT, HD-VGGT, PanoVGGT, Faster VGGT, QuantVGGT 等 |
| [VGGT 应用](#vggt-应用) | VGGT-SLAM, DriveVGGT, VGGT-X, VGGT-World, VGGT-Det, GPA-VGGT 等 |
| [前馈式三维重建基础](#前馈式三维重建基础) | DUSt3R, MASt3R, CUT3R, Fast3R, Speed3R 等 |
| [单目几何估计](#单目几何估计) | MoGe, Depth Anything 3 等 |
| [综述](#综述) | 综述论文 |

#### **📖 Survey**

- [[Survey Papers](./Survey.md)] (1 篇)

---

## VGGT 核心

#### [1] VGGT: Visual Geometry Grounded Transformer
- **🧑‍🔬 作者**：Jianyuan Wang, Minghao Chen, Nikita Karaev, Andrea Vedaldi, Christian Rupprecht, David Novotny
- **🏫 单位**：Meta ⟐ University of Oxford
- **🔗 链接**：[[中英摘要](./abs/2503.11651.md)] [[arXiv:2503.11651](https://arxiv.org/abs/2503.11651)] [[Code](https://github.com/facebookresearch/vggt)]
- **📝 说明**：🏆 CVPR 2025 Best Paper Award

#### [2] VGG-T3: Offline Feed-Forward 3D Reconstruction at Scale
- **🧑‍🔬 作者**：Sven Elflein, Ruilong Li, Sérgio Agostinho, Zan Gojcic, Laura Leal-Taixé, Qunjie Zhou, Aljosa Osep
- **🏫 单位**：NVIDIA ⟐ Technical University of Munich
- **🔗 链接**：[[中英摘要](./abs/2602.23361.md)] [[arXiv:2602.23361](https://arxiv.org/abs/2602.23361)] [Code]
- **📝 说明**：VGGT 的可扩展离线重建版本，线性复杂度，处理 1000 张图像仅需 54 秒

---

## VGGT 变体与加速

#### [3] SwiftVGGT: A Scalable Visual Geometry Grounded Transformer for Large-Scale Scenes
- **🧑‍🔬 作者**：Jungho Lee, Minhyeok Lee, Sunghun Yang, Minseok Kang, Sangyoun Lee
- **🏫 单位**：Yonsei University
- **🔗 链接**：[[中英摘要](./abs/2511.18290.md)] [[arXiv:2511.18290](https://arxiv.org/abs/2511.18290)] [Code]
- **📝 说明**：免训练方法，仅需 33% 推理时间即可实现大规模场景重建

#### [4] FastVGGT: Training-Free Acceleration of Visual Geometry Transformer
- **🧑‍🔬 作者**：You Shen, Zhipeng Zhang, Yansong Qu, Xiawu Zheng, Jiayi Ji, Shengchuan Zhang, Liujuan Cao
- **🏫 单位**：Xiamen University
- **🔗 链接**：[[中英摘要](./abs/2509.02560.md)] [[arXiv:2509.02560](https://arxiv.org/abs/2509.02560)] [Code]
- **📝 说明**：3D Token Merging，1000 张图像输入 4 倍加速

#### [5] HD-VGGT: High-Resolution Visual Geometry Transformer
- **🧑‍🔬 作者**：Tianrun Chen, Yuanqi Hu, Yidong Han, Hanjie Xu, Deyi Ji, Qi Zhu, Chunan Yu, Xin Zhang, Cheng Chen, Chaotao Ding, Ying Zang, Xuanfu Li, Jin Ma, Lanyun Zhu
- **🏫 单位**：Zhejiang University of Technology ⟐ KOKONI3D
- **🔗 链接**：[[中英摘要](./abs/2603.27222.md)] [[arXiv:2603.27222](https://arxiv.org/abs/2603.27222)] [Code]
- **📝 说明**：双分支设计，低分辨率粗糙几何 + 高分辨率细节增强

#### [6] PanoVGGT: Feed-Forward 3D Reconstruction from Panoramic Imagery
- **🧑‍🔬 作者**：Yijing Guo, Mengjun Chao, Luo Wang, Tianyang Zhao, Haizhao Dai, Yingliang Zhang, Jingyi Yu, Yujiao Shi
- **🏫 单位**：ShanghaiTech University
- **🔗 链接**：[[中英摘要](./abs/2603.17571.md)] [[arXiv:2603.17571](https://arxiv.org/abs/2603.17571)] [Code]
- **📝 说明**：全景图像前馈式 3D 重建，球面感知位置编码

#### [7] Faster VGGT with Block-Sparse Global Attention
- **🧑‍🔬 作者**：Chung-Shien Brian Wang, Christian Schmidt, Jens Piekenbrinck, Bastian Leibe
- **🏫 单位**：RWTH Aachen University
- **🔗 链接**：[[中英摘要](./abs/2509.07120.md)] [[arXiv:2509.07120](https://arxiv.org/abs/2509.07120)] [Code]
- **📝 说明**：块稀疏注意力替换全局注意力，推理加速 4 倍，无需重训练

#### [8] QuantVGGT: Quantized Visual Geometry Grounded Transformer
- **🧑‍🔬 作者**：Weilun Feng, Haotong Qin, Mingqiang Wu, Chuanguang Yang, Yuqi Li, Xiangqi Li, Zhulin An, Libo Huang, Yulun Zhang, Michele Magno, Yongjun Xu
- **🏫 单位**：Chinese Academy of Sciences ⟐ ETH Zurich ⟐ Shanghai Jiao Tong University
- **🔗 链接**：[[中英摘要](./abs/2509.21302.md)] [[arXiv:2509.21302](https://arxiv.org/abs/2509.21302)] [[Code](https://github.com/wlfeng0509/QuantVGGT)]
- **📝 说明**：VGGT 首个后训练量化框架，4-bit 实现近无损压缩，内存降低 3.7 倍

---

## VGGT 应用

#### [9] VGGT-SLAM: Dense RGB SLAM Optimized on the SL(4) Manifold
- **🧑‍🔬 作者**：Dominic Maggio, Hyungtae Lim, Luca Carlone
- **🏫 单位**：MIT
- **🔗 链接**：[[中英摘要](./abs/2505.12549.md)] [[arXiv:2505.12549](https://arxiv.org/abs/2505.12549)] [Code]
- **📝 说明**：基于 VGGT 的稠密 SLAM，SL(4) 流形优化

#### [10] VGGT-SLAM 2.0: Real-time Dense Feed-forward Scene Reconstruction
- **🧑‍🔬 作者**：Dominic Maggio, Luca Carlone
- **🏫 单位**：MIT
- **🔗 链接**：[[中英摘要](./abs/2601.19887.md)] [[arXiv:2601.19887](https://arxiv.org/abs/2601.19887)] [Code]
- **📝 说明**：实时前馈 SLAM，位姿误差比 VGGT-SLAM 减少约 23%

#### [11] VGGT-SLAM++
- **🧑‍🔬 作者**：Avilasha Mandal, Rajesh Kumar, Sudarshan Sunil Harithas, Chetan Arora
- **🏫 单位**：IIT Delhi
- **🔗 链接**：[[中英摘要](./abs/2604.06830.md)] [[arXiv:2604.06830](https://arxiv.org/abs/2604.06830)] [Code]
- **📝 说明**：完整 VGGT 视觉 SLAM 系统，含 DEM 图模块与闭环检测

#### [12] PAGE-4D: Disentangled Pose and Geometry Estimation for VGGT-4D Perception
- **🧑‍🔬 作者**：Kaichen Zhou, Yuhan Wang, Grace Chen, Xinhai Chang, Gaspard Beaudouin, Fangneng Zhan, Paul Pu Liang, Mengyu Wang
- **🏫 单位**：MIT ⟐ CMU
- **🔗 链接**：[[中英摘要](./abs/2510.17568.md)] [[arXiv:2510.17568](https://arxiv.org/abs/2510.17568)] [Code]
- **📝 说明**：将 VGGT 扩展至动态场景，解耦位姿与几何估计

#### [13] DriveVGGT: Calibration-Constrained Visual Geometry Transformers for Multi-Camera Autonomous Driving
- **🧑‍🔬 作者**：Xiaosong Jia, Yanhao Liu, Yu Hong, Renqiu Xia, Junqi You, Bin Sun, Zhihui Hao, Junchi Yan
- **🏫 单位**：Shanghai Jiao Tong University
- **🔗 链接**：[[中英摘要](./abs/2511.22264.md)] [[arXiv:2511.22264](https://arxiv.org/abs/2511.22264)] [Code]
- **📝 说明**：面向自动驾驶多相机场景，推理时间减少 49.3%

#### [14] VGGT-X: When VGGT Meets Dense Novel View Synthesis
- **🧑‍🔬 作者**：Yang Liu, Chuanchen Luo, Zimo Tang, Junran Peng, Zhaoxiang Zhang
- **🏫 单位**：Chinese Academy of Sciences
- **🔗 链接**：[[中英摘要](./abs/2509.25191.md)] [[arXiv:2509.25191](https://arxiv.org/abs/2509.25191)] [Code]
- **📝 说明**：将 VGGT 扩展至稠密新视角合成，支持 1000+ 图像，无需 COLMAP

#### [15] Reloc-VGGT: Visual Re-localization with Geometry Grounded Transformer
- **🧑‍🔬 作者**：Tianchen Deng, Wenhua Wu, Kunzhen Wu, Guangming Wang, Siting Zhu, Shenghai Yuan, Xun Chen, Guole Shen, Zhe Liu, Hesheng Wang
- **🏫 单位**：Shanghai Jiao Tong University
- **🔗 链接**：[[中英摘要](./abs/2512.21883.md)] [[arXiv:2512.21883](https://arxiv.org/abs/2512.21883)] [Code]
- **📝 说明**：基于 VGGT 的视觉重定位，多视图早期融合 + 稀疏掩码注意力

#### [16] GPA-VGGT: Adapting VGGT to Large Scale Localization by Self-Supervised Learning with Geometry and Physics Aware Loss
- **🧑‍🔬 作者**：Yangfan Xu, Lilian Zhang, Xiaofeng He, Yugui Shen, Pengdong Wu, Wenqi Wu, Jun Mao
- **🏫 单位**：未标注
- **🔗 链接**：[[中英摘要](./abs/2601.16885.md)] [[arXiv:2601.16885](https://arxiv.org/abs/2601.16885)] [[Code](https://github.com/X-yangfan/GPA-VGGT)]
- **📝 说明**：自监督 VGGT 大规模定位，几何与物理感知联合优化

#### [17] VGGT-Det: Mining VGGT Internal Priors for Sensor-Geometry-Free Multi-View Indoor 3D Object Detection
- **🧑‍🔬 作者**：Yang Cao, Feize Wu, Dave Zhenyu Chen, Yingji Zhong, Lanqing Hong, Dan Xu
- **🏫 单位**：HKUST ⟐ Huawei Noah's Ark Lab
- **🔗 链接**：[[中英摘要](./abs/2603.00912.md)] [[arXiv:2603.00912](https://arxiv.org/abs/2603.00912)] [Code]
- **📝 说明**：无传感器几何的多视图室内 3D 目标检测，利用 VGGT 内部语义 + 几何先验

#### [18] VGGT-World: Transforming VGGT into an Autoregressive Geometry World Model
- **🧑‍🔬 作者**：Xiangyu Sun, Shijie Wang, Fengyi Zhang, Lin Liu, Caiyan Jia, Ziying Song, Zi Huang, Yadan Luo
- **🏫 单位**：Beijing Jiaotong University ⟐ University of Queensland
- **🔗 链接**：[[中英摘要](./abs/2603.12655.md)] [[arXiv:2603.12655](https://arxiv.org/abs/2603.12655)] [Code]
- **📝 说明**：将 VGGT 转化为自回归几何世界模型，速度快 3.6-5 倍，仅 0.43B 参数

#### [19] VGGT-Mapping: A Mapping System for Robot Navigation based on VGGT
- **🧑‍🔬 作者**：Shaofeng Tan, Xiaoguang Ma, Zixi Jia
- **🏫 单位**：未标注
- **🔗 链接**：[[DOI](https://doi.org/10.1109/irac67707.2025.11381128)]
- **📝 说明**：IEEE IRAC 2025 — 面向机器人导航的 VGGT 建图系统

#### [20] VGGT-Geo: Probabilistic Geometric Fusion of VGGT Priors for Robust Dense Indoor SLAM
- **🧑‍🔬 作者**：Kai Qin, Jing Li, Sisi Zlatanova, Haitao Wu, Hao Wu, Yin Gao, Dingjie Zhou, Yuchen Li, Sizhe Shen, Xiangjun Qu, Zhenxin Zhang, Banghui Yang, Shicheng Xu
- **🏫 单位**：Northwestern Polytechnical University
- **🔗 链接**：[[DOI](https://doi.org/10.3390/ijgi15020085)]
- **📝 说明**：ISPRS IJGI 2026 — 概率几何融合框架，轨迹精度提升约 50%

#### [21] OV3DSeg-VGGT: Open-Vocabulary 3D Segmentation with Visual Geometry-Grounded Transformers
- **🧑‍🔬 作者**：Jingke Zhou, Xianliang Huang, Yixin Ren, Dikai Fan, Shengyu Gu, Bin Tian, Xiao Liu, Tianjia Shao
- **🏫 单位**：Zhejiang University
- **🔗 链接**：[[DOI](https://doi.org/10.1016/j.visinf.2026.100311)]
- **📝 说明**：Visual Informatics 2026 — 基于 VGGT 的开放词汇 3D 分割

#### [22] Fast vision-based 3D reconstruction and damage detection based on VGGT
- **🧑‍🔬 作者**：Yumeng Chen, Xiao Pan, Haoyang Zhang, Yousufu Ma, Haoyu Zhang
- **🏫 单位**：未标注
- **🔗 链接**：[[DOI](https://doi.org/10.1016/j.jobe.2026.116066)]
- **📝 说明**：J. Building Engineering 2026 — VGGT 用于建筑结构快速 3D 重建与损伤检测

#### [23] Zero-shot text-to-3D-object generation with VGGT
- **🧑‍🔬 作者**：Dong-hun Lee, Sang-hyo Park
- **🏫 单位**：未标注
- **🔗 链接**：[[DOI](https://doi.org/10.1117/12.3102112)]
- **📝 说明**：SPIE IWAIT 2026 — 基于 VGGT 的零样本文本到 3D 物体生成

---

## 前馈式三维重建基础

#### [24] DUSt3R: Geometric 3D Vision Made Easy
- **🧑‍🔬 作者**：Shuzhe Wang, Vincent Leroy, Yohann Cabon, Boris Chidlovskii, Jerome Revaud
- **🏫 单位**：NAVER LABS Europe
- **🔗 链接**：[[中英摘要](./abs/2312.14132.md)] [[arXiv:2312.14132](https://arxiv.org/abs/2312.14132)] [[Code](https://github.com/naver/dust3r)]
- **📝 说明**：🏆 CVPR 2024 Oral — 开创性工作，将多视图重建转化为点图回归

#### [25] MASt3R: Grounding Image Matching in 3D
- **🧑‍🔬 作者**：Vincent Leroy, Yohann Cabon, Jérôme Revaud
- **🏫 单位**：NAVER LABS Europe
- **🔗 链接**：[[中英摘要](./abs/2406.09756.md)] [[arXiv:2406.09756](https://arxiv.org/abs/2406.09756)] [[Code](https://github.com/naver/mast3r)]
- **📝 说明**：🏆 ECCV 2024 — 在 DUSt3R 基础上增加密集局部特征匹配

#### [26] MASt3R-SfM: a Fully-Integrated Solution for Unconstrained Structure-from-Motion
- **🧑‍🔬 作者**：Bardienus Duisterhof, Lojze Zust, Philippe Weinzaepfel, Vincent Leroy, Yohann Cabon, Jerome Revaud
- **🏫 单位**：NAVER LABS Europe
- **🔗 链接**：[[中英摘要](./abs/2409.19152.md)] [[arXiv:2409.19152](https://arxiv.org/abs/2409.19152)] [[Code](https://github.com/naver/mast3r)]
- **📝 说明**：基于 MASt3R 的完整 SfM 方案，线性复杂度

#### [27] MUSt3R: Multi-view Network for Stereo 3D Reconstruction
- **🧑‍🔬 作者**：Yohann Cabon, Lucas Stoffl, Leonid Antsfeld, Gabriela Csurka, Boris Chidlovskii, Jerome Revaud, Vincent Leroy
- **🏫 单位**：NAVER LABS Europe
- **🔗 链接**：[[中英摘要](./abs/2503.01661.md)] [[arXiv:2503.01661](https://arxiv.org/abs/2503.01661)] [[Code](https://github.com/naver/must3r)]
- **📝 说明**：🏆 CVPR 2025 — 多视图同步处理，多层记忆机制

#### [28] CUT3R: Continuous 3D Perception Model with Persistent State
- **🧑‍🔬 作者**：Qianqian Wang, Yifei Zhang, Aleksander Holynski, Alexei A. Efros, Angjoo Kanazawa
- **🏫 单位**：UC Berkeley ⟐ Google DeepMind
- **🔗 链接**：[[中英摘要](./abs/2501.12387.md)] [[arXiv:2501.12387](https://arxiv.org/abs/2501.12387)] [[Code](https://github.com/CUT3R/CUT3R)]
- **📝 说明**：🏆 ICLR 2026 — 循环式状态更新，支持在线稠密重建

#### [29] Fast3R: Towards 3D Reconstruction of 1000+ Images in One Forward Pass
- **🧑‍🔬 作者**：Jianing Yang, Alexander Sax, Kevin J. Liang, Mikael Henaff, Hao Tang, Ang Cao, Joyce Chai, Franziska Meier, Matt Feiszli
- **🏫 单位**：Meta FAIR ⟐ University of Michigan
- **🔗 链接**：[[中英摘要](./abs/2501.13928.md)] [[arXiv:2501.13928](https://arxiv.org/abs/2501.13928)] [[Code](https://github.com/facebookresearch/fast3r)]
- **📝 说明**：🏆 ICLR 2025 — 单次前向传播处理 1000+ 张图像

#### [30] Spann3R: 3D Reconstruction with Spatial Memory
- **🧑‍🔬 作者**：Hengyi Wang, Lourdes Agapito
- **🏫 单位**：UCL (University College London)
- **🔗 链接**：[[中英摘要](./abs/2408.16061.md)] [[arXiv:2408.16061](https://arxiv.org/abs/2408.16061)] [[Code](https://github.com/HengyiWang/spann3r)]
- **📝 说明**：🏆 NeurIPS 2024 — 空间记忆机制，在全局坐标系中直接生成点图

#### [31] MV-DUSt3R+: Single-Stage Scene Reconstruction from Sparse Views In 2 Seconds
- **🧑‍🔬 作者**：Zhenggang Tang, Yuchen Fan, Dilin Wang, Hongyu Xu, Rakesh Ranjan, Alexander Schwing, Zhicheng Yan
- **🏫 单位**：Meta
- **🔗 链接**：[[中英摘要](./abs/2412.06974.md)] [[arXiv:2412.06974](https://arxiv.org/abs/2412.06974)] [Code]
- **📝 说明**：多视图同步重建 + 高斯溅射

#### [32] AMB3R: Accurate Feed-forward Metric-scale 3D Reconstruction with Backend
- **🧑‍🔬 作者**：Hengyi Wang, Lourdes Agapito
- **🏫 单位**：UCL (University College London)
- **🔗 链接**：[[中英摘要](./abs/2511.20343.md)] [[arXiv:2511.20343](https://arxiv.org/abs/2511.20343)] [Code]
- **📝 说明**：度量尺度前馈重建，稀疏体素后端

#### [33] Speed3R: Sparse Feed-forward 3D Reconstruction Models
- **🧑‍🔬 作者**：Weining Ren, Xiao Tan, Kai Han
- **🏫 单位**：The University of Hong Kong
- **🔗 链接**：[[中英摘要](./abs/2603.08055.md)] [[arXiv:2603.08055](https://arxiv.org/abs/2603.08055)] [Code]
- **📝 说明**：稀疏双分支注意力前馈重建，1000 视图序列 12.4 倍推理加速

---

## 单目几何估计

#### [34] MoGe: Unlocking Accurate Monocular Geometry Estimation for Open-Domain Images with Optimal Training Supervision
- **🧑‍🔬 作者**：Ruicheng Wang, Sicheng Xu, Cassie Dai, Jianfeng Xiang, Yu Deng, Xin Tong, Jiaolong Yang
- **🏫 单位**：Microsoft Research Asia
- **🔗 链接**：[[中英摘要](./abs/2410.19115.md)] [[arXiv:2410.19115](https://arxiv.org/abs/2410.19115)] [[Code](https://github.com/microsoft/MoGe)]
- **📝 说明**：🏆 CVPR 2025 Oral — 仿射不变单目几何估计

#### [35] Depth Anything 3: Recovering the Visual Space from Any Views
- **🧑‍🔬 作者**：Haotong Lin, Sili Chen, Junhao Liew, Donny Y. Chen, Zhenyu Li, Guang Shi, Jiashi Feng, Bingyi Kang
- **🏫 单位**：ByteDance
- **🔗 链接**：[[中英摘要](./abs/2511.10647.md)] [[arXiv:2511.10647](https://arxiv.org/abs/2511.10647)] [[Code](https://github.com/DepthAnything/Depth-Anything-V3)]
- **📝 说明**：超越 VGGT 的位姿精度 44.3%，几何精度 25.1%

---

## 综述

#### [36] Review of Feed-forward 3D Reconstruction: From DUSt3R to VGGT
- **🧑‍🔬 作者**：Wei Zhang, Yihang Wu, Songhua Li, Wenjie Ma, Xin Ma, Qiang Li, Qi Wang
- **🏫 单位**：Northwestern Polytechnical University
- **🔗 链接**：[[中英摘要](./abs/2507.08448.md)] [[arXiv:2507.08448](https://arxiv.org/abs/2507.08448)] [Code]
- **📝 说明**：从 DUSt3R 到 VGGT 的前馈式三维重建全面综述

---

## Star History

如果觉得本项目有帮助，欢迎 Star ⭐

## Acknowledgements

- 项目结构参考 [3D-Gaussian-Splatting-Papers](https://github.com/Awesome3DGS/3D-Gaussian-Splatting-Papers)
- [VGGT](https://github.com/facebookresearch/vggt) by Meta FAIR
- [DUSt3R](https://github.com/naver/dust3r) by NAVER LABS Europe
