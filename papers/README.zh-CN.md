# 📃 论文

## 模型架构

| 标题 | 发表日期  | 作者 | 核心内容 | 链接  |
| ----- | ----- | ----- | ----- | -----  |
| 《Attention Is All You Need》 | 2017年6月 | Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin | 提出了完全摒弃循环和卷积网络的Transformer架构，仅依靠自注意力机制处理序列数据，通过并行计算和位置编码高效捕捉长距离依赖关系 | <https://arxiv.org/abs/1706.03762> |

## 预训练和缩放定律 

| 标题 | 发表日期  | 作者 | 核心内容 | 链接  |
| ----- | ----- | ----- | ----- | -----  |
| 《BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding》 | 2019年 | Jacob Devlin, Ming-Wei Chang, Kenton Lee, Kristina Toutanova (Google AI) | 提出通过掩码语言模型（MLM）实现真正的双向上下文理解，确立了“预训练+微调”范式 | <https://aclanthology.org/N19-1423/> |
| 《Language Models are Few-Shot Learners》| 2020年5月 | Tom B. Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah, Jared Kaplan, Prafulla Dhariwal, Arvind Neelakantan, Pranav Shyam, Girish Sastry, Amanda Askell, Sandhini Agarwal, Ariel Herbert-Voss, Gretchen Krueger, Tom Henighan, Rewon Child, Aditya Ramesh, Daniel M. Ziegler, Jeffrey Wu, Clemens Winter, Christopher Hesse, Mark Chen, Eric Sigler, Mateusz Litwin, Scott Gray, Benjamin Chess, Jack Clark, Christopher Berner, Sam McCandlish, Alec Radford, Ilya Sutskever, Dario Amodei (OpenAI) | 介绍1750亿参数的GPT-3，通过少样本上下文学习在多种任务上取得竞争力 | <https://arxiv.org/abs/2005.14165> |
| 《Scaling Laws for Neural Language Models》 | 2020年 | Jared Kaplan, Sam McCandlish, Tom Henighan, Tom B. Brown, Benjamin Chess, Rewon Child, Scott Gray, Alec Radford, Jeffrey Wu, Dario Amodei (OpenAI) | 系统研究模型性能与参数量、数据集大小、计算量之间的幂律关系 | <https://arxiv.org/abs/2001.08361> |
| 《Training Compute-Optimal Large Language Models》 | 2022年3月 | Jordan Hoffmann, Sebastian Borgeaud, Arthur Mensch, Elena Buchatskaya, Trevor Cai, Eliza Rutherford, Diego de Las Casas, Lisa Anne Hendricks, Johannes Welbl, Aidan Clark, Tom Hennigan, Eric Noland, Katie Millican, George van den Driessche, Bogdan Damoc, Aurelia Guy, Simon Osindero, Karen Simonyan, Erich Elsen, Jack W. Rae, Oriol Vinyals, Laurent Sifre (DeepMind) | 挑战“模型越大越好”的认知，提出模型大小和训练数据应同步增长 | <https://arxiv.org/abs/2203.15556> |

## 人类对齐和RLHF

| 标题 | 发表日期  | 作者 | 核心内容 | 链接  |
| ----- | ----- | ----- | ----- | -----  |
| 《Deep Reinforcement Learning from Human Preferences》 | 2017年6月 | Paul F. Christiano, Jan Leike, Tom B. Brown, Miljan Martic, Shane Legg, Dario Amodei (OpenAI) | 开创性地从人类偏好比较中学习奖励模型，用于强化学习训练 | <https://arxiv.org/abs/1706.03741> |
| 《Training language models to follow instructions with human feedback》 | 2022年3月 | Long Ouyang, Jeff Wu, Xu Jiang, Diogo Almeida, Carroll L. Wainwright, Pamela Mishkin, Chong Zhang, Sandhini Agarwal, Katarina Slama, Alex Ray, John Schulman, Jacob Hilton, Fraser Kelton, Luke Miller, Maddie Simens, Amanda Askell, Peter Welinder, Paul Christiano, Jan Leike, Ryan Lowe (OpenAI) | 使用RLHF训练语言模型更好地遵循指令，InstructGPT在参数更小的情况下表现更优 | <https://arxiv.org/abs/2203.02155> |
| 《Direct Preference Optimization: Your Language Model is Secretly a Reward Model》 | 2023年 | Rafael Rafailov, Archit Sharma, Eric Mitchell, Stefano Ermon, Christopher D. Manning, Chelsea Finn (Stanford) | 提出直接利用偏好数据优化模型，无需单独训练奖励模型 | <https://arxiv.org/abs/2305.18290> | 

## 提示和推理

| 标题 | 发表日期  | 作者 | 核心内容 | 链接  |
| ----- | ----- | ----- | ----- | -----  |
| 《Chain-of-Thought Prompting Elicits Reasoning in Large Language Models》| 2022年1月 | Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Brian Ichter, Fei Xia, Ed H. Chi, Quoc V. Le, Denny Zhou (Google Research) | 发现通过引导模型输出逐步推理链，可大幅提升复杂推理任务的准确率 | <https://arxiv.org/abs/2201.11903> |
| 《Tree of Thoughts: Deliberate Problem Solving with Large Language Models》 | 2023年5月 | Shunyu Yao, Dian Yu, Jeffrey Zhao, Izhak Shafran, Thomas L. Griffiths, Yuan Cao, Karthik Narasimhan (Princeton, Google DeepMind) | 扩展CoT为思维树，允许多条推理路径和自我评估选择 | <https://arxiv.org/abs/2305.10601> |


