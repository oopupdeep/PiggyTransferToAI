原文地址[[2306.00978] AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration](https://arxiv.org/abs/2306.00978)

### 背景
大模型量化（8bit量化和4bit量化）能显著降低内存大小。但是QAT方法会显著的增加训练时长，PTQ方法会造成大量的精度损失。在这样的背景下，作者提出了awq方法。

### 基本思想
awq量化技术基于这样一种观察：权重并非同等重要，只保护 1%的突出权重可以大大减少量化误差。

