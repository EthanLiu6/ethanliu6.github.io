---
title: "毕业论文Ideas: 其他Rec的Ideas"
date: 2025-12-27
draft: false
# password: true
tags: ["大模型","推荐系统"]
categories: ["学习", "LLM4Rec"]
---

{{< quote >}}
毕业论文Ideas: 推荐系统其他的Ideas
{{< /quote >}}
<!--more-->

> [!Note]借此实现（砍掉）我那颗“科研”的念想吧
自己本心是很喜欢探索和研究的，而且很享受那种感觉，事实上，真正尝试做的情况很少很少，很多都是有念头和想法，于是始终有一颗读研的打算（前提是得先考得上），但自己综合考虑之后是选择了先就业（打工）的，于是在选择后尽管自己很坚定，但始终有一个执念在我心头——研究，以至于在多次实习的时候，总是心头想着有个读研的打算，现在毕业论文其实就是一项真正的“研究”，他不同与我之前参加的一些竞赛，这种自我探索远比那些带着方向性的考验性更强，所以，这是让我的那个执念得以一定量放下的最好机会，至于以后是否有考研打算，顺势而为即可，至少，心中那颗心总算可以放一放了，那接下来，我就是慢慢做，做到自己以前想的那样种感觉，不能说要做的多么高大上、多么新颖，而且有一颗认真科研的心，探索里面的乐趣。Let's Go!

![20251227161659](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/20251227161659.png)

- 刺激能够触发记忆（回忆）
- Agent4Rec
- item带有description和‘亮点、特色’，user特色“喜好”
- 有“特别”的评论
- 有共鸣
- 推荐系统将进化为智能体（Agent）。
- 主动交互：当用户意图不明时，Agent 会反问：“你是想找商务风格还是休闲风格的鞋子？”
- 工具调用：Agent 可以调用搜索引擎查看最新测评，或者调用比价插件，为用户提供决策辅助。

- 数据并不一定都损失越小越好，可以随机一些噪音，反而更符合实际

# 数据
- kuairec，是快手的数据集
- microlens，短视频推荐数据集

![20251227163108](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/20251227163108.png)

- 标题、类别、品牌、价格、关键词和属性
- 标题、描述、类目、品牌、销售量排名以及价格等

![20251227165550](https://coderethan-1327000741.cos.ap-chengdu.myqcloud.com/blog-pics/20251227165550.png)

## Papers
- 快手：[OneRec: Unifying Retrieve and Rank with Generative Recommender and Preference Alignment](https://arxiv.org/pdf/2502.18965). 2025-02

- 腾讯：[OnePiece: The Great Route to Generative Recommendation -- A Case Study from Tencent Algorithm Competition](https://arxiv.org/pdf/2512.07424). 2025-12

- Meta:[Scaling Generative Recommendations with Context Parallelism on Hierarchical Sequential Transducers](https://arxiv.org/pdf/2508.04711). 2025-08

- 美团：[Multi-Aspect Cross-modal Quantization for Generative Recommendation](https://arxiv.org/abs/2511.15122). 2025-11

- 快手： [UniSearch: Rethinking Search System with a Unified Generative Architecture](https://arxiv.org/pdf/2509.06887). 2025-09

- SIGIR: [Generative Recommender with End-to-End Learnable Item Tokenization](https://arxiv.org/abs/2409.05546). 2024-09-2025-06

- 阿里：[Scaling Transformers for Discriminative Recommendation via Generative Pretraining](https://arxiv.org/pdf/2506.03699). 2025-06

- [LLM-based Conversational Recommendation Agents with Collaborative Verbalized Experience](https://genai-personalization.github.io/assets/papers/GenAIRecP2025/2_Yaochan.pdf). 2025-11

- Google: [REGEN: Empowering personalized recommendations with natural language](https://research.google/blog/regen-empowering-personalized-recommendations-with-natural-language/). 2025-06

- KDD: [A Review of Modern Recommender Systems Using Generative Models (Gen-RecSys)](https://arxiv.org/pdf/2404.00579v2). 2024-07

- 解读整理：[2025年生成式推荐系统领域最具代表性10篇论文综述](https://zhuanlan.zhihu.com/p/1983610196241704717)


- Shopee [OnePiece: Bringing Context Engineering andReasoning to Industrial Cascade Ranking System](https://arxiv.org/pdf/2509.18091). 2025-09

- 快手综述：[A Survey of Generative Recommendation from a Tri-Decoupled Perspective: Tokenization, Architecture, and Optimization](https://www.preprints.org/manuscript/202512.0203). 2025-12

- 范式：[一文梳理业界落地LLM4Rec的若干范式](https://zhuanlan.zhihu.com/p/19923334099)

- 快手：[KuaiFormer: Transformer-Based Retrieval at Kuaishou](https://arxiv.org/pdf/2411.10057) 2024-11
> https://zhuanlan.zhihu.com/p/1960092167272899457