## 开源模型

| 标题 | 发表日期  | 作者 | 核心内容 | 链接  |
| ----- | ----- | ----- | ----- | -----  |
| 《LLaMA: Open and Efficient Foundation Language Models》 | 2023年2月 | Hugo Touvron, Thibaut Lavril, Gautier Izacard, Xavier Martinet, Marie-Anne Lachaux, Timothée Lacroix, Baptiste Rozière, Naman Goyal, Eric Hambro, Faisal Azhar, Aurelien Rodriguez, Armand Joulin, Edouard Grave, Guillaume Lample (Meta AI) | 发布70亿到650亿参数的开源模型，证明小模型经充分训练可超越大模型 | <https://arxiv.org/abs/2302.13971> | 

## 效率优化

| 标题 | 发表日期  | 作者 | 核心内容 | 链接  |
| ----- | ----- | ----- | ----- | -----  |
| 《FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness》 | 2022年5月 | Tri Dao, Daniel Y. Fu, Stefano Ermon, Atri Rudra, Christopher Ré (Stanford) | 通过IO感知的算法设计，大幅提升注意力计算的速度和内存效率 | <https://arxiv.org/abs/2205.14135> |

## 检索增强生成

| 标题 | 发表日期  | 作者 | 核心内容 | 链接  |
| ----- | ----- | ----- | ----- | -----  |
| 《Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks》 | 2020年 | Patrick Lewis, Ethan Perez, Aleksandra Piktus, Fabio Petroni, Vladimir Karpukhin, Naman Goyal, Heinrich Küttler, Mike Lewis, Wen-tau Yih, Tim Rocktäschel, Sebastian Riedel, Douwe Kiela (Facebook AI, UCL, NYU) | 首次提出RAG框架，结合预训练参数记忆与非参数检索记忆 | <	https://arxiv.org/abs/2005.11401> |


## 智能体

| 标题 | 发表日期  | 作者 | 核心内容 | 链接  |
| ----- | ----- | ----- | ----- | -----  |
| 《ReAct: Synergizing Reasoning and Acting in Language Models》 | 2022年10月 | Shunyu Yao, Jeffrey Zhao, Dian Yu, Nan Du, Izhak Shafran, Karthik Narasimhan, Yuan Cao (Princeton, Google Research) | 提出推理与行动协同的Agent框架，通过与外部工具交互解决复杂任务 | <https://arxiv.org/abs/2210.03629> |
| 《SWE-Bench: Can Language Models Resolve Real-World GitHub Issues?》 | 2023年10月 | Carlos E. Jimenez, John Yang, Alexander Wettig, Shunyu Yao, Kexin Pei, Ofir Press, Karthik R. Narasimhan (Princeton, Chicago) | 提出评估LLM解决真实GitHub问题能力的基准测试 | <https://arxiv.org/abs/2310.06770> | 

## 多模态

| 标题 | 发表日期  | 作者 | 核心内容 | 链接  |
| ----- | ----- | ----- | ----- | -----  |
| 《GPT-4 Technical Report》 | 2023年3月 | OpenAI | 介绍大规模多模态模型GPT-4，展示其在各类基准上的“人类水平”性能 | <https://arxiv.org/abs/2303.08774> |

## 综述与展望

| 标题 | 发表日期  | 作者 | 核心内容 | 链接  |
| ----- | ----- | ----- | ----- | -----  |
| 《A Survey of Large Language Models》 | 2023年 | Wayne Xin Zhao, Kun Zhou, Junyi Li, Tianyi Tang, Xiaolei Wang, Yupeng Hou, Yingqian Min, Beichen Zhang, Junjie Zhang, Zican Dong, Yifan Du, Chen Yang, Yushuo Chen, Zhipeng Chen, Jinhao Jiang, Ruiyang Ren, Yifan Li, Xinyu Tang, Zikang Liu, Peiyu Liu, Jian-Yun Nie, Ji-Rong Wen (Renmin University, Beijing) | 全面回顾大语言模型的发展、技术架构和应用 | <https://arxiv.org/abs/2303.18223> |
| 《AI Alignment: A Comprehensive Survey》 | 2023年 | Jiaming Ji, Tianyi Qiu, Boyuan Chen, Borong Zhang, Hantao Lou, Kaile Wang, Yawen Duan, Zhonghao He, Jiayi Zhou, Zhaowei Zhang, Fanzhi Zeng, Kwan Yee Ng, Juntao Dai, Xuehai Pan, Aidan O‘Gara, Yingshan Lei, Hua Xu, Brian Tse, Jie Fu, Stephen McAleer, Yaodong Yang, Yizhou Wang, Song-Chun Zhu, Yike Guo, Wen Gao (Peking University, Tsinghua, Cambridge, etc.) | 全面综述AI对齐技术，包括RLHF、宪法AI等 | <https://arxiv.org/abs/2310.19852> |


