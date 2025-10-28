---
title: "DeepSeek-OCR 论文解读"
date: 2025-10-28
draft: false
tags: ["大模型", "AI"]
categories: ["学习"]
---
{{< quote >}}
DeepSeek-OCR 论文解读
{{< /quote >}}
<!--more-->
<iframe src="/pdf/deepseek-OCR.pdf#zoom=45" width="750" height="630"></iframe>

> [!Note]关键点
> - "due to quadratic scaling with sequence length."
> 是由于Attention机制本身导致的。
> - "rather than basic VQA [12, 16, 24, 32, 41]"
> 这是训练OCR普遍使用的一种方式
> - 主要的三个贡献
>     1. 定量分析本文视觉压缩
>     2. 设计DeepEncoder模块
>     3. 端到端模型构建与训练
> - "offering a promising direction for addressing long-context challenges in large language models. "
>   能够在LLM的长上下文问题中提供一定的可行性
> - 模型结构
>   ![image-20251028141438493](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/image-20251028141438493.png)
> - 数据
>   1. OCR（1.0和2.0）70%
>   2. 通用视觉数据（目标检测等）20%
>   3. 纯文本（文本token信息）10%
> - HAI-LLM
> 自己的模型训练平台框架，并行策略和算子优化
> - 对比、效果、实验、评估