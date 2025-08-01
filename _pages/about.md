---
permalink: /
title: "基础信息"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## 👤 个人信息

| 🏷️ 姓名   | 👨‍🦰 性别 | 🏛️ 政治面貌 | 🎂 出生年月   | 📧 邮箱              | 📱 电话         | 🏡 籍贯     | 🎓 学历               |
|:----------:|:--------:|:------------:|:--------------:|:--------------------:|:--------------:|:----------:|:---------------------:|
| **杨纯金** | 男       | 中共党员     | 2000年05月     | [au_young@163.com](mailto:au_young@163.com) | 15687459217  | 云南曲靖     | 电子科技大学 硕士     |


---

## 🎓 主要研究方向
**多模态大语言模型(MLLM) | 多模态目标检测 | 视觉-动作-语言(VLA) |目标检测| RAG**  

---

## 📄 学术成果
* [Instance-Wise Adaptive Tuning and Caching for Vision-Language Models](https://ebooks.iospress.nl/doi/10.3233/FAIA230595) ECAI-23 CCF-B 
* [neuro-symbolic method for explainable remote sensing visual question answer](https://2025.ieeeigarss.org/tempdev/view_paper.php?PaperNum=3196&SessionID=1628) 遥感顶会IGARSS,CCF-B 
* [CMP: Composable Meta Prompt for SAM-based Cross-Domain Few-shot Segmentation](https://cmsworkshops.com/ICIP2025/papers/accepted_papers.php) ICIP-25 CCF-C 
* [SS-DC: Spatial-Spectral Decoupling and Coupling Across Visible-Infrared Gap for Domain Adaptive Object Detection](https://arxiv.org/abs/2507.12017) arxiv
* Wavelet-Based Multispectral Detection Transformer with Adaptive Frequency-aware Query Learning TGRS (在投)

---

## 🎓 教育经历

* **2019年-2023年** 电子科技大学 本科 信息与通信工程学院 信息与通信工程专业（A+）
    * 🏅 2023年 优秀共产党员荣誉
    * 🥇 2022年 国家奖学金
    * 🏆 2022年 海军xxx算法挑战赛xxx 全国冠军
    * 🥈 2022年 蓝桥杯嵌入式组 四川省二等奖
    * 🥈 2022年 光电设计大赛 校级二等奖
    * 🥇 2021年 全国大学生数学竞赛 四川省一等奖
    * 🥇 2021年 国家励志奖学金
    * 🏅 2021年 优秀学生奖学金
    * 🏅 2021年 优秀共青团员
    * 🥇 2020年 国家励志奖学金
    * 🏅 2020年 优秀学生奖学金
    * 📝 2020年 卧谈会征文比赛 校级三等奖
    * 🏅 2020年 优秀社会实践队队员 校级二等奖
    * 🏅 2020年 优秀共青团员

* **2023年-2025年** 电子科技大学 硕士 信息与通信工程学院 信息与通信工程专业（A+）
    * 📄 2025年 neuro-symbolic method for explainable remote sensing visual question answer 遥感顶会，CCF-B 论文中稿
    * 📄 2025年 CMP: Composable Meta Prompt for SAM-based Cross-Domain Few-shot Segmentation ICIP CCF-C  论文中稿
    * 🥉 2024年 “华为杯”第6届研究生人工智能创新大赛 全国三等奖
    * 📄 2023年 Instance-Wise Adaptive Tuning and Caching for Vision-Language Models ECAI CCF-B 论文中稿

---

## 🏢 实习经历

**蔚来汽车 | 自动驾驶-大模型开发与应用部门 | 多模态Agent团队**  
<small>2024年-05月至今</small>

- **主要工作**：基于多模态大语言模型的地下停车场端到端自动驾驶VLA算法研发，提出短思维链数据pipeline构建大规模场景VLA数据，微调Qwen2.5-VL-7B+DiT模型，实现地下停车场自动导航算法，在验证集上的未来3s预测轨迹的L2距离达到0.55m。

- **技术贡献**：
    1. 为克服自然场景与自动驾驶领域的模态差异，整合9个主流开源自动驾驶VQA数据集。通过统一bbox标注规范，适配Qwen2.5-VL动态尺寸输入要求，构建规模达230万条的自动驾驶多模态QA数据集。基于该数据集，采用DeepSpeed Zero-2对QwenVL-2.5-7B模型进行全参数微调,作为基础模型。
    2. 针对地下停车场的场景，提出地下停车短COT数据集构建pipeline。首先使用YOLOv8+ByteTrack对所有的路牌进行检测和跟踪，微调Qwen2.5-VL-32B构建专用OCR模型并人工校验关键路牌语义绑定；然后按照“我在哪，为什么，当前状态，下一步应该去哪，为什么？未来三秒的轨迹”的模板构造短COT并使用Qwen3丰富语料库用词，共得到12.5万对结构化推理图文对；最后，为提高没有路牌时模型的性能，提出视觉COT方法，通过从历史4帧中每帧随机采样25%的token与当前帧的token一起送给大语言模型，通过该方法测试集轨迹预测误差降低2.1%。
    3. 针对复杂路口场景的多模态轨迹预测挑战，设计 Diffusion Transformer策略模型，通过Action Token条件逐步降噪生成连续轨迹，采用MSE损失约束轨迹生成过程​，强化动作序列的连续性，与QA任务联合训练，实现多任务协同优化​；相较纯语言模型预测方案，轨迹预测准确率提升5.5%​，该架构通过轨迹生成与语义理解的深度耦合​，同步增强端到端决策的可解释性，并在无路牌场景下将轨迹定位误差降低3.2%。

---

## 🚀 项目 & 科研

### 🔥 四川省智慧消防系统  
*主研/技术负责人*  
<small>四川省消防某单位校企合作 | 2024年10月-至今</small>

- **项目概述**：联合四川消防图层系统公司，构建智能消防系统，融合领域小模型与大规模视觉语言模型，实现消防全要素检测与综合分析，辅助灾情响应，部分功能已上线“消川”大模型。
- **技术贡献**：
    - 结合公开数据预训练与伪标签迭代优化，扩充检测数据，提升模型泛化能力。
    - 两阶段检测与细分类，切片并行推理，模型加速，实时检测识别30FPS。
    - Grounded-SAM2开放词汇跳帧分割，miniCPM-o火灾类型判断准确率93%。
    - Qwen2.5-VL-32B生成caption，LoRA微调Qwen2.5-VL-7B，实现多模态问答。

---

### 🛰️ 某单位智能识别系统  
*主研/专班成员*  
<small>国家重大项目 | 2024年3月-至今</small>

- **项目概述**：构建红外、可见光、SAR等多模态检测模型，实现复杂环境下目标定位与识别，MLLM综合分析HQ。
- **技术贡献**：
    - 双路融合检测算法，模态dropout机制，自适应模态丢失。
    - 频域-空域融合目标检测，DCT分离噪声与特征，抗干扰性提升。
    - GAF角场统一特征域，通道dropout与多模型融合，提升识别准确率。
    - Qwen2-VL-32B提取caption，LoRA微调miniCPM-V，Ascend 910B平台部署。

---

### 🖼️ 基于大规模视觉语言模型的图像质量评估算法研究  
*主研/专班成员*  
<small>华为竞赛 | 2024年7月-2024年10月</small>

- **研究目标**：构建全新图像质量评估模型，获全国三等奖。
- **技术贡献**：
    - 使用CLIP VIT-H编码器，多任务prompt提升理解能力。
    - 多任务回归头，结合图像与文本特征综合评估。

---

### 🌈 多波段单域泛化算法研究  
*主研/核心成员*  
<small>中科院合作项目 | 2023年12月-2024年5月</small>

- **研究目标**：基于可见光-红外图像跨域目标检测，探索共性与特性，内部测试比赛第一名。
- **技术贡献**：
    - 可见光转灰度，缩小域差异，循环解耦模块实现风格与内容解耦。
    - 透视变换、多尺度、随机压缩等数据增广，课程学习多阶段训练提升泛化性。
    - 切片推理提升小目标检测识别能力。

---

### 🧩 基于部件库的多模态分类算法研究  
*核心成员*  
<small>启元实验室合作项目 | 2023年9月-2023年12月</small>

- **研究目标**：基于部件库，构建多模态融合算法提升可见光与深度图融合识别准确性，性能提升大于10%。
- **技术贡献**：
    - 使用languagebind文本编码器构建200部件特征库，图像编码器编码可见光与深度图。
    - 跨模态融合模块，交叉注意力特征融合，多任务分类头，最终分类准确率提升。

---