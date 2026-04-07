# 📃 Papers

## Model Architecture

| Title | Publication Date | Author | Core Content | Link |
| ----- | ----- | ----- | ----- | ----- |
| ***Attention Is All You Need*** | June 2017 | Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin | Proposes the Transformer architecture that completely dispenses with recurrence and convolutions, relying solely on self-attention mechanisms to process sequence data, efficiently capturing long-range dependencies through parallel computation and positional encoding. | <https://arxiv.org/abs/1706.03762> |

## Pre-training and Scaling Laws

| Title | Publication Date | Author | Core Content | Link |
| ----- | ----- | ----- | ----- | ----- |
| ***BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding*** | 2019 | Jacob Devlin, Ming-Wei Chang, Kenton Lee, Kristina Toutanova (Google AI) | Proposes masked language modeling (MLM) to achieve true bidirectional context understanding, establishing the “pre-training + fine-tuning” paradigm. | <https://aclanthology.org/N19-1423/> |
| ***Language Models are Few-Shot Learners*** | May 2020 | Tom B. Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah, Jared Kaplan, Prafulla Dhariwal, Arvind Neelakantan, Pranav Shyam, Girish Sastry, Amanda Askell, Sandhini Agarwal, Ariel Herbert-Voss, Gretchen Krueger, Tom Henighan, Rewon Child, Aditya Ramesh, Daniel M. Ziegler, Jeffrey Wu, Clemens Winter, Christopher Hesse, Mark Chen, Eric Sigler, Mateusz Litwin, Scott Gray, Benjamin Chess, Jack Clark, Christopher Berner, Sam McCandlish, Alec Radford, Ilya Sutskever, Dario Amodei (OpenAI) | Introduces the 175 billion parameter GPT-3, demonstrating competitiveness on various tasks through few-shot in-context learning. | <https://arxiv.org/abs/2005.14165> |
| ***Scaling Laws for Neural Language Models*** | 2020 | Jared Kaplan, Sam McCandlish, Tom Henighan, Tom B. Brown, Benjamin Chess, Rewon Child, Scott Gray, Alec Radford, Jeffrey Wu, Dario Amodei (OpenAI) | Systematically studies the power-law relationships between model performance and parameter count, dataset size, and compute. | <https://arxiv.org/abs/2001.08361> |
| ***Training Compute-Optimal Large Language Models*** | March 2022 | Jordan Hoffmann, Sebastian Borgeaud, Arthur Mensch, Elena Buchatskaya, Trevor Cai, Eliza Rutherford, Diego de Las Casas, Lisa Anne Hendricks, Johannes Welbl, Aidan Clark, Tom Hennigan, Eric Noland, Katie Millican, George van den Driessche, Bogdan Damoc, Aurelia Guy, Simon Osindero, Karen Simonyan, Erich Elsen, Jack W. Rae, Oriol Vinyals, Laurent Sifre (DeepMind) | Challenges the notion that “bigger is better,” proposing that model size and training data should be scaled together. | <https://arxiv.org/abs/2203.15556> |

## Human Alignment and RLHF

| Title | Publication Date | Author | Core Content | Link |
| ----- | ----- | ----- | ----- | ----- |
| ***Deep Reinforcement Learning from Human Preferences*** | June 2017 | Paul F. Christiano, Jan Leike, Tom B. Brown, Miljan Martic, Shane Legg, Dario Amodei (OpenAI) | Pioneers learning reward models from human preference comparisons for reinforcement learning training. | <https://arxiv.org/abs/1706.03741> |
| ***Training language models to follow instructions with human feedback*** | March 2022 | Long Ouyang, Jeff Wu, Xu Jiang, Diogo Almeida, Carroll L. Wainwright, Pamela Mishkin, Chong Zhang, Sandhini Agarwal, Katarina Slama, Alex Ray, John Schulman, Jacob Hilton, Fraser Kelton, Luke Miller, Maddie Simens, Amanda Askell, Peter Welinder, Paul Christiano, Jan Leike, Ryan Lowe (OpenAI) | Uses RLHF to train language models to better follow instructions, with InstructGPT achieving better performance despite smaller size. | <https://arxiv.org/abs/2203.02155> |
| ***Direct Preference Optimization: Your Language Model is Secretly a Reward Model*** | 2023 | Rafael Rafailov, Archit Sharma, Eric Mitchell, Stefano Ermon, Christopher D. Manning, Chelsea Finn (Stanford) | Proposes directly optimizing language models using preference data, eliminating the need for a separate reward model. | <https://arxiv.org/abs/2305.18290> |

## Prompting and Reasoning

| Title | Publication Date | Author | Core Content | Link |
| ----- | ----- | ----- | ----- | ----- |
| ***Chain-of-Thought Prompting Elicits Reasoning in Large Language Models*** | January 2022 | Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Brian Ichter, Fei Xia, Ed H. Chi, Quoc V. Le, Denny Zhou (Google Research) | Discovers that prompting models to output step-by-step reasoning chains dramatically improves accuracy on complex reasoning tasks. | <https://arxiv.org/abs/2201.11903> |
| ***Tree of Thoughts: Deliberate Problem Solving with Large Language Models*** | May 2023 | Shunyu Yao, Dian Yu, Jeffrey Zhao, Izhak Shafran, Thomas L. Griffiths, Yuan Cao, Karthik Narasimhan (Princeton, Google DeepMind) | Extends CoT into a tree of thoughts, allowing multiple reasoning paths and self-evaluation. | <https://arxiv.org/abs/2305.10601> |

