---
title: "LLM4Rec论文阅读: KuaiFormer"
date: 2026-01-10
draft: false
tags: ["大模型","推荐系统"]
categories: ["学习", "LLM4Rec"]
---

{{< quote >}}
LLM4Rec论文阅读——KuaiFormer
{{< /quote >}}
<!--more-->

双语对照：[KuaiFormer](https://yiyibooks.cn/arxiv/2411.10057v1/index.html)

短视频推荐提出了独特的挑战，需要先进的建模技术。 短视频内容的多样性和用户兴趣的快速演变需要实时适应以准确捕捉这些动态偏好。 用户通常每天观看数百个短视频，表达广泛兴趣领域的偏好，而系统则主动推送多样化内容，以缓解审美疲劳并避免“过滤气泡”效应。 因此，依赖每日更新的模型，例如 PinnerFormer（Pancha 等人，2022），很难适应用户不断变化的内容需求。 此外，SASRec 和 Bert4Rec 等传统方法将用户行为压缩为单个兴趣向量，缺乏准确捕获这些交互中反映的全部用户兴趣的能力。

为了更有效地捕获复杂的用户兴趣，MIND （Li 等人，2019）和 ComiRec （Cen 等人，2020）等模型采用胶囊网络等技术从用户动作序列中提取多个兴趣向量。 然而，由于这些模型不利用基于 Transformer 的原生架构，因此它们在充分利用 Transformer 提供的优势方面受到限制。 此外，它们没有解决与处理长序列相关的性能开销，这是工业应用中的一个重要问题。

![图形用户界面, 文本, 应用程序, 电子邮件  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image001.png)

![图形用户界面, 文本, 电子邮件  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image002.png)

![文本, 信件  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image003.png)数据并不一定都损失越小越好，可以随机一些噪音，反而更符合实际

![图示  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image004.png)

![图形用户界面, 文本, 应用程序  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image005.png)

![图形用户界面, 文本, 应用程序, 电子邮件  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image006.png)

![图形用户界面, 文本, 应用程序  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image007.png)

![日程表  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image008.png)

下面那个部署架构还没完全理解。

![img](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image009.png)

![文本, 信件  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image010.png)

![文本  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image011.png)

![图表, 折线图  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image012.png)

![图片包含 文本  AI 生成的内容可能不正确。](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/clip_image013.png)