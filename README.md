# A Comprehensive Survey of LLM-Driven Collective Intelligence: Past, Present, and Future
Collective intelligence (CI) has emerged as a cornerstone for advancing toward Artificial General Intelligence (AGI), with Large Language Models (LLMs) now serving as the primary driver. In this study, we present the first systematic framework to characterize the evolutionary trajectory of CI, and conduct a review of the role of LLMs in driving CI. Historically, CI went through two phases: the initial Collective Intelligence 1.0 Era ("Collective but Unintelligent") introduces various bio-inspired algorithms which demonstrates emergent behaviors but no true cognitive capabilities, while the subsequent Collective Intelligence 2.0 Era ("Specialized yet Disconnected") achieves domain-specific expertise within multi-agent systems but remained isolated across applications. Currently, Collective Intelligence 3.0 Era ("Collectively to Enhance Intelligence") is being shaped by LLMs, with remarkable breakthroughs achieved in both foundation-oriented and application-oriented researches. At the foundational level, by enhancing data, model, and the reasoning process, LLMdriven CI has made remarkable progress in terms of performance optimization, efficiency improvement, and enhancement of robustness and security. In applications, LLM-driven CI excels in complex, long-horizon tasks, such as scientific discovery and autonomous research, delivering innovative solutions to real-world problems. In the future, in order to solve more intricate and even unexplored real-world tasks and scenarios, there is an urgent necessity to transition to Collective Intelligence 4.0 Era ("Collectively to Create Intelligence"). To achieve this, the following aspects can be considered including fundamental capability construction, capability differentiation, cognitive fusion, dynamic organization, and co-evolution, and several challenges such as unclear emergence mechanisms, bottlenecks in continuous learning, interoperability issues among systems , and high demand for computational resources should be solved. The collaborative efforts of the research communities are expected to accelerate the maturation of LLM-driven CI, create immense value for society and drive leapfrog development across various fields, and steadily march towards the AGI goal.

> 📚 A curated list of awesome resources for **Collective Intelligence/Multi-Agent System**.

