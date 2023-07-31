# 20230731

##### Encouraging Divergent Thinking in Large Language Models through Multi-Agent Debate
```
Modern large language models (LLMs) like ChatGPT have shown remarkable performance on general language tasks but still struggle on complex reasoning tasks, which drives the research on cognitive behaviors of LLMs to explore human-like problem-solving strategies. Along this direction, one representative strategy is self-reflection, which asks an LLM to refine the solution with the feedback generated by itself iteratively. However, our study shows that such reflection-style methods suffer from the Degeneration-of-Thought (DoT) problem: once the LLM has established confidence in its solutions, it is unable to generate novel thoughts later through reflection even if its initial stance is incorrect. To address the DoT problem, we propose a Multi-Agent Debate (MAD) framework, in which multiple agents express their arguments in the state of"tit for tat"and a judge manages the debate process to obtain a final solution. Clearly, our MAD framework encourages divergent thinking in LLMs which would be helpful for tasks that require deep levels of contemplation. Experiment results on two challenging datasets, commonsense machine translation and counter-intuitive arithmetic reasoning, demonstrate the effectiveness of our MAD framework. Extensive analyses suggest that the adaptive break of debate and the modest level of"tit for tat"state are required for MAD to obtain good performance. Moreover, we find that LLMs might not be a fair judge if different LLMs are used for agents. Codes: https://github.com/Skytliang/Multi-Agents-Debate
```
一篇后处理的文章，感觉很不错，里面应该有前人self-reflection的文章，提出了思想退化（DoT）问题，提出了一个多主体辩论（MAD）框架，

沿着这个方向，一种有代表性的策略是自我反思，它要求LLM用自己迭代生成的反馈来完善解决方案。然而，我们的研究表明，这种反思式的方法存在思想退化（DoT）问题：一旦LLM对其解决方案建立了信心，即使其最初的立场不正确，它也无法在以后通过反思产生新的思想。为了解决DoT问题，我们提出了一个多主体辩论（MAD）框架，其中多个主体在“针锋相对”的状态下表达他们的论点，法官管理辩论过程以获得最终解决方案。显然，我们的MAD框架鼓励LLM中的发散思维，这将有助于完成需要深入思考的任务。



##### PEARL: Prompting Large Language Models to Plan and Execute Actions Over Long Documents
'''
Strategies such as chain-of-thought prompting improve the performance of large language models (LLMs) on complex reasoning tasks by decomposing input examples into intermediate steps. However, it remains unclear how to apply such methods to reason over long input documents, in which both the decomposition and the output of each intermediate step are non-trivial to obtain. In this work, we propose PEARL, a prompting framework to improve reasoning over long documents, which consists of three stages: action mining, plan formulation, and plan execution. More specifically, given a question about a long document, PEARL decomposes the question into a sequence of actions (e.g., SUMMARIZE, FIND_EVENT, FIND_RELATION) and then executes them over the document to obtain the answer. Each stage of PEARL is implemented via zero-shot or few-shot prompting of LLMs (in our work, GPT-4) with minimal human input. We evaluate PEARL on a challenging subset of the QuALITY dataset, which contains questions that require complex reasoning over long narrative texts. PEARL outperforms zero-shot and chain-of-thought prompting on this dataset, and ablation experiments show that each stage of PEARL is critical to its performance. Overall, PEARL is a first step towards leveraging LLMs to reason over long documents.
'''
针对长文档，设计了SUMMARIZE, FIND_EVENT, FIND_RELATION 动作完成推理。





# LLM_reasoner
调研与汇总大模型推理


[Is ChatGPT a Good Causal Reasoner? A Comprehensive Evaluation](https://arxiv.org/abs/2305.07375)
哈工大一篇推理ChatGPT推理能力的文章

Learning and Leveraging Verifiers to Improve Planning Capabilities of Pre-trained Language Models https://arxiv.org/abs/2305.17077

On the Computational Power of Decoder-Only Transformer Language Models https://arxiv.org/abs/2305.17026 计算能力

CombLM: Adapting Black-Box Language Models through Small Fine-Tuned Models https://arxiv.org/abs/2305.16876

Playing repeated games with Large Language Models https://arxiv.org/abs/2305.16867 博弈游戏

AdaPlanner: Adaptive Planning from Feedback with Language Models https://arxiv.org/abs/2305.16653 闭环

Language Models Can Improve Event Prediction by Few-Shot Abductive Reasoning https://arxiv.org/abs/2305.16646

Beyond Chain-of-Thought, Effective Graph-of-Thought Reasoning in Large Language Models https://arxiv.org/abs/2305.16582 COT

Decomposing the Enigma: Subgoal-based Demonstration Learning for Formal Theorem Proving https://arxiv.org/abs/2305.16366 定理证明

Leveraging LLMs for KPIs Retrieval from Hybrid Long-Document: A Comprehensive Framework and Dataset https://arxiv.org/abs/2305.16344 解析财务报告

OlaGPT: Empowering LLMs With Human-like Problem-Solving Abilities https://arxiv.org/abs/2305.16334

NavGPT: Explicit Reasoning in Vision-and-Language Navigation with Large Language Models https://arxiv.org/abs/2305.16986

Adaptive Chameleon or Stubborn Sloth: Unraveling the Behavior of Large Language Models in Knowledge Clashes https://arxiv.org/abs/2305.13300 知识冲突

Efficient Detection of LLM-generated Texts with a Bayesian Surrogate Model https://arxiv.org/abs/2305.16617 贝叶斯

# 外挂：
DKAF: KB Arbitration for Learning Task-Oriented Dialog Systems with Dialog-KB Inconsistencies https://arxiv.org/abs/2305.16697

On the Tool Manipulation Capability of Open-source Large Language Models https://arxiv.org/abs/2305.16504

Role-Play with Large Language Models https://arxiv.org/abs/2305.16367

Large Language Models as Tool Makers https://arxiv.org/abs/2305.17126

Chain of Knowledge: A Framework for Grounding Large Language Models with Structured Knowledge Bases https://arxiv.org/abs/2305.13269

# 其他大模型

PandaGPT: One Model To Instruction-Follow Them All https://arxiv.org/abs/2305.16355

RecurrentGPT: Interactive Generation of (Arbitrarily) Long Text https://arxiv.org/abs/2305.13304

# 决策
Think Before You Act: Decision Transformers with Internal Working Memory https://arxiv.org/abs/2305.16338

# 大小模型
Impossible Distillation: from Low-Quality Model to High-Quality Dataset & Model for Summarization and Paraphrasing https://arxiv.org/abs/2305.16635

# bias：
[Surfacing Biases in Large Language Models using Contrastive Input Decoding](https://arxiv.org/abs/2305.07378)

Large Language Models Are Partially Primed in Pronoun Interpretation https://arxiv.org/abs/2305.16917

# 多模态
BiomedGPT: A Unified and Generalist Biomedical Generative Pre-trained Transformer for Vision, Language, and Multimodal Tasks https://arxiv.org/pdf/2305.17100

# 生成负面陈述
Can large language models generate salient negative statements? https://arxiv.org/abs/2305.16755

# 跨语言泛化
Don't Trust GPT When Your Question Is Not In English https://arxiv.org/abs/2305.16339

How do languages influence each other? Studying cross-lingual data sharing during LLM fine-tuning https://arxiv.org/abs/2305.13286
