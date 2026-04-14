# 2026 Papers

#### [1] InfiniteVGGT: Visual Geometry Grounded Transformer for Endless Streams
- **🧑‍🔬 作者**：Shuai Yuan, Yantai Yang, Xiaotian Yang, Xupeng Zhang, Zhonghao Zhao, Lingming Zhang, Zhipeng Zhang
- **🏫 单位**：Shanghai Jiao Tong University
- **🔗 链接**：[[中英摘要](../abs/2601.02281.md)] [[arXiv:2601.02281](https://arxiv.org/abs/2601.02281)] [[Code](https://github.com/AutoLab-SAI-SJTU/InfiniteVGGT)]
- **📝 说明**：因果 VGGT + 自适应 KV 缓存裁剪，支持无限时间范围流式重建

#### [2] GPA-VGGT: Adapting VGGT to Large Scale Localization by Self-Supervised Learning with Geometry and Physics Aware Loss
- **🧑‍🔬 作者**：Yangfan Xu, Lilian Zhang, Xiaofeng He, Yugui Shen, Pengdong Wu, Wenqi Wu, Jun Mao
- **🏫 单位**：未标注
- **🔗 链接**：[[中英摘要](../abs/2601.16885.md)] [[arXiv:2601.16885](https://arxiv.org/abs/2601.16885)] [[Code](https://github.com/X-yangfan/GPA-VGGT)]
- **📝 说明**：自监督 VGGT 大规模定位，几何与物理感知联合优化

#### [3] VGGT-SLAM 2.0: Real-time Dense Feed-forward Scene Reconstruction
- **🧑‍🔬 作者**：Dominic Maggio, Luca Carlone
- **🏫 单位**：MIT
- **🔗 链接**：[[中英摘要](../abs/2601.19887.md)] [[arXiv:2601.19887](https://arxiv.org/abs/2601.19887)] [Code]
- **📝 说明**：实时前馈 SLAM，位姿误差比 VGGT-SLAM 减少约 23%

#### [4] tttLRM: Test-Time Training for Long Context and Autoregressive 3D Reconstruction
- **🧑‍🔬 作者**：Chen Wang, Hao Tan, Wang Yifan, Zhiqin Chen, Yuheng Liu, Kalyan Sunkavalli, Sai Bi, Lingjie Liu, Yiwei Hu
- **🏫 单位**：University of Pennsylvania ⟐ Adobe Research ⟐ UC Irvine
- **🔗 链接**：[[中英摘要](../abs/2602.20160.md)] [[arXiv:2602.20160](https://arxiv.org/abs/2602.20160)] [[Code](https://github.com/cwchenwang/tttLRM)]
- **📝 说明**：🏆 CVPR 2026 — TTT 层压缩观测至快速权重，线性复杂度长上下文自回归 3D 重建

#### [5] VGG-T3: Offline Feed-Forward 3D Reconstruction at Scale
- **🧑‍🔬 作者**：Sven Elflein, Ruilong Li, Sérgio Agostinho, Zan Gojcic, Laura Leal-Taixé, Qunjie Zhou, Aljosa Osep
- **🏫 单位**：NVIDIA ⟐ Technical University of Munich
- **🔗 链接**：[[中英摘要](../abs/2602.23361.md)] [[arXiv:2602.23361](https://arxiv.org/abs/2602.23361)] [Code]
- **📝 说明**：VGGT + TTT，将 KV 表示蒸馏为固定大小 MLP，线性复杂度，处理 1000 张图像仅需 54 秒

#### [6] VGGT-Det: Mining VGGT Internal Priors for Sensor-Geometry-Free Multi-View Indoor 3D Object Detection
- **🧑‍🔬 作者**：Yang Cao, Feize Wu, Dave Zhenyu Chen, Yingji Zhong, Lanqing Hong, Dan Xu
- **🏫 单位**：HKUST ⟐ Huawei Noah's Ark Lab
- **🔗 链接**：[[中英摘要](../abs/2603.00912.md)] [[arXiv:2603.00912](https://arxiv.org/abs/2603.00912)] [Code]
- **📝 说明**：无传感器几何的多视图室内 3D 目标检测，利用 VGGT 内部语义 + 几何先验

#### [7] LoGeR: Long-Context Geometric Reconstruction with Hybrid Memory
- **🧑‍🔬 作者**：Junyi Zhang, Charles Herrmann, Junhwa Hur, Chen Sun, Ming-Hsuan Yang, Forrester Cole, Trevor Darrell, Deqing Sun
- **🏫 单位**：Google DeepMind ⟐ UC Berkeley
- **🔗 链接**：[[中英摘要](../abs/2603.03269.md)] [[arXiv:2603.03269](https://arxiv.org/abs/2603.03269)] [[Code](https://github.com/Junyi42/LoGeR)]
- **📝 说明**：TTT 记忆 + 滑动窗口注意力混合架构，128 帧训练泛化至数千帧，KITTI ATE 降低 74%

#### [8] ZipMap: Linear-Time Stateful 3D Reconstruction via Test-Time Training
- **🧑‍🔬 作者**：Haian Jin, Rundi Wu, Tianyuan Zhang, Ruiqi Gao, Jonathan T. Barron, Noah Snavely, Aleksander Hołyński
- **🏫 单位**：Google DeepMind ⟐ Cornell University ⟐ MIT
- **🔗 链接**：[[中英摘要](../abs/2603.04385.md)] [[arXiv:2603.04385](https://arxiv.org/abs/2603.04385)] [[Code](https://github.com/Haian-Jin/ZipMap)]
- **📝 说明**：TTT 层压缩图像集合为紧凑隐式场景状态，700+ 帧 10 秒内重建，比 VGGT 快 20 倍以上

#### [9] Speed3R: Sparse Feed-forward 3D Reconstruction Models
- **🧑‍🔬 作者**：Weining Ren, Xiao Tan, Kai Han
- **🏫 单位**：The University of Hong Kong
- **🔗 链接**：[[中英摘要](../abs/2603.08055.md)] [[arXiv:2603.08055](https://arxiv.org/abs/2603.08055)] [Code]
- **📝 说明**：稀疏双分支注意力前馈重建，1000 视图序列 12.4 倍推理加速

#### [10] VGGT-World: Transforming VGGT into an Autoregressive Geometry World Model
- **🧑‍🔬 作者**：Xiangyu Sun, Shijie Wang, Fengyi Zhang, Lin Liu, Caiyan Jia, Ziying Song, Zi Huang, Yadan Luo
- **🏫 单位**：Beijing Jiaotong University ⟐ University of Queensland
- **🔗 链接**：[[中英摘要](../abs/2603.12655.md)] [[arXiv:2603.12655](https://arxiv.org/abs/2603.12655)] [Code]
- **📝 说明**：将 VGGT 转化为自回归几何世界模型，速度快 3.6-5 倍，仅 0.43B 参数

#### [11] PanoVGGT: Feed-Forward 3D Reconstruction from Panoramic Imagery
- **🧑‍🔬 作者**：Yijing Guo, Mengjun Chao, Luo Wang, Tianyang Zhao, Haizhao Dai, Yingliang Zhang, Jingyi Yu, Yujiao Shi
- **🏫 单位**：ShanghaiTech University
- **🔗 链接**：[[中英摘要](../abs/2603.17571.md)] [[arXiv:2603.17571](https://arxiv.org/abs/2603.17571)] [Code]
- **📝 说明**：全景图像前馈式 3D 重建，球面感知位置编码

#### [12] HD-VGGT: High-Resolution Visual Geometry Transformer
- **🧑‍🔬 作者**：Tianrun Chen, Yuanqi Hu, Yidong Han, Hanjie Xu, Deyi Ji, Qi Zhu, Chunan Yu, Xin Zhang, Cheng Chen, Chaotao Ding, Ying Zang, Xuanfu Li, Jin Ma, Lanyun Zhu
- **🏫 单位**：Zhejiang University of Technology ⟐ KOKONI3D
- **🔗 链接**：[[中英摘要](../abs/2603.27222.md)] [[arXiv:2603.27222](https://arxiv.org/abs/2603.27222)] [Code]
- **📝 说明**：双分支设计，低分辨率粗糙几何 + 高分辨率细节增强

#### [13] Scal3R: Scalable Test-Time Training for Large-Scale 3D Reconstruction
- **🧑‍🔬 作者**：Tao Xie, Peishan Yang, Yudong Jin, Yingfeng Cai, Wei Yin, Weiqiang Ren, Qian Zhang, Wei Hua, Sida Peng, Xiaoyang Guo, Xiaowei Zhou
- **🏫 单位**：Zhejiang University ⟐ Horizon Robotics ⟐ Zhejiang Lab
- **🔗 链接**：[[中英摘要](../abs/2604.08542.md)] [[arXiv:2604.08542](https://arxiv.org/abs/2604.08542)] [[Code](https://github.com/zju3dv/Scal3R)]
- **📝 说明**：🏆 CVPR 2026 Highlight — 神经全局上下文表示 + 轻量子网络测试时自监督适应，公里级大规模场景重建

#### [14] VGGT-SLAM++
- **🧑‍🔬 作者**：Avilasha Mandal, Rajesh Kumar, Sudarshan Sunil Harithas, Chetan Arora
- **🏫 单位**：IIT Delhi
- **🔗 链接**：[[中英摘要](../abs/2604.06830.md)] [[arXiv:2604.06830](https://arxiv.org/abs/2604.06830)] [Code]
- **📝 说明**：完整 VGGT 视觉 SLAM 系统，含 DEM 图模块与闭环检测

#### [15] VGGT-Geo: Probabilistic Geometric Fusion of Visual Geometry Grounded Transformer Priors for Robust Dense Indoor SLAM
- **🧑‍🔬 作者**：Kai Qin, Jing Li, Sisi Zlatanova, Haitao Wu, Hao Wu, Yin Gao, Dingjie Zhou, Yuchen Li, Sizhe Shen, Xiangjun Qu, Zhenxin Zhang, Banghui Yang, Shicheng Xu
- **🏫 单位**：Northwestern Polytechnical University
- **🔗 链接**：[[DOI](https://doi.org/10.3390/ijgi15020085)]
- **📝 说明**：ISPRS IJGI 2026 — 概率几何融合框架，轨迹精度提升约 50%

#### [16] OV3DSeg-VGGT: Open-Vocabulary 3D Segmentation with Visual Geometry-Grounded Transformers
- **🧑‍🔬 作者**：Jingke Zhou, Xianliang Huang, Yixin Ren, Dikai Fan, Shengyu Gu, Bin Tian, Xiao Liu, Tianjia Shao
- **🏫 单位**：Zhejiang University
- **🔗 链接**：[[DOI](https://doi.org/10.1016/j.visinf.2026.100311)]
- **📝 说明**：Visual Informatics 2026 — 基于 VGGT 的开放词汇 3D 分割

#### [17] Fast vision-based 3D reconstruction and damage detection of building structures based on visual geometry grounded transformer
- **🧑‍🔬 作者**：Yumeng Chen, Xiao Pan, Haoyang Zhang, Yousufu Ma, Haoyu Zhang
- **🏫 单位**：未标注
- **🔗 链接**：[[DOI](https://doi.org/10.1016/j.jobe.2026.116066)]
- **📝 说明**：J. Building Engineering 2026 — VGGT 用于建筑结构快速 3D 重建与损伤检测

#### [18] Zero-shot text-to-3D-object generation with visual-geometry-grounded transformer
- **🧑‍🔬 作者**：Dong-hun Lee, Sang-hyo Park
- **🏫 单位**：未标注
- **🔗 链接**：[[DOI](https://doi.org/10.1117/12.3102112)]
- **📝 说明**：SPIE IWAIT 2026 — 基于 VGGT 的零样本文本到 3D 物体生成

#### [19] Review of Feed-forward 3D Reconstruction: From DUSt3R to VGGT
- **🧑‍🔬 作者**：Wei Zhang, Yihang Wu, Songhua Li, Wenjie Ma, Xin Ma, Qiang Li, Qi Wang
- **🏫 单位**：Northwestern Polytechnical University
- **🔗 链接**：[[中英摘要](../abs/2507.08448.md)] [[arXiv:2507.08448](https://arxiv.org/abs/2507.08448)] [Code]
- **📝 说明**：从 DUSt3R 到 VGGT 的前馈式三维重建全面综述