## Open-Source Models

| Title | Publication Date | Author | Core Content | Link |
| ----- | ----- | ----- | ----- | ----- |
| ***LLaMA: Open and Efficient Foundation Language Models*** | February 2023 | Hugo Touvron, Thibaut Lavril, Gautier Izacard, Xavier Martinet, Marie-Anne Lachaux, Timothée Lacroix, Baptiste Rozière, Naman Goyal, Eric Hambro, Faisal Azhar, Aurelien Rodriguez, Armand Joulin, Edouard Grave, Guillaume Lample (Meta AI) | Releases open-source models ranging from 7B to 65B parameters, demonstrating that smaller models trained sufficiently can outperform larger ones. | <https://arxiv.org/abs/2302.13971> |

## Efficiency Optimization

| Title | Publication Date | Author | Core Content | Link |
| ----- | ----- | ----- | ----- | ----- |
| ***FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness*** | May 2022 | Tri Dao, Daniel Y. Fu, Stefano Ermon, Atri Rudra, Christopher Ré (Stanford) | Dramatically improves the speed and memory efficiency of attention computation through an IO-aware algorithm design. | <https://arxiv.org/abs/2205.14135> |

## Retrieval-Augmented Generation

| Title | Publication Date | Author | Core Content | Link |
| ----- | ----- | ----- | ----- | ----- |
| ***Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks*** | 2020 | Patrick Lewis, Ethan Perez, Aleksandra Piktus, Fabio Petroni, Vladimir Karpukhin, Naman Goyal, Heinrich Küttler, Mike Lewis, Wen-tau Yih, Tim Rocktäschel, Sebastian Riedel, Douwe Kiela (Facebook AI, UCL, NYU) | First proposes the RAG framework, combining parametric memory of pre-trained models with non-parametric retrieval memory. | <https://arxiv.org/abs/2005.11401> |

## Agents

| Title | Publication Date | Author | Core Content | Link |
| ----- | ----- | ----- | ----- | ----- |
| ***ReAct: Synergizing Reasoning and Acting in Language Models*** | October 2022 | Shunyu Yao, Jeffrey Zhao, Dian Yu, Nan Du, Izhak Shafran, Karthik Narasimhan, Yuan Cao (Princeton, Google Research) | Proposes an Agent framework synergizing reasoning and acting, solving complex tasks by interacting with external tools. | <https://arxiv.org/abs/2210.03629> |
| ***SWE-Bench: Can Language Models Resolve Real-World GitHub Issues?*** | October 2023 | Carlos E. Jimenez, John Yang, Alexander Wettig, Shunyu Yao, Kexin Pei, Ofir Press, Karthik R. Narasimhan (Princeton, Chicago) | Proposes a benchmark for evaluating the ability of LLMs to resolve real-world GitHub issues. | <https://arxiv.org/abs/2310.06770> |

## Multimodal

| Title | Publication Date | Author | Core Content | Link |
| ----- | ----- | ----- | ----- | ----- |
| ***GPT-4 Technical Report*** | March 2023 | OpenAI | Introduces the large-scale multimodal model GPT-4, demonstrating “human-level” performance on various benchmarks. | <https://arxiv.org/abs/2303.08774> |

## Surveys and Perspectives

| Title | Publication Date | Author | Core Content | Link |
| ----- | ----- | ----- | ----- | ----- |
| ***A Survey of Large Language Models*** | 2023 | Wayne Xin Zhao, Kun Zhou, Junyi Li, Tianyi Tang, Xiaolei Wang, Yupeng Hou, Yingqian Min, Beichen Zhang, Junjie Zhang, Zican Dong, Yifan Du, Chen Yang, Yushuo Chen, Zhipeng Chen, Jinhao Jiang, Ruiyang Ren, Yifan Li, Xinyu Tang, Zikang Liu, Peiyu Liu, Jian-Yun Nie, Ji-Rong Wen (Renmin University, Beijing) | Comprehensively reviews the development, technical architecture, and applications of large language models. | <https://arxiv.org/abs/2303.18223> |
| ***AI Alignment: A Comprehensive Survey*** | 2023 | Jiaming Ji, Tianyi Qiu, Boyuan Chen, Borong Zhang, Hantao Lou, Kaile Wang, Yawen Duan, Zhonghao He, Jiayi Zhou, Zhaowei Zhang, Fanzhi Zeng, Kwan Yee Ng, Juntao Dai, Xuehai Pan, Aidan O‘Gara, Yingshan Lei, Hua Xu, Brian Tse, Jie Fu, Stephen McAleer, Yaodong Yang, Yizhou Wang, Song-Chun Zhu, Yike Guo, Wen Gao (Peking University, Tsinghua, Cambridge, etc.) | Comprehensively surveys AI alignment techniques, including RLHF, Constitutional AI, and more. | <https://arxiv.org/abs/2310.19852> |
