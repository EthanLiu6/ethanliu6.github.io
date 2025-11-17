---
title: "平时的一些ideas"
date: 2025-10-24
draft: false
tags: ["ideas"]
categories: ["学术"]
weight: 1
---
{{< quote >}}
平常脑海突然觉得可尝试的一些ideas
{{< /quote >}}
<!--more-->

> [!NOTE] 头脑风暴

- 模型中间层随便random或者shuff一下会怎样

- 参数初始化以及token idx的值对模型效果有较大影响
* idx后的embedding模型咋训练

- 在Attention的时候会加重自身的注意力信息

* 多头注意力（以及优化的）是默认了各个子空间的重要性是平等的，是否需要分配不同的权重，如何有机融合？如何实现？

- 几乎每一个token在全句中的注意力都是稀疏的（MHA一方面缓解了这个问题）

- 不同注意力头attention后的可视化分析
> 论文：
> "What Does BERT Look At? An Analysis of BERT’s Attention"
> "Analyzing Multi-Head Self-Attention: Specialized Heads Do the Heavy Lifting, the Rest Can Be Pruned"
> "

- 头数目与emb_dim的分析对比（模型效果）

- 激活函数真的就不能升维度吗

- embedding在后层再用一次可以嘛（会不会跟short-cut的效果一样）

- 长序列输入可以先padding再压缩

- 关注度不等重要

- GBDT和ResNet思想一致

- 软间隔、标签平滑、噪音

- 高数，投影，降维度，积分

- 卷积转换成矩阵乘法跟那个旋转位置编码的旋转矩阵很相似哎

- 如何解决未来数据稀缺问题，或者数据高质量问题

- 一个领域的专业在另一行业就成为工具了（也是以后需要考虑和发展的方向）

- RNN的位置编码靠隐藏层状态矩阵

- 用极坐标改写RoPE

- 深度学习（特别是NLP领域）每五-六年进行一次大变革

- tokenizer识别不出来的token不一定会无法输出

- 栈具有记忆功能（状态机、自动机）

- MoE的加入以及负载均衡解决办法

- kl距离相对熵，和位置编码，交叉熵

- 开关和记忆（异或或者掩码用01比特序列）