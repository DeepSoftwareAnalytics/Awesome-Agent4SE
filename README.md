# Agents in Software Engineering: Survey, Landscape, and Vision

In recent years, Large Language Models (LLMs) have achieved remarkable success and have been widely used in various downstream tasks, especially in the tasks of the software engineering (SE) field. We find that many studies combining LLMs with SE have employed the concept of agents either explicitly or implicitly. However, there is a lack of an in-depth survey to sort out the development context of existing works, analyze how existing works combine the LLM-based agent technologies to optimize various tasks and clarify the framework of LLM-based agents in SE. 
In this paper, we conduct the first survey of the studies on combining LLM-based agents with SE and present a framework of LLM-based agents in SE which includes three key modules: perception, memory, and action. We collected 115 related papers about LLM-based agents in SE and classified them. We also summarize the current challenges in combining the two fields and propose future opportunities in response to existing challenges. 

# Table of Contents
* [Perception](#-Perception)
  * [Textual Input](#Textual-Input)
    * [Token-based Input](#Token-based-Input)
    * [Tree/Graph-based Input](#ree/Graph-based-Input)
    * [Hybrid-based Input](#Hybrid-based-Input)
  * [Visual Input](#Visual-Input)
  * [Auditory Input](###Auditory-Input)
* [Memory](##-Memory))
  * [Semantic Memory](###Semantic-Memory)
  * [Episodic Memory](###Episodic-Memory)
  * [Procedural Memory](###Procedural-Memory)
    * [Implicit Knowledge](####Implicit-Knowledge)
    * [Explicit Knowledge](####Explicit-Knowledge)
* [Action](##-Action))
  * [Internal Actions](###Internal-Actions)
    * [Reasong Actions](####Reasong-Actions)
    * [Retrieval Actions](####Retrieval-Actions)
    * [Learning Actions](####Learning-Actions)
  * [External Actions](###External-Actions)
    * [Dialogue with Human/Agents](####Dialogue-with-Human/Agents)
    * [Digital Environments](####Digital-Environments)

# Agent in Software Engineering


## Perception

### Textual Input
#### Token-based Input
* [2022/12] **Prompting Is Programming: A Query Language for Large Language Models** *Beurer-Kellner et al. arXiv.* [[paper](https://arxiv.org/abs/2212.06094)]
* [2023/01] **Extending Source Code Pre-Trained Language Models to Summarise Decompiled Binaries** *Al-Kaswan et al. arXiv.* [[paper](https://arxiv.org/abs/2301.01701)]
* [2023/03] **Exploring Distributional Shifts in Large Language Models for Code Analysis** *Arakelyan et al. arXiv.* [[paper](https://arxiv.org/abs/2303.09128)]
* [2023/04] **Automatic Semantic Augmentation of Language Model Prompts (for Code Summarization)** *Ahmed et al. arXiv.* [[paper](https://arxiv.org/abs/2304.06815)]
* [2023/04] **Low Level Source Code Vulnerability Detection Using Advanced BERT Language Model** *Alqarni et al.* [[paper](https://assets.pubpub.org/bbi2k2lr/31652980468154.pdf)]   			
#### Tree/Graph-based Input
* [2023/03] **Evaluating and improving transformers pre-trained on ASTs for Code Completion** *Ochs et al. SANER* [[paper](https://ieeexplore.ieee.org/document/10123540)]
* [2023/05] **Neural Program Repair with Program Dependence Analysis and Effective Filter Mechanism** *Zhang et al. arXiv.* [[paper](https://arxiv.org/abs/2305.09315)]
* [2024/02] **The Scope of ChatGPT in Software Engineering: A Thorough Investigation** *Ma et al. arXiv.* [[paper](https://arxiv.org/abs/2305.12138v1)]

#### Hybrid-based Input

* [2022/08] **Tackling Long Code Search with Splitting, Encoding, and Aggregating** *Hu et al. ACL.* [[paper](https://arxiv.org/abs/2208.11271v3)]
* [2022/05] **SPT-Code: Sequence-to-Sequence Pre-Training for Learning Source Code Representations** *Niu et al. ICSE.* [[paper](https://arxiv.org/abs/2201.01549)]
* [2022/03] **UniXcoder: Unified Cross-Modal Pre-training for Code Representation** *Guo et al. ACL.* [[paper](https://arxiv.org/abs/2203.03850)]

<br/>

### Visual Input
* [2023/03] **PaLM-E: An Embodied Multimodal Language Model** *Driess et al. arXiv.* [[paper](https://arxiv.org/abs/2303.03378)]
* [2019/11] **User Interface Code Retrieval: A Novel Visual-Representation-Aware Approach** *Xie et al. IEEE Access.* [[paper](https://ieeexplore.ieee.org/document/8891747)]
* [2018/05] **GUIfetch: supporting app design and development through GUI search** *Behrang et al. ICSE.* [[paper](https://dl.acm.org/doi/10.1145/3197231.3197244)]
* [2014/09] **Seeking the user interface** *Reiss et al. ASE.* [[paper](https://dl.acm.org/doi/10.1145/2642937.2642976)]

<br/>

### Auditory Input
* [2020/06] **psc2code: Denoising Code Extraction from Programming Screencasts** *Bao et al. TOSEM.* [[paper](https://dl.acm.org/doi/10.1145/3392093)]

<br/>

## Memory
### Semantic Memory
* [2024/01] **Teaching Code LLMs to Use Autocompletion Tools in Repository-Level Code Generation** *Wang et al. arXiv.* [[paper](https://arxiv.org/pdf/2401.06391)]
* [2024/01] **CodeAgent: Enhancing Code Generation with Tool-Integrated Agent Systems for Real-World Repo-level Coding Challenges** *Zhang et al. arXiv.* [[paper](https://arxiv.org/abs/2401.07339)]
* [2024/01] **De-Hallucinator: Mitigating LLM Hallucinations in Code Generation Tasks via Iterative Grounding** *Eghbali et al. arXiv.* [[paper](https://arxiv.org/pdf/2401.01701)]
* [2023/11] **Evaluating In-Context Learning of Libraries for Code Generation** *Patel et al. arXiv.* [[paper](https://arxiv.org/pdf/2311.09635)]
* [2022/07] **DocPrompting: Generating Code by Retrieving the Docs** *Zhou et al. arXiv.* [[paper](https://arxiv.org/abs/2207.05987)]
* [2023/09] **From Misuse to Mastery: Enhancing Code Generation with Knowledge-Driven AI Chaining** *Ren et al. ASE.* [[paper](https://arxiv.org/abs/2309.15606)]
* [2023/05] **ToolCoder: Teach Code Generation Models to use API search tools** *Zhang et al. arXiv.* [[paper](https://arxiv.org/abs/2305.04032)]
* [2023/04] **Automatic Semantic Augmentation of Language Model Prompts (for Code Summarization)** *Ahmed et al. arXiv.* [[paper](https://arxiv.org/abs/2304.06815)]

<br/>
  
### Episodic Memory
* [2024/01] **De-Hallucinator: Mitigating LLM Hallucinations in Code Generation Tasks via Iterative Grounding** *Eghbali et al. arXiv.* [[paper](https://arxiv.org/pdf/2401.01701)]
* [2023/09] **Copiloting the Copilots: Fusing Large Language Models with Completion Engines for Automated Program Repair** *Wei et al. ESEC/FSE.* [[paper](https://arxiv.org/pdf/2309.00608)]
* [2023/07] **Multilingual Code Co-Evolution Using Large Language Models** *Zhang et al. ESEC/FSE.* [[paper](https://arxiv.org/pdf/2307.14991)]
* [2023/06] **Prompting Is All You Need: Automated Android Bug Replay with Large Language Models** *Feng et al. ICSE.* [[paper](https://arxiv.org/abs/2306.01987)]
* [2023/05] **COEDITOR: LEVERAGING REPO-LEVEL DIFFS FOR CODE AUTO-EDITING** *Wei et al. arXiv.* [[paper](https://arxiv.org/pdf/2305.18584)]
* [2023/04] **Automatic Semantic Augmentation of Language Model Prompts (for Code Summarization)** *Ahmed et al. arXiv.* [[paper](https://arxiv.org/abs/2304.06815)]
* [2023/03] **RepoCoder: Repository-Level Code Completion Through Iterative Retrieval and Generation** *Zhang et al. arXiv.* [[paper](https://arxiv.org/pdf/2303.12570)]
* [2023/03] **AceCoder: Utilizing Existing Code to Enhance Code Generation** *Li et al. arXiv.* [[paper](https://arxiv.org/abs/2303.17780)]

<br/>

### Procedural Memory
#### Implicit Knowledge
* [2024/01] **DeepSeek-Coder: When the Large Language Model Meets Programming - The Rise of Code Intelligence** *Guo et al. arXiv.* [[paper](https://arxiv.org/pdf/2401.14196)]
* [2024/01] **Mutation-based Consistency Testing for Evaluating the Code Understanding Capability of LLMs** *Li et al. ICSE.* [[paper](https://arxiv.org/abs/2401.05940)]
* [2023/12] **Traces of Memorisation in Large Language Models for Code** *Al-Kaswan et al. arXiv.* [[paper](https://arxiv.org/abs/2312.11658)]
* [2023/12] **Competition-Level Problems are Effective LLM Evaluators** *Huang et al. arXiv.* [[paper](https://arxiv.org/pdf/2312.02143)]
* [2023/11] **A Survey of Large Language Models for Code: Evolution, Benchmarking, and Future Trends** *Zheng et al. arXiv.* [[paper](https://arxiv.org/abs/2311.10372)]
* [2023/11] **Unifying the Perspectives of NLP and Software Engineering: A Survey on Language Models for Code** *Zhang et al. arXiv.* [[paper](https://arxiv.org/abs/2311.07989)]
* [2023/10] **Gotcha! This Model Uses My Code! Evaluating Membership Leakage Risks in Code Models** *Yang et al. arXiv.* [[paper](https://arxiv.org/abs/2310.01166)]
* [2023/10] **CodeFuse-13B: A Pretrained Multi-lingual Code Large Language Model** *Di et al. ICSE-SEIP.* [[paper](https://arxiv.org/abs/2310.06266)]
* [2023/10] **Beyond Accuracy: Evaluating Self-Consistency of Code Large Language Models with IdentityChain** *Min et al. ICLR.* [[paper](https://arxiv.org/abs/2310.14053)]
* [2023/10] **Personalised Distillation: Empowering Open-Sourced LLMs with Adaptive Learning for Code Generation** *Chen et al. EMNLP.* [[paper](https://arxiv.org/abs/2310.18628)]
* [2023/09] **Textbooks Are All You Need II: phi-1.5 technical report** *Li et al. arXiv.* [[paper](https://arxiv.org/abs/2309.05463)]
* [2023/08] **Can ChatGPT replace StackOverflow? A Study on Robustness and Reliability of Large Language Model Code Generation** *Zhong et al. arXiv.* [[paper](https://arxiv.org/abs/2308.10335)]
* [2023/08] **Code Llama: Open Foundation Models for Code** *Rozière et al. arXiv.* [[paper](https://arxiv.org/abs/2308.12950)]
* [2023/08] **Unveiling Memorization in Code Models** *Yang et al. ICSE.* [[paper](https://arxiv.org/abs/2308.09932)]
* [2023/07] **PanGu-Coder2: Boosting Large Language Models for Code with Ranking Feedback** *Shen et al. arXiv.* [[paper](https://arxiv.org/abs/2307.14936)]
* [2023/06] **Textbooks Are All You Need** *Gunasekar et al. arXiv.* [[paper](https://arxiv.org/abs/2306.11644)]
* [2023/06] **CodeTF: One-stop Transformer Library for State-of-the-art Code LLM** *Bui et al. arXiv.* [[paper](https://arxiv.org/abs/2306.00029)]
* [2023/05] **StarCoder: may the source be with you!** *Li et al. arXiv.* [[paper](https://arxiv.org/abs/2305.06161)]
* [2023/05] **CodeT5+: Open Code Large Language Models for Code Understanding and Generation** *Wang et al. arXiv.* [[paper](https://arxiv.org/abs/2305.07922)]
* [2023/05] **CodeIE: Large Code Generation Models are Better Few-Shot Information Extractors** *Li et al. ACL.* [[paper](https://arxiv.org/abs/2305.05711)]
* [2023/04] **WizardLM: Empowering Large Language Models to Follow Complex Instructions** *Xu et al. arXiv.* [[paper](https://arxiv.org/abs/2304.12244)]
* [2023/03] **CodeGeeX: A Pre-Trained Model for Code Generation with Multilingual Benchmarking on HumanEval-X** *Zheng et al. arXiv.* [[paper](https://arxiv.org/abs/2303.17568)]
* [2022/12] **MultiCoder: Multi-Programming-Lingual Pre-Training for Low-Resource Code Completion** *Gong et al. arXiv.* [[paper](https://arxiv.org/abs/2212.09666)]
* [2022/07] **PanGu-Coder: Program Synthesis with Function-Level Language Modeling** *Christopoulou et al. arXiv.* [[paper](https://arxiv.org/abs/2207.11280)]
* [2022/03] **CERT: Continual Pre-training on Sketches for Library-oriented Code Generation** *Zan et al. IJCAI.* [[paper](https://www.ijcai.org/proceedings/2022/329)]
* [2022/01] **Training and Evaluating a Jupyter Notebook Data Science Assistant** *Chandel et al. arXiv.* [[paper](https://arxiv.org/abs/2201.12901)]
* [2022/01] **LaMDA: Language Models for Dialog Applications** *Thoppilan et al. arXiv.* [[paper](https://arxiv.org/abs/2201.08239)]

#### Explicit Knowledge
* [2023/11] **Evaluating In-Context Learning of Libraries for Code Generation** *Patel et al. arXiv.* [[paper](https://arxiv.org/pdf/2311.09635)]
* [2023/10] **Prompt Engineering or Fine Tuning: An Empirical Assessment of Large Language Models in Automated Software Engineering Tasks** *Shin et al. arXiv.* [[paper](https://arxiv.org/abs/2310.10508)]
* [2023/08] **Prompt-Enhanced Software Vulnerability Detection Using ChatGPT** *Zhang et al. ICSE.* [[paper](https://arxiv.org/abs/2308.12697)]

<br/>

## Action

###  Internal Actions

#### Reasoning Actions
* [2024/01] **Teaching Code LLMs to Use Autocompletion Tools in Repository-Level Code Generation** *Wang et al. arXiv.* [[paper](https://arxiv.org/pdf/2401.06391)]
* [2024/01] **Leveraging Print Debugging to Improve Code Generation in Large Language Models** *Hu et al. arXiv.* [[paper](https://arxiv.org/abs/2401.05319)]
* [2023/12] **Chain-of-Thought in Neural Code Generation: From and For Lightweight Language Models** *Yang et al. TSE.* [[paper](https://arxiv.org/abs/2312.05562)]
* [2023/12] **Pangu-Agent: A Fine-Tunable Generalist Agent with Structured Reasoning** *Christianos et al. arXiv.* [[paper](https://arxiv.org/abs/2312.14878)]
* [2023/12] **Enhancing Exploratory Testing by Large Language Model and Knowledge Graph** *Su et al. ICSE.* [[paper](https://dl.acm.org/doi/abs/10.1145/3597503.3639157)]
* [2023/10] **CodeChain: Towards Modular Code Generation Through Chain of Self-revisions with Representative Sub-modules** *Le et al. ICLR.* [[paper](https://arxiv.org/abs/2310.08992)]
* [2023/10] **ClarifyGPT: Empowering LLM-based Code Generation with Intention Clarification** *Mu et al. arXiv.* [[paper](https://arxiv.org/abs/2310.10996)]
* [2023/09] **CodePlan: Repository-level Coding using LLMs and Planning** *Bairi et al. arXiv.* [[paper](https://arxiv.org/abs/2309.12499)]
* [2023/09] **Draft & Verify: Lossless Large Language Model Acceleration via Self-Speculative Decoding** *Zhang et al. ACL.* [[paper](https://arxiv.org/abs/2309.08168)]
* [2023/09] **Test-Case-Driven Programming Understanding in Large Language Models for Better Code Generation** *Tian et al. arXiv.* [[paper](https://browse.arxiv.org/pdf/2309.16120)]
* [2023/08] **CodeCoT: Tackling Code Syntax Errors in CoT Reasoning for Code Generation** *Huang et al. arXiv.* [[paper](https://arxiv.org/abs/2308.08784)]
* [2023/06] **Prompting Is All You Need: Automated Android Bug Replay with Large Language Models** *Feng et al. ICSE.* [[paper](https://arxiv.org/abs/2306.01987)]
* [2023/05] **Structured Chain-of-Thought Prompting for Code Generation** *Li et al. arXiv.* [[paper](https://arxiv.org/abs/2305.06599)]
* [2023/05] **Think Outside the Code: Brainstorming Boosts Large Language Models in Code Generation** *Li et al. arXiv.* [[paper](https://arxiv.org/abs/2305.10679)]
* [2023/03] **Self-planning Code Generation with Large Language Models** *Jiang et al. TOSEM.* [[paper](https://arxiv.org/abs/2303.06689)]




#### Retrieval Actions
* [2024/01] **CodeAgent: Enhancing Code Generation with Tool-Integrated Agent Systems for Real-World Repo-level Coding Challenges** *Zhang et al. arXiv.* [[paper](https://arxiv.org/abs/2401.07339)]
* [2024/01] **De-Hallucinator: Mitigating LLM Hallucinations in Code Generation Tasks via Iterative Grounding** *Eghbali et al. arXiv.* [[paper](https://arxiv.org/pdf/2401.01701)]
* [2023/10] **When Language Model Meets Private Library** *Zan et al. EMNLP.* [[paper](https://arxiv.org/abs/2210.17236)]
* [2023/10] **Large Language Model-Aware In-Context Learning for Code Generation** *Li et al. arXiv.* [[paper](https://arxiv.org/abs/2310.09748)]
* [2023/06] **epoFusion: Training Code Models to Understand Your Repository** *Shrivastava et al. arXiv.* [[paper](https://arxiv.org/abs/2306.10998)]
* [2023/05] **Retrieval-Based Prompt Selection for Code-Related Few-Shot Learning** *Nashid et al. ICSE.* [[paper](https://ieeexplore.ieee.org/abstract/document/10172590)]
* [2023/05] **ToolCoder: Teach Code Generation Models to use API search tools** *Zhang et al. arXiv.* [[paper](https://arxiv.org/abs/2305.04032)]
* [2023/04] **Large Language Models are Few-Shot Summarizers: Multi-Intent Comment Generation via In-Context Learning** *Geng et al. ICSE.* [[paper](https://arxiv.org/abs/2304.11384)]
* [2023/03] **RepoCoder: Repository-Level Code Completion Through Iterative Retrieval and Generation** *Zhang et al. arXiv.* [[paper](https://arxiv.org/pdf/2303.12570)]
* [2023/03] **AceCoder: Utilizing Existing Code to Enhance Code Generation** *Li et al. arXiv.* [[paper](https://arxiv.org/abs/2303.17780)]
* [2022/12] **Generation-Augmented Query Expansion For Code Retrieval** *Li et al. arXiv.* [[paper](https://arxiv.org/abs/2212.10692)]
* [2022/07] **DocPrompting: Generating Code by Retrieving the Docs** *Zhou et al. ICLR.* [[paper](https://arxiv.org/abs/2207.05987)]








#### Learning Actions

*Updating Semantic Memory with Knowledge*

* [2024/06] **Vul-RAG: Enhancing LLM-based Vulnerability Detection via Knowledge-level RAG** *Du et al. arXiv.* [[paper](https://arxiv.org/abs/2406.11147)]
* [2023/12] **A3-CodGen: A Repository-Level Code Generation Framework for Code Reuse with Local-Aware, Global-Aware, and Third-Party-Library-Aware** *Liao et al. arXiv.* [[paper](https://arxiv.org/pdf/2312.05772)]

*Updating Implicit Knowledge*
* [2023/12] **Magicoder: Empowering Code Generation with OSS-INSTRUCT** *Wei et al. PMLR.* [[paper](https://arxiv.org/pdf/2312.02120)]
* [2023/10] **Prompt Engineering or Fine Tuning: An Empirical Assessment of Large Language Models in Automated Software Engineering Tasks** *Shin et al. arXiv.* [[paper](https://arxiv.org/abs/2310.10508)]
* [2023/10] **Improving Code Style for Accurate Code Generation** *Jain et al. NeurIPS Workshop.* [[paper](https://openreview.net/pdf?id=uc9sYHRX6O)]
* [2023/10] **Large Language Models for Test-Free Fault Localization** *Yang et al. arXiv.* [[paper](https://arxiv.org/abs/2310.01726)]
* [2023/09] **An Empirical Study on Fine-Tuning Large Language Models of Code for Automated Program Repair** *Huang et al. ASE.* [[paper](https://ieeexplore.ieee.org/document/10298532)]
* [2023/08] **VeriGen: A Large Language Model for Verilog Code Generation** *Thakur et al. arXiv.* [[paper](https://arxiv.org/abs/2308.00708)]
* [2023/08] **Exploring Parameter-Efficient Fine-Tuning Techniques for Code Generation with Large Language Models** *Weyssow et al. arXiv.* [[paper](https://arxiv.org/abs/2308.10462)]
* [2023/07] **Multilingual Code Co-Evolution Using Large Language Models** *Zhang et al. ESEC/FSE.* [[paper](https://arxiv.org/pdf/2307.14991)]
* [2023/06] **WizardCoder: Empowering Code Large Language Models with Evol-Instruct** *Luo et al. arXiv.* [[paper](https://arxiv.org/abs/2306.08568)]
* [2023/05] **COEDITOR: LEVERAGING REPO-LEVEL DIFFS FOR CODE AUTO-EDITING** *Wei et al. arXiv.* [[paper](https://arxiv.org/pdf/2305.18584)]
* [2023/05] **Coarse-Tuning Models of Code with Reinforcement Learning Feedback** *Jain et al. arXiv.* [[paper](https://arxiv.org/abs/2305.18341)]
* [2023/03] **Revisiting the Plastic Surgery Hypothesis via Large Language Models** *Xia et al. arXiv.* [[paper](https://arxiv.org/abs/2303.10494)]
* [2023/03] **One Adapter for All Programming Languages? Adapter Tuning for Code Search and Summarization** *Wang et al. arXiv.* [[paper](https://arxiv.org/pdf/2303.15822v1)]

*Updating Agent Code*
* [2023/10] **InstructCoder: Instruction Tuning Large Language Models for Code Editing** *Li et al. arXiv.* [[paper](https://arxiv.org/abs/2310.20329)]
* [2023/08] **OctoPack: Instruction Tuning Code Large Language Models** *Muennighoff et al. arXiv.* [[paper](https://arxiv.org/abs/2308.07124)]
* [2023/08] **Can Programming Languages Boost Each Other via Instruction Tuning?** *Zan et al. arXiv.* [[paper](https://arxiv.org/abs/2308.16824)]
* [2023/05] **CodeIE: Large Code Generation Models are Better Few-Shot Information Extractors** *Li et al. ACL.* [[paper](https://arxiv.org/abs/2305.05711)]
* [2022/12] **Self-Adaptive In-Context Learning: An Information Compression Perspective for In-Context Example Selection and Ordering** *Wu et al. ACL.* [[paper](https://arxiv.org/abs/2212.10375)]

<br/>

### External Actions

#### Dialogue with Human/Agents
* [2023/12] **Supervised Knowledge Makes Large Language Models Better In-context Learners** *Yang et al. ICLR.* [[paper](https://arxiv.org/abs/2312.15918)]
* [2023/12] **AgentCoder: Multi-Agent Code Generation with Effective Testing and Self-optimisation** *Huang et al. arXiv.* [[paper](https://arxiv.org/pdf/2312.13010)]
* [2023/11] **Coffee: Boost Your Code LLMs by Fixing Bugs with Feedback** *Moon et al. arXiv.* [[paper](https://arxiv.org/abs/2311.07215)]
* [2023/11] **Functional Overlap Reranking for Neural Code Generation** *To et al. arXiv.* [[paper](https://arxiv.org/pdf/2311.03366)]
* [2023/11] **ChatCoder: Chat-based Refine Requirement Improves LLMs' Code Generation** *Wang et al. arXiv.* [[paper](https://arxiv.org/abs/2311.00272)]
* [2023/10] **Clover: Closed-Loop Verifiable Code Generation** *Sun et al. arXiv.* [[paper](https://arxiv.org/abs/2310.17807)]
* [2023/10] **ClarifyGPT: Empowering LLM-based Code Generation with Intention Clarification** *Mu et al. arXiv.* [[paper](https://arxiv.org/abs/2310.10996)]
* [2023/09] **Exploring the Potential of Large Language Models to Generate Formative Programming Feedback** *Kiesler et al. FIE.* [[paper](https://arxiv.org/abs/2309.00029)]
* [2023/09] **Copiloting the Copilots: Fusing Large Language Models with Completion Engines for Automated Program Repair** *Wei et al. ESEC/FSE.* [[paper](https://arxiv.org/pdf/2309.00608)]
* [2023/09] **MINT: Evaluating LLMs in Multi-turn Interaction with Tools and Language Feedback** *Wang et al. arXiv.* [[paper](https://arxiv.org/abs/2309.10691)]
* [2023/09] **Exploring the Potential of ChatGPT in Automated Code Refinement: An Empirical Study** *Guo et al. arXiv.* [[paper](https://arxiv.org/abs/2309.08221)]
* [2023/08] **MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework** *Hong et al. arXiv.* [[paper](https://arxiv.org/abs/2308.00352)]
* [2023/07] **RLTF: Reinforcement Learning from Unit Test Feedback** *Liu et al. TMLR.* [[paper](https://arxiv.org/abs/2307.04349)]
* [2023/05] **Coarse-Tuning Models of Code with Reinforcement Learning Feedback** *Jain et al. arXiv.* [[paper](https://arxiv.org/abs/2305.18341)]
* [2023/04] **REFINER: Reasoning Feedback on Intermediate Representations** *Paul et al. EACL.* [[paper](https://arxiv.org/abs/2304.01904)]
* [2023/03] **Reflexion: Language Agents with Verbal Reinforcement Learning** *Shinn et al. arXiv.* [[paper](https://arxiv.org/abs/2303.11366)]
* [2023/03] **Self-Refine: Iterative Refinement with Self-Feedback** *Madaan et al. arXiv.* [[paper](https://arxiv.org/abs/2303.17651)]
* [2023/01] **Execution-based Code Generation using Deep Reinforcement Learning** *Shojaee et al. TMLR.* [[paper](https://arxiv.org/abs/2301.13816)]

#### Digital Environments

* [2024/01] **CodeAgent: Enhancing Code Generation with Tool-Integrated Agent Systems for Real-World Repo-level Coding Challenges** *Zhang et al. arXiv.* [[paper](https://arxiv.org/abs/2401.07339)]
* [2024/01] **Teaching Code LLMs to Use Autocompletion Tools in Repository-Level Code Generation** *Wang et al. arXiv.* [[paper](https://arxiv.org/pdf/2401.06391)]
* [2023/09] **Copiloting the Copilots: Fusing Large Language Models with Completion Engines for Automated Program Repair** *Wei et al. ESEC/FSE.* [[paper](https://arxiv.org/pdf/2309.00608)]
* [2023/09] **MINT: Evaluating LLMs in Multi-turn Interaction with Tools and Language Feedback** *Wang et al. arXiv.* [[paper](https://arxiv.org/abs/2309.10691)]
* [2023/07] **RLTF: Reinforcement Learning from Unit Test Feedback** *Liu et al. TMLR.* [[paper](https://arxiv.org/abs/2307.04349)]
* [2023/06] **Guiding Language Models of Code with Global Context using Monitors** *Agrawal et al. arXiv.* [[paper](https://arxiv.org/pdf/2306.10763)]
* [2023/05] **Coarse-Tuning Models of Code with Reinforcement Learning Feedback** *Jain et al. arXiv.* [[paper](https://arxiv.org/abs/2305.18341)]
* [2023/05] **Self-Edit: Fault-Aware Code Editor for Code Generation** *Zhang et al. ACL.* [[paper](https://arxiv.org/abs/2305.04087)]
* [2023/01] **Execution-based Code Generation using Deep Reinforcement Learning** *Shojaee et al. TMLR.* [[paper](https://arxiv.org/abs/2301.13816)]
* [2022/03] **Compilable Neural Code Generation with Compiler Feedback** *Wang et al. ACL.* [[paper](https://arxiv.org/abs/2203.05132)]