![GitHub Repo stars](https://img.shields.io/github/stars/d-andelions/awesome-LLM-Driven-Collective-Intelligence?color=yellow&cacheSeconds=60)
![GitHub forks](https://img.shields.io/github/forks/d-andelions/awesome-LLM-Driven-Collective-Intelligence?color=lightblue)
![GitHub last commit](https://img.shields.io/github/last-commit/d-andelions/awesome-LLM-Driven-Collective-Intelligence?color=green)
<!-- <a href="https://arxiv.org/abs/2509.02350" target="_blank"><img src="https://img.shields.io/badge/arXiv-2509.02350-009688.svg" alt="arXiv" /></a> -->

## 📂 Contents
> 
- [Evolution of Collective Intelligence](#evolution-of-collective-intelligence)
- [Key Techniques of Large Language Models](#key-techniques-of-large-language-models)
  - [Pre-Training](#pre-training)
  - [Supervised Fine-Tuning(SFT)](#supervised-fine-tuning(SFT))
  - [Human Preference Alignment](#human-preference-alignment)
  - [Prompt Engineering](#prompt-engineering)
  - [Tool Use](#tool-use)
  - [Memory Mechanism](#memory-mechanism)
  - [Parameter-Efficient Fine-Tuning (PEFT)](#parameter-efficient-fine-tuning-(PEFT))
  - [LLM-Based Agents](#llm-based-agents)
- [LLM-based Collective Intelligence](#llm-based-collective-intelligence)
- [Collective Intelligence 1.0 and 2.0 Era](#collective-intelligence-1.0-and-2.0-era)
  - [Collective Intelligence 1.0 Era](#collective-intelligence-1.0-era)
  - [Collective Intelligence 2.0 Era](#collective-intelligence-2.0-era)
- [Collective Intelligence 3.0 Era](#application-oriented-ci)
  - [Data-Level Enhancement](#data-level-enhancement)
     - [Same LLM Driven](#Same-LLM-Driven)
     - [Different LLM Driven](#Different-LLM-Driven)
  - [Model-Level Enhancement](#model-level-enhancement)
     - [Model Routing](#Model-Routing)
     - [Model Merging](#Model-Merging)
     - [Model Ensemble](#Model-Ensemble)
  - [Inference-Level Enhancement](#inference-level-enhancement)
     - [Self-driven Enhancement](#Self-driven-Enhancement)
     - [Cooperation-driven Enhancement](#Cooperation-driven-Enhancement)
     - [Competition-involved Enhancement](#Competition-involved-Enhancement)
     - [Self-Organizing Collective Optimization](#Self-Organizing-Collective-Optimization)
- [LLM Driven Application-Oriented Collective Intelligence](#LLM-Driven-Application-Oriented-Collective-Intelligence)
  - [Scientific Discovery and Autonomous Research](#Scientific-Discovery-and-Autonomous-Research)
     - [Scientific Discovery](#Scientific-Discovery)
     - [Autonomous Research](#Autonomous-Research)
  - [Embodied Intelligence Research](#Embodied-Intelligence-Research)
     - [Centralized Control Paradigm](#Centralized-Control-Paradigm)
     - [Decentralized Interactive Paradigm](#Decentralized-Interactive-Paradigm)
  - [Social Science Research](#Social-Science-Research)
     - [Scope of Simulation](#Scope-of-Simulation)
     - [Application of Simulation](#Application-of-Simulation)
  - [Auto-Programming](#Auto-Programming)
     - [Foundation-Oriented Programming](#Foundation-Oriented-Programming)
     - [Application-Oriented Programming](#Application-Oriented-Programming)
  - [GUI Operations](#GUI-Operations)
     - [Prompting-Based Methods](#Prompting-Based-Methods)
     - [Tuning-Based Methods](#Tuning-Based-Methods)
  - [Game Theory and Interactive Games](#Game-Theory-and-Interactive-Games)
     - [Application in Game Theory](#Application-in-Game-Theory)
     - [Application in Interactive Games](#Application-in-Interactive-Games)
- [Collective Intelligence 4.0 Era](#future-challenges)

## 🧬Evolution of Collective Intelligence
![CI Framework](https://github.com/d-andelions/awesome-LLM-Driven-Collective-Intelligence/blob/main/figs/1.png)
The **Collective Intelligence 1.0 Era** established the core principles of emergent group behavior through bio-inspired algorithms. Early works have demonstrated that complex group behaviors can emerge from simple interaction rules.

The **Collective Intelligence 2.0 Era** marked a significant advancement through the development of specialized multi-agent architectures. Researches on adaptive coordination mechanisms and hybrid collective algorithms enabled more sophisticated collaborative capabilities.

Currently, we are witnessing the emergence and popularity of the **Collective Intelligence 3.0 Era**, where breakthroughs in Large Language Models (LLMs) are revolutionizing the collective intelligence field. Generally, these LLM-powered entities will achieve collective intelligence from the following unique perspectives: 
> 1. the LLM perspective, which investigates how collaboration at various levels enhances the models themselves; 
> 2. the collective-intelligence perspective, which analyzes the composition of participating entities and the nature of their interactions. Driven by LLMs, it is capable of productively yield the effect denoted by _Collectively to Enhance Intelligence_.

In the future, as artificial intelligence continues to progress, it will encounter more intricate and even unexplored real-world tasks and scenarios. Thus, there is an urgent necessity to transition to the **Collective Intelligence 4.0 Era**, whose core is the establishment of a novel paradigm known as _Collectively to Create Intelligence_."

## 📘Key Techniques of Large Language Models
**Pre-Training:** Pre-training serves as the foundational stage in LLM development, where models acquire general language understanding capabilities by predicting the next token from massive unlabeled text corpora.
> A Law of Next-Token Prediction in Large Language Models <a href="https://arxiv.org/abs/2408.13442"><img src="https://img.shields.io/badge/arXiv-2408.13442-009688.svg" alt="arXiv" /></a> <br>
> Efficient training of language models with compact and consistent next token distributions <a href="https://arxiv.org/abs/2407.02819"><img src="https://img.shields.io/badge/arXiv-2407.02819-009688.svg" alt="arXiv" /></a> <br>
> Better & faster large language models via multi-token prediction <a href="https://arxiv.org/abs/2404.19737"><img src="https://img.shields.io/badge/arXiv-2404.19737-009688.svg" alt="arXiv" /></a> <br>
> A clip-powered framework for robust and generalizable data selection <a href="https://arxiv.org/abs/2410.11215"><img src="https://img.shields.io/badge/arXiv-2410.11215-009688.svg" alt="arXiv" /></a> <br>

**Supervised Fine-Tuning(SFT):** SFT is a pivotal post-training stage that refines pre-trained LLMs to enhance task-specific performance or instruction-following capabilities.
> Scaling instructionfinetuned language models <a href="https://arxiv.org/abs/2210.11416"><img src="https://img.shields.io/badge/arXiv-2210.11416-009688.svg" alt="arXiv" /></a> <br>
> Language models are few-shot learners <a href="https://arxiv.org/abs/2005.14165"><img src="https://img.shields.io/badge/arXiv-2005.14165-009688.svg" alt="arXiv" /></a> <br>

**Human Preference Alignment:** Human Preference Alignment addresses the critical challenge of ensuring LLMs produce outputs that align with human ethics, preferences, and safety standards.
> Deep reinforcement learning from human preferences <a href="https://arxiv.org/abs/1706.03741"><img src="https://img.shields.io/badge/arXiv-1706.03741-009688.svg" alt="arXiv" /></a> <br>
> Direct preference optimization: Your language model is secretly a reward model <a href="https://arxiv.org/abs/2305.18290v3"><img src="https://img.shields.io/badge/arXiv-2305.18290v3-009688.svg" alt="arXiv" /></a> <br>
> Proximal policy optimization algorithms <a href="https://arxiv.org/abs/1707.06347"><img src="https://img.shields.io/badge/arXiv-1707.06347-009688.svg" alt="arXiv" /></a> <br>

**Prompt Engineering:** By designing input text (prompts), it guides LLMs to produce desired responses, leveraging the model’s contextual understanding. To activate task-specific reasoning paths, a series of prompt optimization frameworks is proposed.
> Openprompt: An open-source framework for prompt-learning [![arXiv](https://img.shields.io/badge/arXiv-1707.06347-009688.svg)](https://arxiv.org/abs/1707.06347) <br>
> Active prompting with chain-of-thought for large language models [![arXiv](https://img.shields.io/badge/arXiv-2302.12246-009688.svg)](https://arxiv.org/abs/2302.12246) <br>
> Chain-of-thought prompting elicits reasoning in large language models [![arXiv](https://img.shields.io/badge/arXiv-2201.11903-009688.svg)](https://arxiv.org/abs/2201.11903) <br>
> Towards understanding chain-of-thought prompting: An empirical study of what matters [![arXiv](https://img.shields.io/badge/arXiv-2212.10001-009688.svg)](https://arxiv.org/abs/2212.10001) <br>
> Tree of thoughts: Deliberate problem solving with large language models [![arXiv](https://img.shields.io/badge/arXiv-2212.10001-009688.svg)](https://arxiv.org/abs/2212.10001) <br>

**Tool Use:** Tool use refers to techniques that enable LLMs to use external tools.
> Tool learning with large language models: A survey [![arXiv](https://img.shields.io/badge/arXiv-2405.17935-009688.svg)](https://arxiv.org/abs/2405.17935) <br>

**Memory Mechanism:** The memory mechanism in LLMs refers to the framework designed to accumulate knowledge, process historical information, and retrieve relevant context to support decision-making and response generation, mimicking human cognitive memory functions.
> Training language models with memory augmentation [![arXiv](https://img.shields.io/badge/arXiv-2205.12674-009688.svg)](https://arxiv.org/abs/2205.12674) <br>
> Augmenting language models with longterm memory [![arXiv](https://img.shields.io/badge/arXiv-2306.07174-009688.svg)](https://arxiv.org/abs/2306.07174) <br>
> Lost in the middle: How language models use long contexts [![arXiv](https://img.shields.io/badge/arXiv-2307.03172-009688.svg)](https://arxiv.org/abs/2307.03172) <br>

**Parameter-Efficient Fine-Tuning (PEFT):** PEFT is a critical technique for optimizing LLMs by reducing the trainable parameter number and GPU memory overhead, addressing the infeasibility of full fine-tuning in resourceconstrained environments.
> Parameter-efficient fine-tuning methods for pretrained language models: A critical review and assessment [![arXiv](https://img.shields.io/badge/arXiv-2312.12148-009688.svg)](https://arxiv.org/abs/2312.12148) <br>
> Lora: Low-rank adaptation of large language models [![arXiv](https://img.shields.io/badge/arXiv-2106.09685-009688.svg)](https://arxiv.org/abs/2106.09685) <br>

**LLM-Based Agents:** LLM-based agents represent a transformative evolution of LLMs, enabling them to function as autonomous entities capable of perceiving environments, reasoning, and executing actions.
> Toolformer: Language models can teach themselves to use tools [![arXiv](https://img.shields.io/badge/arXiv-2302.04761-009688.svg)](https://arxiv.org/abs/2302.04761) <br>

## 📙LLM-based Collective Intelligence
![CI Framework](https://github.com/d-andelions/awesome-LLM-Driven-Collective-Intelligence/blob/main/figs/3.png)
> Donod: Robust and generalizable instruction fine-tuning for llms via modelintrinsic dataset pruning [![arXiv](https://img.shields.io/badge/arXiv-2504.14810v1-009688.svg)](https://arxiv.org/html/2504.14810v1) <br>
> Switch transformers: Scaling to trillion parameter models with simple and efficient sparsity [![arXiv](https://img.shields.io/badge/arXiv-2101.03961-009688.svg)](https://arxiv.org/abs/2101.03961) <br>
> Tree of thoughts: Deliberate problem solving with large language models [![arXiv](https://img.shields.io/badge/arXiv-2212.10001-009688.svg)](https://arxiv.org/abs/2212.10001) <br>
> Generative agents: Interactive simulacra of human behavior [![arXiv](https://img.shields.io/badge/arXiv-2304.03442-009688.svg)](https://arxiv.org/abs/2304.03442) <br>

## 📗Collective Intelligence 1.0 and 2.0 Era
**Collective Intelligence 1.0 Era:** Complex group behaviors can emerge from simple interaction rules.
> Swarm intelligence: from natural to artificial systems [![arXiv](https://img.shields.io/badge/Oxford-40811-009688.svg)](https://academic.oup.com/book/40811) <br>
> Ant colony optimization: a new metaheuristic [![arXiv](https://img.shields.io/badge/IEEE-782657-009688.svg)](https://ieeexplore.ieee.org/document/782657) <br>
> Particle swarm optimization [![arXiv](https://img.shields.io/badge/IEEE-488968-009688.svg)](https://ieeexplore.ieee.org/abstract/document/488968) <br>
> Aco algorithms for the traveling salesman problem [![arXiv](https://img.shields.io/badge/ResearchGate-2771967-009688.svg)](https://www.researchgate.net/publication/2771967_ACO_Algorithms_for_the_Traveling_Salesman_Problem) <br>
> A modified particle swarm optimizer [![arXiv](https://img.shields.io/badge/IEEE-699146-009688.svg)](https://ieeexplore.ieee.org/document/699146) <br>

**Collective Intelligence 2.0 Era:** The Collective Intelligence 2.0 Era marked a significant advancement through the development of specialized multi-agent architectures.
> Multi-agent architectures as organizational structures [![arXiv](https://img.shields.io/badge/springer-10.1007-009688.svg)](https://link.springer.com/article/10.1007/s10458-006-5717-6) <br>
> Parameter adaptation in ant colony optimization [![arXiv](https://img.shields.io/badge/springer-10.1007-009688.svg)](https://link.springer.com/chapter/10.1007/978-3-642-21434-9_8) <br>
> Swarm intelligence and evolutionary computation [![arXiv](https://img.shields.io/badge/sciencedirect-journal-009688.svg)](https://www.sciencedirect.com/journal/swarm-and-evolutionary-computation) <br>
> Distributed algorithms for multi-robot observation of multiple moving targets [![arXiv](https://img.shields.io/badge/springer-10.1023-009688.svg)](https://link.springer.com/article/10.1023/A:1015256330750) <br>
> Wireless sensor network survey [![arXiv](https://img.shields.io/badge/sciencedirect-article-009688.svg)](https://www.sciencedirect.com/science/article/pii/S1389128608001254) <br>

## 📘Collective Intelligence 3.0 Era
![Figure 4](https://github.com/d-andelions/awesome-LLM-Driven-Collective-Intelligence/blob/main/figs/4.png)
### 📖Data-Level Enhancement
**Same LLM Driven:**
> **Single-Round Role-Playing Interaction**
> Role play with large language models [![arXiv](https://img.shields.io/badge/arXiv-2305.16367-009688.svg)](https://arxiv.org/abs/2305.16367) <br>
> Picle: Eliciting diverse behaviors from large language models with persona in-context learning [![arXiv](https://img.shields.io/badge/arXiv-2405.02501-009688.svg)](https://arxiv.org/abs/2405.02501) <br>
> On the steerability of large language models toward data-driven personas [![arXiv](https://img.shields.io/badge/arXiv-2311.04978-009688.svg)](https://arxiv.org/abs/2311.04978) <br>
> Synthetic dialogue dataset generation using llm agents [![arXiv](https://img.shields.io/badge/arXiv-2401.17461-009688.svg)](https://arxiv.org/abs/2401.17461) <br>

> **Multi-Round Role-Playing Interaction**
> Unleashing the emergent cognitive synergy in large language models: A task-solving agent through multi-persona self-collaboration [![arXiv](https://img.shields.io/badge/arXiv-2307.05300-009688.svg)](https://arxiv.org/abs/2307.05300) <br>
> Diasynth: Synthetic dialogue generation framework for low resource dialogue applications [![arXiv](https://img.shields.io/badge/arXiv-2409.19020-009688.svg)](https://arxiv.org/abs/2409.19020) <br>
> Psydial: Personality-based synthetic dialogue generation using large language models [![arXiv](https://img.shields.io/badge/arXiv-2404.00930-009688.svg)](https://arxiv.org/abs/2404.00930) <br>
> Erabal: Enhancing role-playing agents through boundary-aware learning [![arXiv](https://img.shields.io/badge/arXiv-2409.14710-009688.svg)](https://arxiv.org/abs/2409.14710) <br>
> Reviewinstruct: A review-driven multi-turn conversations generation method for large language models [![arXiv](https://img.shields.io/badge/arXiv-2505.11010-009688.svg)](https://arxiv.org/abs/2505.11010) <br>

**Different LLM Driven:**
> **Centralized Control**
> Synthesizing post-training data for llms through multi-agent simulation [![arXiv](https://img.shields.io/badge/arXiv-2410.14251-009688.svg)](https://arxiv.org/abs/2410.14251) <br>
> Dflow: Diverse dialogue flow simulation with large language models [![arXiv](https://img.shields.io/badge/arXiv-2410.14853-009688.svg)](https://arxiv.org/abs/2410.14853) <br>

> **Decentralized Control**
> Scaling synthetic data creation with 1,000,000,000 personas [![arXiv](https://img.shields.io/badge/arXiv-2406.20094-009688.svg)](https://arxiv.org/abs/2406.20094) <br>
> Mag-v: A multi-agent framework for synthetic data generation and verification [![arXiv](https://img.shields.io/badge/arXiv-2412.04494-009688.svg)](https://arxiv.org/abs/2412.04494) <br>
> The fellowship of the llms: Multi-agent workflows for synthetic preference optimization dataset generation [![arXiv](https://img.shields.io/badge/arXiv-2408.08688-009688.svg)](https://arxiv.org/abs/2408.08688) <br>
> Language games as the pathway to artificial superhuman intelligence [![arXiv](https://img.shields.io/badge/arXiv-2501.18924-009688.svg)](https://arxiv.org/abs/2501.18924) <br>

### 📖Model-Level Enhancement
**Model Routing:**
> **Routing for Cost Reduction**
> Frugalgpt: How to use large language models while reducing cost and improving performance [![arXiv](https://img.shields.io/badge/arXiv-2305.05176-009688.svg)](https://arxiv.org/abs/2305.05176) <br>
> Automix: Automatically mixing language models [![arXiv](https://img.shields.io/badge/arXiv-2310.12963-009688.svg)](https://arxiv.org/abs/2310.12963) <br>
> Hybrid llm: Cost-efficient and quality-aware query routing [![arXiv](https://img.shields.io/badge/arXiv-2404.14618-009688.svg)](https://arxiv.org/abs/2404.14618) <br>
> Mixllm: Dynamic routing in mixed large language models [![arXiv](https://img.shields.io/badge/arXiv-2502.18482-009688.svg)](https://arxiv.org/abs/2502.18482) <br>
> Swiftsage: A generative agent with fast and slow thinking for complex interactive tasks [![arXiv](https://img.shields.io/badge/arXiv-2305.17390-009688.svg)](https://arxiv.org/abs/2305.17390) <br>
> Llm-powered hierarchical language agent for real-time humanai coordination [![arXiv](https://img.shields.io/badge/arXiv-2312.15224-009688.svg)](https://arxiv.org/abs/2312.15224) <br>
> Routoo: Learning to route to large language models effectively [![arXiv](https://img.shields.io/badge/arXiv-2401.13979-009688.svg)](https://arxiv.org/abs/2401.13979) <br>
> Routellm: Learning to route llms with preference data [![arXiv](https://img.shields.io/badge/arXiv-2406.18665-009688.svg)](https://arxiv.org/abs/2406.18665) <br>
> Llm bandit: Cost-efficient llm generation via preferenceconditioned dynamic routing [![arXiv](https://img.shields.io/badge/arXiv-2502.02743-009688.svg)](https://arxiv.org/abs/2502.02743) <br>

> **Routing for Performance Enhancement**
> Llm-blender: Ensembling large language models with pairwise ranking and generative fusion [![arXiv](https://img.shields.io/badge/arXiv-2306.02561-009688.svg)](https://arxiv.org/abs/2306.02561) <br>
> Loraretriever: Input-aware lora retrieval and composition for mixed tasks in the wild [![arXiv](https://img.shields.io/badge/arXiv-2402.09997-009688.svg)](https://arxiv.org/abs/2402.09997) <br>
> Large language model routing with benchmark datasets [![arXiv](https://img.shields.io/badge/arXiv-2309.15789-009688.svg)](https://arxiv.org/abs/2309.15789) <br>
> Routing to the expert: Efficient reward-guided ensemble of large language models [![arXiv](https://img.shields.io/badge/arXiv-2311.08692-009688.svg)](https://arxiv.org/abs/2311.08692) <br>
> Universal model routing for efficient LLM inference [![arXiv](https://img.shields.io/badge/arXiv-2502.08773-009688.svg)](https://arxiv.org/abs/2502.08773) <br>
> Capability instruction tuning: A new paradigm for dynamic LLM routing [![arXiv](https://img.shields.io/badge/arXiv-2502.17282-009688.svg)](https://arxiv.org/abs/2502.17282) <br>
> EmbedLLM: Learning compact representations of large language models [![arXiv](https://img.shields.io/badge/arXiv-2410.02223-009688.svg)](https://arxiv.org/abs/2410.02223) <br>
> Routerbench: A benchmark for multi-LLM routing system [![arXiv](https://img.shields.io/badge/arXiv-2403.12031-009688.svg)](https://arxiv.org/abs/2403.12031) <br>
> Routerdc: Query-based router by dual contrastive learning for assembling large language models [![arXiv](https://img.shields.io/badge/arXiv-2409.19886-009688.svg)](https://arxiv.org/abs/2409.19886) <br>
> Graphrouter: A graph-based router for LLM selections [![arXiv](https://img.shields.io/badge/arXiv-2410.03834-009688.svg)](https://arxiv.org/abs/2410.03834) <br>
> Learning to decode collaboratively with multiple language models [![arXiv](https://img.shields.io/badge/arXiv-2403.03870-009688.svg)](https://arxiv.org/abs/2403.03870) <br>
> Citer: Collaborative inference for efficient large language model decoding with token-level routing [![arXiv](https://img.shields.io/badge/arXiv-2502.01976-009688.svg)](https://arxiv.org/abs/2502.01976) <br>

**Model Merging:**
> **Single-task Homogeneous Merging**
> Emr-merging: Tuning-free high-performance model merging[![arXiv](https://img.shields.io/badge/arXiv-2405.17461-009688.svg)](https://arxiv.org/abs/2405.17461) <br>
> Editing models with task arithmetic merging[![arXiv](https://img.shields.io/badge/arXiv-2212.04089-009688.svg)](https://arxiv.org/abs/2212.04089) <br>
> Evolutionary optimization of model merging recipes [![arXiv](https://img.shields.io/badge/arXiv-2403.13187-009688.svg)](https://arxiv.org/abs/2403.13187) <br>
> Representation surgery for multi-task model merging [![arXiv](https://img.shields.io/badge/arXiv-2402.02705-009688.svg)](https://arxiv.org/abs/2402.02705) <br>
> Merging multi-task models via weight-ensembling mixture of experts [![arXiv](https://img.shields.io/badge/arXiv-2402.00433-009688.svg)](https://arxiv.org/abs/2402.00433) <br>
> Dynamic model merging with mixture of weights [![arXiv](https://img.shields.io/badge/IEEE-10900479-009688.svg)](https://ieeexplore.ieee.org/document/10900479) <br>
> Twinmerging: Dynamic integration of modular expertise in model merging [![arXiv](https://img.shields.io/badge/arXiv-2406.15479-009688.svg)](https://arxiv.org/abs/2406.15479) <br>
> Less is more: Efficient model merging with binary task switch [![arXiv](https://img.shields.io/badge/arXiv-2412.00054-009688.svg)](https://arxiv.org/abs/2412.00054) <br>
> Lora soups: Merging loras for practical skill composition tasks [![arXiv](https://img.shields.io/badge/arXiv-2410.13025-009688.svg)](https://arxiv.org/abs/2410.13025) <br>
> Model merging with svd to tie the knots [![arXiv](https://img.shields.io/badge/arXiv-2410.19735-009688.svg)](https://arxiv.org/abs/2410.19735) <br>
> Merging loras like playing lego: Pushing the modularity of lora to extremes through rank-wise clustering [![arXiv](https://img.shields.io/badge/arXiv-2409.16167-009688.svg)](https://arxiv.org/abs/2409.16167) <br>
> Lori: Reducing cross-task interference in multi-task low-rank adaptation [![arXiv](https://img.shields.io/badge/arXiv-2504.07448-009688.svg)](https://arxiv.org/abs/2504.07448) <br>
> Experts weights averaging: A new general training scheme for vision transformers [![arXiv](https://img.shields.io/badge/arXiv-2308.06093-009688.svg)](https://arxiv.org/abs/2308.06093) <br>
> Model soups: averaging weights of multiple fine-tuned models improves accuracy without increasing inference time rank-wise clustering [![arXiv](https://img.shields.io/badge/arXiv-2203.05482-009688.svg)](https://arxiv.org/abs/2203.05482) <br>
> Model ratatouille: Recycling diverse models for out-of-distribution generalization [![arXiv](https://img.shields.io/badge/arXiv-2212.10445-009688.svg)](https://arxiv.org/abs/2212.10445) <br>

> **Multi-task Homogeneous Merging**
> Editing models with task arithmetic [![arXiv](https://img.shields.io/badge/arXiv-2212.04089-009688.svg)](https://arxiv.org/abs/2212.04089) <br>
> Evolutionary optimization of model merging recipes [![arXiv](https://img.shields.io/badge/arXiv-2403.13187-009688.svg)](https://arxiv.org/abs/2403.13187) <br>
> Representation surgery for multi-task model merging [![arXiv](https://img.shields.io/badge/arXiv-2402.02705-009688.svg)](https://arxiv.org/abs/2402.02705) <br>
> Merging multi-task models via weight-ensembling mixture of experts [![arXiv](https://img.shields.io/badge/arXiv-2402.00433-009688.svg)](https://arxiv.org/abs/2402.00433) <br>
> Dynamic model merging with mixture of weights [![arXiv](https://img.shields.io/badge/IEEE-10900479-009688.svg)](https://ieeexplore.ieee.org/document/10900479) <br>
> EMR-Merging: Tuning-free high-performance model merging [![arXiv](https://img.shields.io/badge/arXiv-2405.17461-009688.svg)](https://arxiv.org/abs/2405.17461) <br>
> Twinmerging: Dynamic integration of modular expertise in model merging [![arXiv](https://img.shields.io/badge/arXiv-2406.15479-009688.svg)](https://arxiv.org/abs/2406.15479) <br>
> Less is more: Efficient model merging with binary task switch [![arXiv](https://img.shields.io/badge/arXiv-2412.00054-009688.svg)](https://arxiv.org/abs/2412.00054) <br>
> Lora soups: Merging loras for practical skill composition tasks [![arXiv](https://img.shields.io/badge/arXiv-2410.13025-009688.svg)](https://arxiv.org/abs/2410.13025) <br>
> Model merging with svd to tie the knots [![arXiv](https://img.shields.io/badge/arXiv-2410.19735-009688.svg)](https://arxiv.org/abs/2410.19735) <br>
> Merging loras like playing lego: Pushing the modularity of lora to extremes through rank-wise clustering [![arXiv](https://img.shields.io/badge/arXiv-2409.16167-009688.svg)](https://arxiv.org/abs/2409.16167) <br>
> Lori: Reducing cross-task interference in multi-task low-rank adaptation [![arXiv](https://img.shields.io/badge/arXiv-2504.07448-009688.svg)](https://arxiv.org/abs/2504.07448) <br>

**Model Ensemble:**
> **Token-level Ensemble**
> Breaking the ceiling of the LLM community by treating token generation as a classification for ensembling [![arXiv](https://img.shields.io/badge/arXiv-2406.12585-009688.svg)](https://arxiv.org/abs/2406.12585) <br>
> Determine-then-ensemble: Necessity of top-k union for large language model ensembling [![arXiv](https://img.shields.io/badge/arXiv-2410.03777-009688.svg)](https://arxiv.org/abs/2410.03777) <br>
> Pack of LLMs: Model fusion at test-time via perplexity optimization [![arXiv](https://img.shields.io/badge/arXiv-2404.11531-009688.svg)](https://arxiv.org/abs/2404.11531) <br>
> Collaborative decoding of critical tokens for boosting factuality of large language models [![arXiv](https://img.shields.io/badge/arXiv-2402.17982-009688.svg)](https://arxiv.org/abs/2402.17982) <br>
> Bridging the gap between different vocabularies for llm ensemble [![arXiv](https://img.shields.io/badge/arXiv-2404.09492-009688.svg)](https://arxiv.org/abs/2404.09492) <br>
> Ensemble learning for heterogeneous large language models with deep parallel collaboration [![arXiv](https://img.shields.io/badge/arXiv-2406.15479-009688.svg)](https://arxiv.org/abs/2406.15479) <br>

> **Span-level Ensemble**
> Coolfusion: Fuse large language models without training [![arXiv](https://img.shields.io/badge/arXiv-2407.19807-009688.svg)](https://arxiv.org/abs/2407.19807) <br>
> Ensembling large language models with process reward-guided tree search for better complex reasoning [![arXiv](https://img.shields.io/badge/arXiv-2412.15797-009688.svg)](https://arxiv.org/abs/2412.15797) <br>
> Hit the sweet spot! Span-level ensemble for large language models [![arXiv](https://img.shields.io/badge/arXiv-2409.18583-009688.svg)](https://arxiv.org/abs/2409.18583) <br>
> Specfuse: Ensembling large language models via next-segment prediction [![arXiv](https://img.shields.io/badge/arXiv-2412.07380-009688.svg)](https://arxiv.org/abs/2412.07380) <br>

> **Response-level Ensemble**
> Mixture-of-agents enhances large language model capabilities [![arXiv](https://img.shields.io/badge/arXiv-2406.04692-009688.svg)](https://arxiv.org/abs/2406.04692) <br>
> SMoA: Improving multi-agent large language models with sparse mixture-of-agents [![arXiv](https://img.shields.io/badge/arXiv-2411.03284-009688.svg)](https://arxiv.org/abs/2411.03284) <br>
> Symbolic mixture-of-experts: Adaptive skill-based routing for heterogeneous reasoning [![arXiv](https://img.shields.io/badge/arXiv-2503.05641-009688.svg)](https://arxiv.org/abs/2503.05641) <br>
> Do we truly need so many samples? Multi-LLM repeated sampling efficiently scale test-time compute [![arXiv](https://img.shields.io/badge/arXiv-2504.00762-009688.svg)](https://arxiv.org/abs/2504.00762) <br>
> More agents is all you need [![arXiv](https://img.shields.io/badge/arXiv-2402.05120-009688.svg)](https://arxiv.org/abs/2402.05120) <br>
> Rethinking mixture-of-agents: Is mixing different large language models beneficial? [![arXiv](https://img.shields.io/badge/arXiv-2502.00674-009688.svg)](https://arxiv.org/abs/2502.00674) <br>

### 📖Inference-Level Enhancement
**Self-driven Enhancement:**
> **Self-Ensemble Enhancement**
> Self-consistency improves chain of thought reasoning in language models [![arXiv](https://img.shields.io/badge/arXiv-2203.11171-009688.svg)](https://arxiv.org/abs/2203.11171) <br>
> The curious case of neural text degeneration [![arXiv](https://img.shields.io/badge/arXiv-1904.09751-009688.svg)](https://arxiv.org/abs/1904.09751) <br>
> Chain-of-thought prompting elicits reasoning in large language models [![arXiv](https://img.shields.io/badge/arXiv-2201.11903-009688.svg)](https://arxiv.org/abs/2201.11903) <br>
> Accessing GPT-4 level mathematical olympiad solutions via Monte Carlo tree self-refine with LLaMa-3 8B [![arXiv](https://img.shields.io/badge/arXiv-2406.07394-009688.svg)](https://arxiv.org/abs/2406.07394) <br>
> CoT-based synthesizer: Enhancing LLM performance through answer synthesis [![arXiv](https://img.shields.io/badge/arXiv-2501.01668-009688.svg)](https://arxiv.org/abs/2501.01668) <br>
> Tree of thoughts: Deliberate problem solving with large language models [![arXiv](https://img.shields.io/badge/arXiv-2212.10001-009688.svg)](https://arxiv.org/abs/2212.10001) <br>
> **Self-Improvement Enhancement**
> Reflexion: Language agents with verbal reinforcement learning [![arXiv](https://img.shields.io/badge/arXiv-2303.11366-009688.svg)](https://arxiv.org/abs/2303.11366) <br>
> Retroformer: Retrospective large language agents with policy gradient optimization [![arXiv](https://img.shields.io/badge/arXiv-2308.02151-009688.svg)](https://arxiv.org/abs/2308.02151) <br>
> Reflective multi-agent collaboration based on large language models [![arXiv](https://img.shields.io/badge/ACM-10.5555-009688.svg)](https://dl.acm.org/doi/10.5555/3737916.3742313) <br>
> ProAgent: Building proactive cooperative agents with large language models [![arXiv](https://img.shields.io/badge/arXiv-2308.11339-009688.svg)](https://arxiv.org/abs/2308.11339) <br>
> Hypothetical minds: Scaffolding theory of mind for multi-agent tasks with large language models [![arXiv](https://img.shields.io/badge/arXiv-2407.07086-009688.svg)](https://arxiv.org/abs/2407.07086) <br>

**Cooperation-driven Enhancement:**
> **Task Planning Based Collaboration**
> HuggingGPT: Solving AI tasks with ChatGPT and its friends in Hugging Face [![arXiv](https://img.shields.io/badge/arXiv-2303.17580-009688.svg)](https://arxiv.org/abs/2303.17580) <br>
> Skeleton-of-thought: Prompting LLMs for efficient parallel generation [![arXiv](https://img.shields.io/badge/arXiv-2307.15337-009688.svg)](https://arxiv.org/abs/2307.15337) <br>
> Voyager: An open-ended embodied agent with large language models [![arXiv](https://img.shields.io/badge/arXiv-2305.16291-009688.svg)](https://arxiv.org/abs/2305.16291) <br>
> Scalable multi-robot collaboration with large language models: Centralized or decentralized systems? [![arXiv](https://img.shields.io/badge/arXiv-2309.15943-009688.svg)](https://arxiv.org/abs/2309.15943) <br>
> RoCo: Dialectic multi-robot collaboration with large language models [![arXiv](https://img.shields.io/badge/arXiv-2307.04738-009688.svg)](https://arxiv.org/abs/2307.04738) <br>
> Chameleon: Plug-and-play compositional reasoning with large language models [![arXiv](https://img.shields.io/badge/arXiv-2304.09842-009688.svg)](https://arxiv.org/abs/2304.09842) <br>
> TwoStep: Multi-agent task planning using classical planners and large language models [![arXiv](https://img.shields.io/badge/arXiv-2403.17246-009688.svg)](https://arxiv.org/abs/2403.17246) <br>
> AutoGen: Enabling next-gen LLM applications via multi-agent conversation [![arXiv](https://img.shields.io/badge/arXiv-2308.08155-009688.svg)](https://arxiv.org/abs/2308.08155) <br>
> Magis: LLM-based multi-agent framework for GitHub issue resolution [![arXiv](https://img.shields.io/badge/arXiv-2403.17927-009688.svg)](https://arxiv.org/abs/2403.17927) <br>

> **LLM–SLM Collaboration**
> CITER: Collaborative inference for efficient large language model decoding with token-level routing [![arXiv](https://img.shields.io/badge/arXiv-2502.01976-009688.svg)](https://arxiv.org/abs/2502.01976) <br>
> CoGenesis: A framework collaborating large and small language models for secure context-aware instruction following [![arXiv](https://img.shields.io/badge/arXiv-2403.03129-009688.svg)](https://arxiv.org/abs/2403.03129) <br>
> Hybrid LLM: Towards low-latency multi-granularity routing between small and large models [![arXiv](https://img.shields.io/badge/arXiv-2404.14618-009688.svg)](https://arxiv.org/abs/2404.14618) <br>
> Collab-RAG: Collaborative retrieval-augmented generation using large and small language models [![arXiv](https://img.shields.io/badge/arXiv-2504.04915-009688.svg)](https://arxiv.org/abs/2504.04915) <br>
> CE-CoLLM: Cloud-edge cooperative LLM framework for enterprise knowledge management [![arXiv](https://img.shields.io/badge/arXiv-2411.02829-009688.svg)](https://arxiv.org/abs/2411.02829) <br>
> FedCoLLM: Federated collaboration of large and small language models for private data processing [![arXiv](https://img.shields.io/badge/arXiv-2411.11707-009688.svg)](https://arxiv.org/abs/2411.11707) <br>
> Collaboration of large language models and small recommendation models for device-cloud recommendation [![arXiv](https://img.shields.io/badge/arXiv-2501.05647-009688.svg)](https://arxiv.org/abs/2501.05647) <br>

> **Dual-System Collaboration**
> Thinking, Fast and Slow [![arXiv](https://img.shields.io/badge/wikipedia-Thinking-009688.svg)](https://en.wikipedia.org/wiki/Thinking,_Fast_and_Slow) <br>
> DSADF: Thinking fast and slow for decision making [![arXiv](https://img.shields.io/badge/arXiv-2505.08189-009688.svg)](https://arxiv.org/abs/2505.08189) <br>
> Visual agents as fast and slow thinkers [![arXiv](https://img.shields.io/badge/arXiv-2408.08862-009688.svg)](https://arxiv.org/abs/2408.08862) <br>
> Thinking fast and slow: Efficient text-to-visual retrieval with transformers [![arXiv](https://img.shields.io/badge/arXiv-2103.16553-009688.svg)](https://arxiv.org/abs/2103.16553) <br>
> Interactive continual learning: Fast and slow thinking [![arXiv](https://img.shields.io/badge/arXiv-2403.02628-009688.svg)](https://arxiv.org/abs/2403.02628) <br>
> Thinking fast and slow in large language models [![arXiv](https://img.shields.io/badge/arXiv-2212.05206-009688.svg)](https://arxiv.org/abs/2212.05206) <br>
> RoboMamba: Multimodal state space model for efficient robot reasoning and manipulation [![arXiv](https://img.shields.io/badge/arXiv-2406.04339-009688.svg)](https://arxiv.org/abs/2406.04339) <br>


**Competition-involved Enhancement**
> **Multi-Agent Debate**
> Improving factuality and reasoning in language models through multi-agent debate [![arXiv](https://img.shields.io/badge/arXiv-2305.14325-009688.svg)](https://arxiv.org/abs/2305.14325) <br>
> Examining inter-consistency of large language models collaboration: An in-depth analysis via debate [![arXiv](https://img.shields.io/badge/arXiv-2305.11595-009688.svg)](https://arxiv.org/abs/2305.11595) <br>
> ReConcile: Roundtable conference improves reasoning via consensus among diverse LLMs [![arXiv](https://img.shields.io/badge/arXiv-2309.13007-009688.svg)](https://arxiv.org/abs/2309.13007) <br>
> ChatEval: Towards better LLM-based evaluators through multi-agent debate [![arXiv](https://img.shields.io/badge/arXiv-2308.07201-009688.svg)](https://arxiv.org/abs/2308.07201) <br>
> CAMEL: Communicative agents for "mind" exploration of large language model society [![arXiv](https://img.shields.io/badge/arXiv-2303.17760-009688.svg)](https://arxiv.org/abs/2303.17760) <br>
> CoMM: Collaborative multi-agent, multi-reasoning-path prompting for complex problem solving [![arXiv](https://img.shields.io/badge/arXiv-2404.17729-009688.svg)](https://arxiv.org/abs/2404.17729) <br>
> Encouraging divergent thinking in large language models through multi-agent debate [![arXiv](https://img.shields.io/badge/arXiv-2305.19118-009688.svg)](https://arxiv.org/abs/2305.19118) <br>
> LM vs LM: Detecting factual errors via cross examination [![arXiv](https://img.shields.io/badge/arXiv-2305.13281-009688.svg)](https://arxiv.org/abs/2305.13281) <br>
> Exchange-of-thought: Enhancing large language model capabilities through cross-model communication [![arXiv](https://img.shields.io/badge/arXiv-2312.01823-009688.svg)](https://arxiv.org/abs/2312.01823) <br>
> Can LLMs beat humans in debating? A dynamic multi-agent framework for competitive debate [![arXiv](https://img.shields.io/badge/arXiv-2408.04472-009688.svg)](https://arxiv.org/abs/2408.04472) <br>
> Internet of agents: Weaving a web of heterogeneous agents for collaborative intelligence [![arXiv](https://img.shields.io/badge/arXiv-2407.07061-009688.svg)](https://arxiv.org/abs/2407.07061) <br>
> Improving multi-agent debate with sparse communication topology [![arXiv](https://img.shields.io/badge/arXiv-2406.11776-009688.svg)](https://arxiv.org/abs/2406.11776) <br>
> Rethinking the bounds of LLM reasoning: Are multi-agent discussions the key? [![arXiv](https://img.shields.io/badge/arXiv-2402.18272-009688.svg)](https://arxiv.org/abs/2402.18272) <br>
> If multi-agent debate is the answer, what is the question? [![arXiv](https://img.shields.io/badge/arXiv-2502.08788-009688.svg)](https://arxiv.org/abs/2502.08788) <br>
> Agentverse: Facilitating multi-agent collaboration and exploring emergent behaviors [![arXiv](https://img.shields.io/badge/arXiv-2308.10848-009688.svg)](https://arxiv.org/abs/2308.10848) <br>

> **Critique Mechanisms**
> Multi-agent verification: Scaling test-time compute with multiple verifiers [![arXiv](https://img.shields.io/badge/arXiv-2502.20379-009688.svg)](https://arxiv.org/abs/2502.20379) <br>
> Critic-V: VLM critics help catch VLM errors in multimodal reasoning [![arXiv](https://img.shields.io/badge/arXiv-2411.18203-009688.svg)](https://arxiv.org/abs/2411.18203) <br>
> LLaMA-Berry: Pairwise optimization for O1-like olympiad-level mathematical reasoning [![arXiv](https://img.shields.io/badge/arXiv-2410.02884-009688.svg)](https://arxiv.org/abs/2410.02884) <br>
> CRITIC: Large language models can self-correct with tool-interactive critiquing [![arXiv](https://img.shields.io/badge/arXiv-2305.11738-009688.svg)](https://arxiv.org/abs/2305.11738) <br>
> TORA: A tool-integrated reasoning agent for mathematical problem solving [![arXiv](https://img.shields.io/badge/arXiv-2309.17452-009688.svg)](https://arxiv.org/abs/2309.17452) <br>
> Training language models to critique with multi-agent feedback [![arXiv](https://img.shields.io/badge/arXiv-2410.15287-009688.svg)](https://arxiv.org/abs/2410.15287) <br>
> Towards efficient LLM grounding for embodied multi-agent collaboration [![arXiv](https://img.shields.io/badge/arXiv-2405.14314-009688.svg)](https://arxiv.org/abs/2405.14314) <br>

**Self-Organizing Collective Optimization**
> **Heuristic Collective Optimization**
> Model Swarms: Collaborative search to adapt LLM experts via swarm intelligence [![arXiv](https://img.shields.io/badge/arXiv-2410.11163-009688.svg)](https://arxiv.org/abs/2410.11163) <br>
> Heterogeneous Swarms: Jointly optimizing model roles and weights for multi-LLM systems [![arXiv](https://img.shields.io/badge/arXiv-2502.04510-009688.svg)](https://arxiv.org/abs/2502.04510) <br>
> SwarmPrompt: Swarm intelligence-driven prompt optimization using large language models [![arXiv](https://img.shields.io/badge/researchr-ShriyanSASA25-009688.svg)](https://researchr.org/publication/ShriyanSASA25) <br>
> Multi-agent systems powered by large language models: Applications in swarm intelligence [![arXiv](https://img.shields.io/badge/arXiv-2503.03800-009688.svg)](https://arxiv.org/abs/2503.03800) <br>
> Nature-inspired population-based evolution of large language models [![arXiv](https://img.shields.io/badge/arXiv-2503.01155-009688.svg)](https://arxiv.org/abs/2503.01155) <br>
> The society of hivemind: Multi-agent optimization of foundation model swarms to unlock the potential of collective intelligence [![arXiv](https://img.shields.io/badge/arXiv-2503.05473-009688.svg)](https://arxiv.org/abs/2503.05473) <br>
> EvoFlow: Evolving diverse agentic workflows on the fly [![arXiv](https://img.shields.io/badge/arXiv-2502.07373-009688.svg)](https://arxiv.org/abs/2502.07373) <br>
> EvoAgent: Towards automatic multi-agent generation via evolutionary algorithms [![arXiv](https://img.shields.io/badge/arXiv-2406.14228-009688.svg)](https://arxiv.org/abs/2406.14228) <br>

> **Automated Collective Optimization**
> Multi-agent architecture search via agentic supernet [![arXiv](https://img.shields.io/badge/arXiv-2502.04180-009688.svg)](https://arxiv.org/abs/2502.04180) <br>
> GPTSwarm: Language agents as optimizable graphs [![arXiv](https://img.shields.io/badge/arXiv-2402.16823v3-009688.svg)](https://arxiv.org/abs/2402.16823v3) <br>
> AgentDropout: Dynamic agent elimination for token-efficient and high-performance LLM-based multi-agent collaboration [![arXiv](https://img.shields.io/badge/arXiv-2503.18891-009688.svg)](https://arxiv.org/abs/2503.18891) <br>
> Automated design of agentic systems [![arXiv](https://img.shields.io/badge/arXiv-2408.08435-009688.svg)](https://arxiv.org/abs/2408.08435) <br>
> ReSO: A reward-driven self-organizing LLM-based multi-agent system for reasoning tasks [![arXiv](https://img.shields.io/badge/arXiv-2503.02390-009688.svg)](https://arxiv.org/abs/2503.02390) <br>
> AFlow: Automating agentic workflow generation [![arXiv](https://img.shields.io/badge/arXiv-2410.10762-009688.svg)](https://arxiv.org/abs/2410.10762) <br>
> Multi-agent design: Optimizing agents with better prompts and topologies [![arXiv](https://img.shields.io/badge/arXiv-2502.02533-009688.svg)](https://arxiv.org/abs/2502.02533) <br>
> Symbolic learning enables self-evolving agents [![arXiv](https://img.shields.io/badge/arXiv-2406.18532-009688.svg)](https://arxiv.org/abs/2406.18532) <br>


## 📙LLM Driven Application-Oriented Collective Intelligence
![Figure 5](https://github.com/d-andelions/awesome-LLM-Driven-Collective-Intelligence/blob/main/figs/5.png)
### 📖Scientific Discovery and Autonomous Research
**Scientific Discovery:**
**Autonomous Research:**

### 📖Embodied Intelligence Research
**Centralized Control Paradigm:**
**Decentralized Interactive Paradigm:**

### 📖Social Science Research
**Scope of Simulation:**
**Application of Simulation:**

### 📖Auto-Programming
**Foundation-Oriented Programming:**
**Application-Oriented Programming:**

### 📖GUI Operations
**Prompting-Based Methods:**
**Tuning-Based Methods:**

### 📖Game Theory and Interactive Games
**Application in Game Theory:**
**Application in Interactive Games:**

## 📗Collective Intelligence 4.0 Era
