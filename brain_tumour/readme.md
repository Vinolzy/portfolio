# 基于Transformer的脑肿瘤分类系统

本项目旨在构建一个基于医学影像的脑肿瘤自动分类系统，探索Transformer与传统CNN(如VGG16、AlexNet、ResNet18)在医学图像处理中的性能差异，并结合可解释性技术提升模型可信度与实用性。

## 项目结构说明

- `Preoptimized_Baseline_Model_Training_Code.ipynb`  
  
  基线模型训练代码，使用VGG16、AlexNet和ResNet18进行迁移学习，尚未进行优化处理，模型性能相对较低。
  
- `final-model.ipynb`  
  
  优化后的完整模型代码。包括去除冗余的数据增强、添加标准化处理、引入梯度裁剪，并在此基础上实现优化后的CNN模型与Transformer模型(分别处理RGB和灰度图像)。
  
- `Evaluation_Metrics_Along_Epochs_Plot.ipynb`  
  
  对模型训练和验证过程中F1分数与损失值进行可视化展示，数据来源于TensorBoard记录。
  
- `GradCAM_and_LLM_Intergration_Code.ipynb`  
  
  结合Grad-CAM与Gemini 2.0 Flash API，对模型输出的分类结果进行可解释性分析，提升用户对模型判断结果的信任度。
  
- `Model_Inference_and_Metrics_Plotting.ipynb`  
  
  加载训练过程中表现最优的模型，进行推理并评估其F1、Precision、Recall、Specificity，同时对比各模型的推理时间与参数规模。
  
- `基于Transformer的脑肿瘤分类系统.pdf`  
  
  项目的完整报告文档，详细说明研究背景、方法实现、结果分析与未来工作方向。

## 报告演示视频

> **Bilibili 视频链接：** [https://www.bilibili.com/video/BV1T98CzcEBd](https://www.bilibili.com/video/BV1T98CzcEBd)

[![演示视频](https://i1.hdslb.com/bfs/archive/fbe75afbd47d103e2b4d73255d7891f2481233d6.jpg@672w_378h_1c.webp)](https://www.bilibili.com/video/BV1T98CzcEBd)

如需更多细节，请参考各 notebook 文件及项目报告。