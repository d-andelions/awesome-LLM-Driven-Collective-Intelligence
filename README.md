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
  - [SAIL THE WAY TO THE INTELLIGENCE FUTURE](#SAIL-THE-WAY-TO-THE-INTELLIGENCE-FUTURE)
  - [Major Scientific Problems](#Major-Scientific-Problems)
- [Conclusion](#conclusion)

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
> **Single-Round Role-Playing Interaction** <br>
> Role play with large language models [![arXiv](https://img.shields.io/badge/arXiv-2305.16367-009688.svg)](https://arxiv.org/abs/2305.16367) <br>
> Picle: Eliciting diverse behaviors from large language models with persona in-context learning [![arXiv](https://img.shields.io/badge/arXiv-2405.02501-009688.svg)](https://arxiv.org/abs/2405.02501) <br>
> On the steerability of large language models toward data-driven personas [![arXiv](https://img.shields.io/badge/arXiv-2311.04978-009688.svg)](https://arxiv.org/abs/2311.04978) <br>
> Synthetic dialogue dataset generation using llm agents [![arXiv](https://img.shields.io/badge/arXiv-2401.17461-009688.svg)](https://arxiv.org/abs/2401.17461) <br>

> **Multi-Round Role-Playing Interaction** <br>
> Unleashing the emergent cognitive synergy in large language models: A task-solving agent through multi-persona self-collaboration [![arXiv](https://img.shields.io/badge/arXiv-2307.05300-009688.svg)](https://arxiv.org/abs/2307.05300) <br>
> Diasynth: Synthetic dialogue generation framework for low resource dialogue applications [![arXiv](https://img.shields.io/badge/arXiv-2409.19020-009688.svg)](https://arxiv.org/abs/2409.19020) <br>
> Psydial: Personality-based synthetic dialogue generation using large language models [![arXiv](https://img.shields.io/badge/arXiv-2404.00930-009688.svg)](https://arxiv.org/abs/2404.00930) <br>
> Erabal: Enhancing role-playing agents through boundary-aware learning [![arXiv](https://img.shields.io/badge/arXiv-2409.14710-009688.svg)](https://arxiv.org/abs/2409.14710) <br>
> Reviewinstruct: A review-driven multi-turn conversations generation method for large language models [![arXiv](https://img.shields.io/badge/arXiv-2505.11010-009688.svg)](https://arxiv.org/abs/2505.11010) <br>

**Different LLM Driven:**
> **Centralized Control** <br>
> Synthesizing post-training data for llms through multi-agent simulation [![arXiv](https://img.shields.io/badge/arXiv-2410.14251-009688.svg)](https://arxiv.org/abs/2410.14251) <br>
> Dflow: Diverse dialogue flow simulation with large language models [![arXiv](https://img.shields.io/badge/arXiv-2410.14853-009688.svg)](https://arxiv.org/abs/2410.14853) <br>

> **Decentralized Control** <br>
> Scaling synthetic data creation with 1,000,000,000 personas [![arXiv](https://img.shields.io/badge/arXiv-2406.20094-009688.svg)](https://arxiv.org/abs/2406.20094) <br>
> Mag-v: A multi-agent framework for synthetic data generation and verification [![arXiv](https://img.shields.io/badge/arXiv-2412.04494-009688.svg)](https://arxiv.org/abs/2412.04494) <br>
> The fellowship of the llms: Multi-agent workflows for synthetic preference optimization dataset generation [![arXiv](https://img.shields.io/badge/arXiv-2408.08688-009688.svg)](https://arxiv.org/abs/2408.08688) <br>
> Language games as the pathway to artificial superhuman intelligence [![arXiv](https://img.shields.io/badge/arXiv-2501.18924-009688.svg)](https://arxiv.org/abs/2501.18924) <br>

### 📖Model-Level Enhancement
**Model Routing:**
> **Routing for Cost Reduction** <br>
> Frugalgpt: How to use large language models while reducing cost and improving performance [![arXiv](https://img.shields.io/badge/arXiv-2305.05176-009688.svg)](https://arxiv.org/abs/2305.05176) <br>
> Automix: Automatically mixing language models [![arXiv](https://img.shields.io/badge/arXiv-2310.12963-009688.svg)](https://arxiv.org/abs/2310.12963) <br>
> Hybrid llm: Cost-efficient and quality-aware query routing [![arXiv](https://img.shields.io/badge/arXiv-2404.14618-009688.svg)](https://arxiv.org/abs/2404.14618) <br>
> Mixllm: Dynamic routing in mixed large language models [![arXiv](https://img.shields.io/badge/arXiv-2502.18482-009688.svg)](https://arxiv.org/abs/2502.18482) <br>
> Swiftsage: A generative agent with fast and slow thinking for complex interactive tasks [![arXiv](https://img.shields.io/badge/arXiv-2305.17390-009688.svg)](https://arxiv.org/abs/2305.17390) <br>
> Llm-powered hierarchical language agent for real-time humanai coordination [![arXiv](https://img.shields.io/badge/arXiv-2312.15224-009688.svg)](https://arxiv.org/abs/2312.15224) <br>
> Routoo: Learning to route to large language models effectively [![arXiv](https://img.shields.io/badge/arXiv-2401.13979-009688.svg)](https://arxiv.org/abs/2401.13979) <br>
> Routellm: Learning to route llms with preference data [![arXiv](https://img.shields.io/badge/arXiv-2406.18665-009688.svg)](https://arxiv.org/abs/2406.18665) <br>
> Llm bandit: Cost-efficient llm generation via preferenceconditioned dynamic routing [![arXiv](https://img.shields.io/badge/arXiv-2502.02743-009688.svg)](https://arxiv.org/abs/2502.02743) <br>

> **Routing for Performance Enhancement** <br>
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
> **Single-task Homogeneous Merging** <br>
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

> **Multi-task Homogeneous Merging** <br>
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
> **Token-level Ensemble** <br>
> Breaking the ceiling of the LLM community by treating token generation as a classification for ensembling [![arXiv](https://img.shields.io/badge/arXiv-2406.12585-009688.svg)](https://arxiv.org/abs/2406.12585) <br>
> Determine-then-ensemble: Necessity of top-k union for large language model ensembling [![arXiv](https://img.shields.io/badge/arXiv-2410.03777-009688.svg)](https://arxiv.org/abs/2410.03777) <br>
> Pack of LLMs: Model fusion at test-time via perplexity optimization [![arXiv](https://img.shields.io/badge/arXiv-2404.11531-009688.svg)](https://arxiv.org/abs/2404.11531) <br>
> Collaborative decoding of critical tokens for boosting factuality of large language models [![arXiv](https://img.shields.io/badge/arXiv-2402.17982-009688.svg)](https://arxiv.org/abs/2402.17982) <br>
> Bridging the gap between different vocabularies for llm ensemble [![arXiv](https://img.shields.io/badge/arXiv-2404.09492-009688.svg)](https://arxiv.org/abs/2404.09492) <br>
> Ensemble learning for heterogeneous large language models with deep parallel collaboration [![arXiv](https://img.shields.io/badge/arXiv-2406.15479-009688.svg)](https://arxiv.org/abs/2406.15479) <br>

> **Span-level Ensemble** <br>
> Coolfusion: Fuse large language models without training [![arXiv](https://img.shields.io/badge/arXiv-2407.19807-009688.svg)](https://arxiv.org/abs/2407.19807) <br>
> Ensembling large language models with process reward-guided tree search for better complex reasoning [![arXiv](https://img.shields.io/badge/arXiv-2412.15797-009688.svg)](https://arxiv.org/abs/2412.15797) <br>
> Hit the sweet spot! Span-level ensemble for large language models [![arXiv](https://img.shields.io/badge/arXiv-2409.18583-009688.svg)](https://arxiv.org/abs/2409.18583) <br>
> Specfuse: Ensembling large language models via next-segment prediction [![arXiv](https://img.shields.io/badge/arXiv-2412.07380-009688.svg)](https://arxiv.org/abs/2412.07380) <br>

> **Response-level Ensemble** <br>
> Mixture-of-agents enhances large language model capabilities [![arXiv](https://img.shields.io/badge/arXiv-2406.04692-009688.svg)](https://arxiv.org/abs/2406.04692) <br>
> SMoA: Improving multi-agent large language models with sparse mixture-of-agents [![arXiv](https://img.shields.io/badge/arXiv-2411.03284-009688.svg)](https://arxiv.org/abs/2411.03284) <br>
> Symbolic mixture-of-experts: Adaptive skill-based routing for heterogeneous reasoning [![arXiv](https://img.shields.io/badge/arXiv-2503.05641-009688.svg)](https://arxiv.org/abs/2503.05641) <br>
> Do we truly need so many samples? Multi-LLM repeated sampling efficiently scale test-time compute [![arXiv](https://img.shields.io/badge/arXiv-2504.00762-009688.svg)](https://arxiv.org/abs/2504.00762) <br>
> More agents is all you need [![arXiv](https://img.shields.io/badge/arXiv-2402.05120-009688.svg)](https://arxiv.org/abs/2402.05120) <br>
> Rethinking mixture-of-agents: Is mixing different large language models beneficial? [![arXiv](https://img.shields.io/badge/arXiv-2502.00674-009688.svg)](https://arxiv.org/abs/2502.00674) <br>

### 📖Inference-Level Enhancement
**Self-driven Enhancement:**
> **Self-Ensemble Enhancement** <br>
> Self-consistency improves chain of thought reasoning in language models [![arXiv](https://img.shields.io/badge/arXiv-2203.11171-009688.svg)](https://arxiv.org/abs/2203.11171) <br>
> The curious case of neural text degeneration [![arXiv](https://img.shields.io/badge/arXiv-1904.09751-009688.svg)](https://arxiv.org/abs/1904.09751) <br>
> Chain-of-thought prompting elicits reasoning in large language models [![arXiv](https://img.shields.io/badge/arXiv-2201.11903-009688.svg)](https://arxiv.org/abs/2201.11903) <br>
> Accessing GPT-4 level mathematical olympiad solutions via Monte Carlo tree self-refine with LLaMa-3 8B [![arXiv](https://img.shields.io/badge/arXiv-2406.07394-009688.svg)](https://arxiv.org/abs/2406.07394) <br>
> CoT-based synthesizer: Enhancing LLM performance through answer synthesis [![arXiv](https://img.shields.io/badge/arXiv-2501.01668-009688.svg)](https://arxiv.org/abs/2501.01668) <br>
> Tree of thoughts: Deliberate problem solving with large language models [![arXiv](https://img.shields.io/badge/arXiv-2212.10001-009688.svg)](https://arxiv.org/abs/2212.10001) <br>
> **Self-Improvement Enhancement** <br>
> Reflexion: Language agents with verbal reinforcement learning [![arXiv](https://img.shields.io/badge/arXiv-2303.11366-009688.svg)](https://arxiv.org/abs/2303.11366) <br>
> Retroformer: Retrospective large language agents with policy gradient optimization [![arXiv](https://img.shields.io/badge/arXiv-2308.02151-009688.svg)](https://arxiv.org/abs/2308.02151) <br>
> Reflective multi-agent collaboration based on large language models [![arXiv](https://img.shields.io/badge/ACM-10.5555-009688.svg)](https://dl.acm.org/doi/10.5555/3737916.3742313) <br>
> ProAgent: Building proactive cooperative agents with large language models [![arXiv](https://img.shields.io/badge/arXiv-2308.11339-009688.svg)](https://arxiv.org/abs/2308.11339) <br>
> Hypothetical minds: Scaffolding theory of mind for multi-agent tasks with large language models [![arXiv](https://img.shields.io/badge/arXiv-2407.07086-009688.svg)](https://arxiv.org/abs/2407.07086) <br>

**Cooperation-driven Enhancement:**
> **Task Planning Based Collaboration** <br>
> HuggingGPT: Solving AI tasks with ChatGPT and its friends in Hugging Face [![arXiv](https://img.shields.io/badge/arXiv-2303.17580-009688.svg)](https://arxiv.org/abs/2303.17580) <br>
> Skeleton-of-thought: Prompting LLMs for efficient parallel generation [![arXiv](https://img.shields.io/badge/arXiv-2307.15337-009688.svg)](https://arxiv.org/abs/2307.15337) <br>
> Voyager: An open-ended embodied agent with large language models [![arXiv](https://img.shields.io/badge/arXiv-2305.16291-009688.svg)](https://arxiv.org/abs/2305.16291) <br>
> Scalable multi-robot collaboration with large language models: Centralized or decentralized systems? [![arXiv](https://img.shields.io/badge/arXiv-2309.15943-009688.svg)](https://arxiv.org/abs/2309.15943) <br>
> RoCo: Dialectic multi-robot collaboration with large language models [![arXiv](https://img.shields.io/badge/arXiv-2307.04738-009688.svg)](https://arxiv.org/abs/2307.04738) <br>
> Chameleon: Plug-and-play compositional reasoning with large language models [![arXiv](https://img.shields.io/badge/arXiv-2304.09842-009688.svg)](https://arxiv.org/abs/2304.09842) <br>
> TwoStep: Multi-agent task planning using classical planners and large language models [![arXiv](https://img.shields.io/badge/arXiv-2403.17246-009688.svg)](https://arxiv.org/abs/2403.17246) <br>
> AutoGen: Enabling next-gen LLM applications via multi-agent conversation [![arXiv](https://img.shields.io/badge/arXiv-2308.08155-009688.svg)](https://arxiv.org/abs/2308.08155) <br>
> Magis: LLM-based multi-agent framework for GitHub issue resolution [![arXiv](https://img.shields.io/badge/arXiv-2403.17927-009688.svg)](https://arxiv.org/abs/2403.17927) <br>

> **LLM–SLM Collaboration** <br>
> CITER: Collaborative inference for efficient large language model decoding with token-level routing [![arXiv](https://img.shields.io/badge/arXiv-2502.01976-009688.svg)](https://arxiv.org/abs/2502.01976) <br>
> CoGenesis: A framework collaborating large and small language models for secure context-aware instruction following [![arXiv](https://img.shields.io/badge/arXiv-2403.03129-009688.svg)](https://arxiv.org/abs/2403.03129) <br>
> Hybrid LLM: Towards low-latency multi-granularity routing between small and large models [![arXiv](https://img.shields.io/badge/arXiv-2404.14618-009688.svg)](https://arxiv.org/abs/2404.14618) <br>
> Collab-RAG: Collaborative retrieval-augmented generation using large and small language models [![arXiv](https://img.shields.io/badge/arXiv-2504.04915-009688.svg)](https://arxiv.org/abs/2504.04915) <br>
> CE-CoLLM: Cloud-edge cooperative LLM framework for enterprise knowledge management [![arXiv](https://img.shields.io/badge/arXiv-2411.02829-009688.svg)](https://arxiv.org/abs/2411.02829) <br>
> FedCoLLM: Federated collaboration of large and small language models for private data processing [![arXiv](https://img.shields.io/badge/arXiv-2411.11707-009688.svg)](https://arxiv.org/abs/2411.11707) <br>
> Collaboration of large language models and small recommendation models for device-cloud recommendation [![arXiv](https://img.shields.io/badge/arXiv-2501.05647-009688.svg)](https://arxiv.org/abs/2501.05647) <br>

> **Dual-System Collaboration** <br>
> Thinking, Fast and Slow [![arXiv](https://img.shields.io/badge/wikipedia-Thinking-009688.svg)](https://en.wikipedia.org/wiki/Thinking,_Fast_and_Slow) <br>
> DSADF: Thinking fast and slow for decision making [![arXiv](https://img.shields.io/badge/arXiv-2505.08189-009688.svg)](https://arxiv.org/abs/2505.08189) <br>
> Visual agents as fast and slow thinkers [![arXiv](https://img.shields.io/badge/arXiv-2408.08862-009688.svg)](https://arxiv.org/abs/2408.08862) <br>
> Thinking fast and slow: Efficient text-to-visual retrieval with transformers [![arXiv](https://img.shields.io/badge/arXiv-2103.16553-009688.svg)](https://arxiv.org/abs/2103.16553) <br>
> Interactive continual learning: Fast and slow thinking [![arXiv](https://img.shields.io/badge/arXiv-2403.02628-009688.svg)](https://arxiv.org/abs/2403.02628) <br>
> Thinking fast and slow in large language models [![arXiv](https://img.shields.io/badge/arXiv-2212.05206-009688.svg)](https://arxiv.org/abs/2212.05206) <br>
> RoboMamba: Multimodal state space model for efficient robot reasoning and manipulation [![arXiv](https://img.shields.io/badge/arXiv-2406.04339-009688.svg)](https://arxiv.org/abs/2406.04339) <br>


**Competition-involved Enhancement**
> **Multi-Agent Debate** <br>
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

> **Critique Mechanisms** <br>
> Multi-agent verification: Scaling test-time compute with multiple verifiers [![arXiv](https://img.shields.io/badge/arXiv-2502.20379-009688.svg)](https://arxiv.org/abs/2502.20379) <br>
> Critic-V: VLM critics help catch VLM errors in multimodal reasoning [![arXiv](https://img.shields.io/badge/arXiv-2411.18203-009688.svg)](https://arxiv.org/abs/2411.18203) <br>
> LLaMA-Berry: Pairwise optimization for O1-like olympiad-level mathematical reasoning [![arXiv](https://img.shields.io/badge/arXiv-2410.02884-009688.svg)](https://arxiv.org/abs/2410.02884) <br>
> CRITIC: Large language models can self-correct with tool-interactive critiquing [![arXiv](https://img.shields.io/badge/arXiv-2305.11738-009688.svg)](https://arxiv.org/abs/2305.11738) <br>
> TORA: A tool-integrated reasoning agent for mathematical problem solving [![arXiv](https://img.shields.io/badge/arXiv-2309.17452-009688.svg)](https://arxiv.org/abs/2309.17452) <br>
> Training language models to critique with multi-agent feedback [![arXiv](https://img.shields.io/badge/arXiv-2410.15287-009688.svg)](https://arxiv.org/abs/2410.15287) <br>
> Towards efficient LLM grounding for embodied multi-agent collaboration [![arXiv](https://img.shields.io/badge/arXiv-2405.14314-009688.svg)](https://arxiv.org/abs/2405.14314) <br>

**Self-Organizing Collective Optimization**
> **Heuristic Collective Optimization** <br>
> Model Swarms: Collaborative search to adapt LLM experts via swarm intelligence [![arXiv](https://img.shields.io/badge/arXiv-2410.11163-009688.svg)](https://arxiv.org/abs/2410.11163) <br>
> Heterogeneous Swarms: Jointly optimizing model roles and weights for multi-LLM systems [![arXiv](https://img.shields.io/badge/arXiv-2502.04510-009688.svg)](https://arxiv.org/abs/2502.04510) <br>
> SwarmPrompt: Swarm intelligence-driven prompt optimization using large language models [![arXiv](https://img.shields.io/badge/researchr-ShriyanSASA25-009688.svg)](https://researchr.org/publication/ShriyanSASA25) <br>
> Multi-agent systems powered by large language models: Applications in swarm intelligence [![arXiv](https://img.shields.io/badge/arXiv-2503.03800-009688.svg)](https://arxiv.org/abs/2503.03800) <br>
> Nature-inspired population-based evolution of large language models [![arXiv](https://img.shields.io/badge/arXiv-2503.01155-009688.svg)](https://arxiv.org/abs/2503.01155) <br>
> The society of hivemind: Multi-agent optimization of foundation model swarms to unlock the potential of collective intelligence [![arXiv](https://img.shields.io/badge/arXiv-2503.05473-009688.svg)](https://arxiv.org/abs/2503.05473) <br>
> EvoFlow: Evolving diverse agentic workflows on the fly [![arXiv](https://img.shields.io/badge/arXiv-2502.07373-009688.svg)](https://arxiv.org/abs/2502.07373) <br>
> EvoAgent: Towards automatic multi-agent generation via evolutionary algorithms [![arXiv](https://img.shields.io/badge/arXiv-2406.14228-009688.svg)](https://arxiv.org/abs/2406.14228) <br>

> **Automated Collective Optimization** <br>
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
> **Mathematics and Physics** <br>
> MathLearner: A large language model agent framework for learning to solve mathematical problems [![arXiv](https://img.shields.io/badge/arXiv-2408.01779-009688.svg)](https://arxiv.org/abs/2408.01779) <br>
> MA-LoT: Multi-agent lean-based long chain-of-thought reasoning enhances formal theorem proving [![arXiv](https://img.shields.io/badge/arXiv-2503.03205-009688.svg)](https://arxiv.org/abs/2503.03205) <br>
> MyCrunchGPT: A LLM assisted framework for scientific machine learning [![arXiv](https://img.shields.io/badge/arXiv-2306.15551-009688.svg)](https://arxiv.org/abs/2306.15551) <br>
> Automating mathematical proof generation using large language model agents and knowledge graphs [![arXiv](https://img.shields.io/badge/arXiv-2503.11657-009688.svg)](https://arxiv.org/abs/2503.11657) <br>
> LLMPhy: Complex physical reasoning using large language models and world models [![arXiv](https://img.shields.io/badge/arXiv-2411.08027-009688.svg)](https://arxiv.org/abs/2411.08027) <br>
> MechAgents: Large language model multi-agent collaborations can solve mechanics problems, generate new data, and integrate knowledge [![arXiv](https://img.shields.io/badge/arXiv-2311.08166-009688.svg)](https://arxiv.org/abs/2311.08166) <br>
> Physics-informed LLM-Agent for automated modulation design in power electronics systems [![arXiv](https://img.shields.io/badge/arXiv-2411.14214-009688.svg)](https://arxiv.org/abs/2411.14214) <br>
> MathChat: Converse to tackle challenging math problems with LLM agents [![arXiv](https://img.shields.io/badge/arXiv-2306.01337-009688.svg)](https://arxiv.org/abs/2306.01337) <br>

> **Chemistry and Material** <br>
> Moose-Chem: Large language models for rediscovering unseen chemistry scientific hypotheses [![arXiv](https://img.shields.io/badge/arXiv-2410.07076-009688.svg)](https://arxiv.org/abs/2410.07076) <br>
> ChemCrow: Augmenting large-language models with chemistry tools [![arXiv](https://img.shields.io/badge/arXiv-2304.05376-009688.svg)](https://arxiv.org/abs/2304.05376) <br>
> Towards an AI Co-Scientist [![arXiv](https://img.shields.io/badge/arXiv-2502.18864-009688.svg)](https://arxiv.org/abs/2502.18864) <br>
> An autonomous laboratory for the accelerated synthesis of novel materials [![arXiv](https://img.shields.io/badge/nature-s41586.023.06734.w-009688.svg)](https://www.nature.com/articles/s41586-023-06734-w) <br>
> Agent Laboratory: Using LLM agents as research assistants [![arXiv](https://img.shields.io/badge/arXiv-2501.04227-009688.svg)](https://arxiv.org/abs/2501.04227) <br>
> Chemist-X: Large language model-empowered agent for reaction condition recommendation in chemical synthesis [![arXiv](https://img.shields.io/badge/arXiv-2311.10776-009688.svg)](https://arxiv.org/abs/2311.10776) <br>
> Honeycomb: A flexible LLM-based agent system for materials science [![arXiv](https://img.shields.io/badge/arXiv-2409.00135-009688.svg)](https://arxiv.org/abs/2409.00135) <br>

> **Biology and Medicine** <br>
> Toward a Team of AI-made Scientists for Scientific Discovery from Gene Expression Data [![arXiv](https://img.shields.io/badge/arXiv-2402.12391-009688.svg)](https://arxiv.org/abs/2402.12391) <br>
> CRISPR-GPT: An LLM Agent for Automated Design of Gene-Editing Experiments [![arXiv](https://img.shields.io/badge/arXiv-2404.18021-009688.svg)](https://arxiv.org/abs/2404.18021) <br>
> BioDiscoveryAgent: An AI Agent for Designing Genetic Perturbation Experiments [![arXiv](https://img.shields.io/badge/arXiv-2405.17631-009688.svg)](https://arxiv.org/abs/2405.17631) <br>
> AgentMD: Empowering Language Agents for Risk Prediction with Large-scale Clinical Tool Learning [![arXiv](https://img.shields.io/badge/arXiv-2402.13225-009688.svg)](https://arxiv.org/abs/2402.13225) <br>
> ProtAgents: Protein discovery via large language model multi-agent collaborations combining physics and machine learning [![arXiv](https://img.shields.io/badge/arXiv-2402.04268-009688.svg)](https://arxiv.org/abs/2402.04268) <br>

**Autonomous Research:**
> **Autonomous Literature Analysis** <br>
> ChatCite: LLM Agent with Human Workflow Guidance for Comparative Literature Summary [![arXiv](https://img.shields.io/badge/arXiv-2403.02574-009688.svg)](https://arxiv.org/abs/2403.02574) <br>
> SurveyForge: On the Outline Heuristics, Memory-driven Generation, and Multi-dimensional Evaluation for Automated Survey Writing [![arXiv](https://img.shields.io/badge/arXiv-2503.04629-009688.svg)](https://arxiv.org/abs/2503.04629) <br>
> System for Systematic Literature Review Using Multiple AI Agents: Concept and an Empirical Evaluation [![arXiv](https://img.shields.io/badge/arXiv-2403.08399-009688.svg)](https://arxiv.org/abs/2403.08399) <br>
> ReviewAgents: Bridging the Gap between Human and AI-generated Paper Reviews [![arXiv](https://img.shields.io/badge/arXiv-2503.08506-009688.svg)](https://arxiv.org/abs/2503.08506) <br>

> **Autonomous Scientific Research** <br>
> ResearchAgent: Iterative research idea generation over scientific literature with large language models [![arXiv](https://img.shields.io/badge/arXiv-2404.07738-009688.svg)](https://arxiv.org/abs/2404.07738) <br>
> Dolphin: Closed-loop open-ended auto-research through thinking, practice, and feedback [![arXiv](https://img.shields.io/badge/arXiv-2501.03916-009688.svg)](https://arxiv.org/abs/2501.03916) <br>
> Many Heads Are Better Than One: Improved scientific idea generation by a LLM-based multi-agent system [![arXiv](https://img.shields.io/badge/arXiv-2410.09403-009688.svg)](https://arxiv.org/abs/2410.09403) <br>
> AutoAgent: A fully-automated and zero-code framework for LLM agents [![arXiv](https://img.shields.io/badge/arXiv-2502.05957-009688.svg)](https://arxiv.org/abs/2502.05957) <br>
> NovelSeek: When agent becomes the scientist – building closed-loop system from hypothesis to verification [![arXiv](https://img.shields.io/badge/arXiv-2505.16938-009688.svg)](https://arxiv.org/abs/2505.16938) <br>
> OriGene: A self-evolving virtual disease biologist automating therapeutic target discovery [![bioRxiv](https://img.shields.io/badge/researchgate-392477961-009688.svg)](https://www.researchgate.net/publication/392477961_OriGene_A_Self-Evolving_Virtual_Disease_Biologist_Automating_Therapeutic_Target_Discovery) <br>
> Chain of Ideas: Revolutionizing research via novel idea development with LLM agents [![arXiv](https://img.shields.io/badge/arXiv-2410.13185-009688.svg)](https://arxiv.org/abs/2410.13185) <br>
> Agent Laboratory: Using LLM agents as research assistants [![arXiv](https://img.shields.io/badge/arXiv-2501.04227-009688.svg)](https://arxiv.org/abs/2501.04227) <br>

### 📖Embodied Intelligence Research
**Centralized Control Paradigm:**
> **Task Allocation and Decision Making** <br>
> OPEX: A component-wise analysis of LLM-centric agents in embodied instruction following [![arXiv](https://img.shields.io/badge/arXiv-2403.03017-009688.svg)](https://arxiv.org/abs/2403.03017) <br>
> Long-horizon planning for multi-agent robots in partially observable environments [![arXiv](https://img.shields.io/badge/arXiv-2407.10031-009688.svg)](https://arxiv.org/abs/2407.10031) <br>
> Plan, Eliminate, and Track – Language models are good teachers for embodied agents [![arXiv](https://img.shields.io/badge/arXiv-2305.02412-009688.svg)](https://arxiv.org/abs/2305.02412) <br>
> LLM-Planner: Few-shot grounded planning for embodied agents with large language models [![arXiv](https://img.shields.io/badge/arXiv-2212.04088-009688.svg)](https://arxiv.org/abs/2212.04088) <br>
> CAPO: Cooperative plan optimization for efficient embodied multi-agent cooperation [![arXiv](https://img.shields.io/badge/arXiv-2411.04679-009688.svg)](https://arxiv.org/abs/2411.04679) <br>
> EMOS: Embodiment-aware heterogeneous multi-robot operating system with LLM agents [![arXiv](https://img.shields.io/badge/arXiv-2410.22662-009688.svg)](https://arxiv.org/abs/2410.22662) <br>
> LIP-LLM: Integrating linear programming and dependency graph with large language models for multi-robot task planning, IEEE Robotics and Automation Letters [![arXiv](https://img.shields.io/badge/IEEE-10803039-009688.svg)](https://ieeexplore.ieee.org/document/10803039) <br>
> SMART-LLM: Smart multi-agent robot task planning using large language models [![arXiv](https://img.shields.io/badge/arXiv-2309.10062-009688.svg)](https://arxiv.org/abs/2309.10062) <br>
> LAMMA-P: Generalizable multi-agent long-horizon task allocation and planning with LM-driven PDDL planner [![arXiv](https://img.shields.io/badge/arXiv-2409.20560-009688.svg)](https://arxiv.org/abs/2409.20560) <br>
> TANGO: Training-free embodied AI agents for open-world tasks [![arXiv](https://img.shields.io/badge/arXiv-2412.10402-009688.svg)](https://arxiv.org/abs/2412.10402) <br>
> Embodied task planning with large language models [![arXiv](https://img.shields.io/badge/arXiv-2307.01848-009688.svg)](https://arxiv.org/abs/2307.01848) <br>
> Co-NavGPT: Multi-robot cooperative visual semantic navigation using large language models [![arXiv](https://img.shields.io/badge/arXiv-2310.07937-009688.svg)](https://arxiv.org/abs/2310.07937) <br>
> Embodied Agent Interface: Benchmarking LLMs for embodied decision making [![arXiv](https://img.shields.io/badge/arXiv-2410.07166-009688.svg)](https://arxiv.org/abs/2410.07166) <br>
> Hazard Challenge: Embodied decision making in dynamically changing environments [![arXiv](https://img.shields.io/badge/arXiv-2401.12975-009688.svg)](https://arxiv.org/abs/2401.12975) <br>
> Large language models to the rescue: Deadlock resolution in multi-robot systems [![arXiv](https://img.shields.io/badge/arXiv-2404-009688.svg)](https://arxiv.org/abs/2404.00000) <br>
> NavGPT: Explicit reasoning in vision-and-language navigation with large language models [![arXiv](https://img.shields.io/badge/arXiv-2407.10031-009688.svg)](https://arxiv.org/abs/2407.10031) <br>
> LLM-powered Hierarchical Language Agent for Real-time Human-AI Coordination [![arXiv](https://img.shields.io/badge/arXiv-2312.15224-009688.svg)](https://arxiv.org/abs/2312.15224) <br>
> Voyager: An open-ended embodied agent with large language models [![arXiv](https://img.shields.io/badge/arXiv-2305.16291-009688.svg)](https://arxiv.org/abs/2305.16291) <br>
> LLM-Planner: Few-shot grounded planning for embodied agents with large language models [![arXiv](https://img.shields.io/badge/arXiv-2212.04088-009688.svg)](https://arxiv.org/abs/2212.04088) <br>

**Decentralized Interactive Paradigm:**
> **Agent Interaction Mechanism** <br>
> COMBO: Compositional world models for embodied multi-agent cooperation [![arXiv](https://img.shields.io/badge/arXiv-2404.10775-009688.svg)](https://arxiv.org/abs/2404.10775) <br>
> Evaluating Multi-Agent Coordination Abilities in Large Language Models [![arXiv](https://img.shields.io/badge/openreview-OEDM8mzbsl-009688.svg)](https://openreview.net/forum?id=OEDM8mzbsl) <br>
> Embodied LLM Agents Learn to Cooperate in Organized Teams [![arXiv](https://img.shields.io/badge/arXiv-2403.12482-009688.svg)](https://arxiv.org/abs/2403.12482) <br>
> S-Agents: Self-organizing Agents in Open-Ended Environments [![arXiv](https://img.shields.io/badge/arXiv-2402.04578-009688.svg)](https://arxiv.org/abs/2402.04578) <br>
> Hierarchical Auto-Organizing System for Open-Ended Multi-Agent Navigation [![arXiv](https://img.shields.io/badge/arXiv-2403.08282-009688.svg)](https://arxiv.org/abs/2403.08282) <br>
> Scalable Multi-Robot Collaboration with Large Language Models: Centralized or Decentralized Systems [![arXiv](https://img.shields.io/badge/arXiv-2309.15943-009688.svg)](https://arxiv.org/abs/2309.15943) <br>

### 📖Social Science Research
**Scope of Simulation:**
> **Scenario Simulation** <br>
> ChatLLM Network: More Brains, More Intelligence [![arXiv](https://img.shields.io/badge/arXiv-2304.12998-009688.svg)](https://arxiv.org/abs/2304.12998) <br>
> ChatGPT Research Group for Optimizing the Crystallinity of MOFs and COFs [![arXiv](https://img.shields.io/badge/ACS-10.1021-009688.svg)](https://pubs.acs.org/doi/10.1021/acscentsci.3c01087) <br>
> ChatEval: Towards Better LLM-based Evaluators through Multi-Agent Debate [![arXiv](https://img.shields.io/badge/arXiv-2308.07201-009688.svg)](https://arxiv.org/abs/2308.07201) <br>
> Social Skill Training with Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2404.04204-009688.svg)](https://arxiv.org/abs/2404.04204) <br>
> Debate on Graph: A Flexible and Reliable Reasoning Framework for Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2409.03155-009688.svg)](https://arxiv.org/abs/2409.03155) <br>
> CulturePark: Boosting Cross-Cultural Understanding in Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2405.15145-009688.svg)](https://arxiv.org/abs/2405.15145) <br>
> AI Hospital: Interactive Evaluation and Collaboration of LLMs as Intern Doctors [![arXiv](https://img.shields.io/badge/arXiv-2402-009688.svg)](https://arxiv.org/abs/2402.00000) <br>
> Encouraging Divergent Thinking in Large Language Models through Multi-Agent Debate [![arXiv](https://img.shields.io/badge/arXiv-2305.19118-009688.svg)](https://arxiv.org/abs/2305.19118) <br>
> Improving Factuality and Reasoning in Language Models through Multiagent Debate [![arXiv](https://img.shields.io/badge/arXiv-2305.14325-009688.svg)](https://arxiv.org/abs/2305.14325) <br>
> Beyond Natural Language: LLMs Leveraging Alternative Formats for Enhanced Reasoning and Communication [![arXiv](https://img.shields.io/badge/arXiv-2402.18439-009688.svg)](https://arxiv.org/abs/2402.18439) <br>
> A Scalable Communication Protocol for Networks of Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2410.11905-009688.svg)](https://arxiv.org/abs/2410.11905) <br>
> Blind Judgement: Agent-Based Supreme Court Modelling with GPT [![arXiv](https://img.shields.io/badge/arXiv-2301.05327-009688.svg)](https://arxiv.org/abs/2301.05327) <br>
> Exploring Large Language Models for Communication Games: An Empirical Study on Werewolf [![arXiv](https://img.shields.io/badge/arXiv-2309.04658-009688.svg)](https://arxiv.org/abs/2309.04658) <br>
> SimuCourt: Building Judicial Decision-Making Agents with Real-World Judgement Documents [![arXiv](https://img.shields.io/badge/arXiv-2403-009688.svg)](https://arxiv.org/abs/2403.00000) <br>
> TradingGPT: Multi-Agent System with Layered Memory and Distinct Characters for Enhanced Financial Trading Performance [![arXiv](https://img.shields.io/badge/arXiv-2309.03736-009688.svg)](https://arxiv.org/abs/2309.03736) <br>
> AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation [![arXiv](https://img.shields.io/badge/arXiv-2308.08155-009688.svg)](https://arxiv.org/abs/2308.08155) <br>
> MetaGPT: Meta Programming for Multi-Agent Collaborative Framework [![arXiv](https://img.shields.io/badge/arXiv-2308.00352-009688.svg)](https://arxiv.org/abs/2308.00352) <br>
> ChatDev: Communicative Agents for Software Development, ACL 2024 [![ACL](https://img.shields.io/badge/ACL-2024.810-009688.svg)](https://aclanthology.org/2024.acl-long.810) <br>
> AgentVerse: Facilitating Multi-Agent Collaboration and Exploring Emergent Behaviors [![arXiv](https://img.shields.io/badge/arXiv-2308.10848-009688.svg)](https://arxiv.org/abs/2308.10848) <br>
> Scalable Multi-Robot Collaboration with Large Language Models: Centralized or Decentralized Systems [![arXiv](https://img.shields.io/badge/arXiv-2309.15943-009688.svg)](https://arxiv.org/abs/2309.15943) <br>

> **Society Simulation** <br>
> The Wisdom of Partisan Crowds: Comparing Collective Intelligence in Humans and LLM-based Agents [![arXiv](https://img.shields.io/badge/arXiv-2311.09665-009688.svg)](https://arxiv.org/abs/2311.09665) <br>
> Generative Agent Simulations of 1,000 People [![arXiv](https://img.shields.io/badge/arXiv-2411.10109-009688.svg)](https://arxiv.org/abs/2411.10109) <br>
> Epidemic Modeling with Generative Agents [![arXiv](https://img.shields.io/badge/arXiv-2307.04986-009688.svg)](https://arxiv.org/abs/2307.04986) <br>
> ElectionSim: Massive Population Election Simulation Powered by Large Language Model Driven Agents [![arXiv](https://img.shields.io/badge/arXiv-2410.20746-009688.svg)](https://arxiv.org/abs/2410.20746) <br>
> On the Limits of Agency in Agent-Based Models [![arXiv](https://img.shields.io/badge/arXiv-2409.10568-009688.svg)](https://arxiv.org/abs/2409.10568) <br>
> Affordable Generative Agents [![arXiv](https://img.shields.io/badge/arXiv-2402.02053-009688.svg)](https://arxiv.org/abs/2402.02053) <br>
> Social Simulation in the Social Sciences: A Brief Overview, Social Science Computer Review [![arXiv](https://img.shields.io/badge/ACM-10.1177-009688.svg)](https://dl.acm.org/doi/10.1177/0894439313512975) <br>
> RecAgent: A Novel Simulation Paradigm for Recommender Systems [![arXiv](https://img.shields.io/badge/arXiv-2306.02552-009688.svg)](https://arxiv.org/abs/2306.02552) <br>
> From Skepticism to Acceptance: Simulating the Attitude Dynamics Toward Fake News [![arXiv](https://img.shields.io/badge/arXiv-2403.09498-009688.svg)](https://arxiv.org/abs/2403.09498) <br>
> "Guinea Pig Trials" Utilizing GPT: A Novel Smart Agent-Based Modeling Approach for Studying Firm Competition and Collusion [![arXiv](https://img.shields.io/badge/arXiv-2308.10974-009688.svg)](https://arxiv.org/abs/2308.10974) <br>
> Social Simulacra: Creating Populated Prototypes for Social Computing Systems [![arXiv](https://img.shields.io/badge/arXiv-2208.04024-009688.svg)](https://arxiv.org/abs/2208.04024) <br>
> Language Evolution for Evading Social Media Regulation via LLM-based Multi-Agent Simulation [![arXiv](https://img.shields.io/badge/arXiv-2405.02858-009688.svg)](https://arxiv.org/abs/2405.02858) <br>
> Can LLMs Understand Social Norms in Autonomous Driving Games? [![arXiv](https://img.shields.io/badge/arXiv-2408.12680-009688.svg)](https://arxiv.org/abs/2408.12680) <br>
> On Generative Agents in Recommendation [![arXiv](https://img.shields.io/badge/arXiv-2310.10108-009688.svg)](https://arxiv.org/abs/2310.10108) <br>
> Unveiling the Truth and Facilitating Change: Towards Agent-Based Large-Scale Social Movement Simulation [![arXiv](https://img.shields.io/badge/arXiv-2402.16333-009688.svg)](https://arxiv.org/abs/2402.16333) <br>
> Generative Agents: Interactive Simulacra of Human Behavior [![arXiv](https://img.shields.io/badge/arXiv-2304.03442-009688.svg)](https://arxiv.org/abs/2304.03442) <br>
> Emergence of Social Norms in Generative Agent Societies: Principles and Architecture [![arXiv](https://img.shields.io/badge/arXiv-2403.08251-009688.svg)](https://arxiv.org/abs/2403.08251) <br>

**Application of Simulation:**
> **Scientific Inquiry** <br>
> Simulating Opinion Dynamics with Networks of LLM-based Agents [![arXiv](https://img.shields.io/badge/arXiv-2311.09618-009688.svg)](https://arxiv.org/abs/2311.09618) <br>
> An LLM-Enhanced Agent-Based Simulation Tool for Information Propagation [![arXiv](https://img.shields.io/badge/IJCAI-2024.1007-009688.svg)](https://www.ijcai.org/proceedings/2024/1007.pdf) <br>
> Attention Mechanism for LLM-based Agents Dynamic Diffusion under Information Asymmetry [![arXiv](https://img.shields.io/badge/arXiv-2502.13160-009688.svg)](https://arxiv.org/abs/2502.13160) <br>
> EconAgent: Large Language Model-Empowered Agents for Simulating Macroeconomic Activities [![arXiv](https://img.shields.io/badge/arXiv-2310.10436-009688.svg)](https://arxiv.org/abs/2310.10436) <br>
> A Multi-LLM-Agent-Based Framework for Economic and Public Policy Analysis [![arXiv](https://img.shields.io/badge/arXiv-2502.16879-009688.svg)](https://arxiv.org/abs/2502.16879) <br>
> Can Generative AI Agents Behave Like Humans? Evidence from Laboratory Market Experiments [![arXiv](https://img.shields.io/badge/arXiv-2505.07457-009688.svg)](https://arxiv.org/abs/2505.07457) <br>

> **Problem-Solving** <br>
> Multi-Agent Collaboration Mechanisms: A Survey of LLMs [![arXiv](https://img.shields.io/badge/arXiv-2501.06322-009688.svg)](https://arxiv.org/abs/2501.06322) <br>
> Simulating Strategic Reasoning: Comparing the Ability of Single LLMs and Multi-Agent Systems to Replicate Human Behavior [![arXiv](https://img.shields.io/badge/arXiv-2402.08189-009688.svg)](https://arxiv.org/abs/2402.08189) <br>
> Review of Autonomous and Collaborative Agentic AI and Multi-Agent Systems for Enterprise Applications [![arXiv](https://img.shields.io/badge/researchgate-393232793-009688.svg)](https://www.researchgate.net/publication/393232793_Review_of_Autonomous_and_Collaborative_Agentic_AI_and_Multi-_Agent_Systems_for_Enterprise_Applications) <br>
> Agentic Large Language Models: A Survey [![arXiv](https://img.shields.io/badge/arXiv-2503.23037-009688.svg)](https://arxiv.org/abs/2503.23037) <br>

### 📖Auto-Programming
**Foundation-Oriented Programming:**
> **Simple Programming Problems** <br>
> AutoCoder: Enhancing code large language model with AIEV-INSTRUCT [![arXiv](https://img.shields.io/badge/arXiv-2405.14906-009688.svg)](https://arxiv.org/abs/2405.14906) <br>
> INTERVENOR: Prompting the Coding Ability of Large Language Models with the Interactive Chain of Repair [![arXiv](https://img.shields.io/badge/arXiv-2311.09868-009688.svg)](https://arxiv.org/abs/2311.09868) <br>
> AgentCoder: Multi-agent-based Code Generation with Iterative Testing and Optimisation [![arXiv](https://img.shields.io/badge/arXiv-2312.13010-009688.svg)](https://arxiv.org/abs/2312.13010) <br>
> AgileCoder: Dynamic Collaborative Agents for Software Development based on Agile Methodology [![arXiv](https://img.shields.io/badge/arXiv-2406.11912-009688.svg)](https://arxiv.org/abs/2406.11912) <br>
> AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation [![arXiv](https://img.shields.io/badge/arXiv-2308.08155-009688.svg)](https://arxiv.org/abs/2308.08155) <br>
> Self-Organized Agents: A LLM Multi-Agent Framework Toward Ultra Large-Scale Code Generation and Optimization [![arXiv](https://img.shields.io/badge/arXiv-2404.02183-009688.svg)](https://arxiv.org/abs/2404.02183) <br>
> Is Self-Repair a Silver Bullet for Code Generation? [![arXiv](https://img.shields.io/badge/arXiv-2306.09896-009688.svg)](https://arxiv.org/abs/2306.09896) <br>
> Test-driven Development and LLM-based Code Generation [![arXiv](https://img.shields.io/badge/arXiv-2402.13521-009688.svg)](https://arxiv.org/abs/2402.13521) <br>

> **Advanced Programming Problems** <br>
> Autonomous Large Language Model Agents Enabling Intent-Driven Mobile GUI Testing [![arXiv](https://img.shields.io/badge/arXiv-2311.08649-009688.svg)](https://arxiv.org/abs/2311.08649) <br>
> AxNav: Replaying Accessibility Tests from Natural Language  [![arXiv](https://img.shields.io/badge/arXiv-2310.02424-009688.svg)](https://arxiv.org/abs/2310.02424) <br>
> RCAgent: Cloud Root Cause Analysis by Autonomous Agents with Tool-Augmented Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2310.16340-009688.svg)](https://arxiv.org/abs/2310.16340) <br>
> AcFix: Guiding LLMs with Mined Common RBAC Practices for Context-Aware Repair of Access Control Vulnerabilities in Smart Contracts [![arXiv](https://img.shields.io/badge/arXiv-2403.06838-009688.svg)](https://arxiv.org/abs/2403.06838) <br>
> Multi-Role Consensus Through LLMs Discussions for Vulnerability Detection [![arXiv](https://img.shields.io/badge/arXiv-2403.14274-009688.svg)](https://arxiv.org/abs/2403.14274) <br>
> Measuring Coding Challenge Competence with APPS, NeurIPS Datasets and Benchmarks Track 2021 [![arXiv](https://img.shields.io/badge/arXiv-2311.08649-009688.svg)](https://arxiv.org/abs/2311.08649) <br>
> XCodeEval: A Large Scale Multilingual Multitask Benchmark for Code Understanding, Generation, Translation and Retrieval [![arXiv](https://img.shields.io/badge/arXiv-2303.03004-009688.svg)](https://arxiv.org/abs/2303.03004) <br>
> Codeforces [![Website](https://img.shields.io/badge/Web-Codeforces.com-blue.svg)](https://codeforces.com) <br>
> LeetCode [![Website](https://img.shields.io/badge/Web-LeetCode.com-blue.svg)](https://leetcode.com) <br>
> MapCoder: Multi-Agent Code Generation for Competitive Problem Solving [![arXiv](https://img.shields.io/badge/arXiv-2405.11403-009688.svg)](https://arxiv.org/abs/2405.11403) <br>
> FLOWS: Building Blocks of Reasoning and Collaborating AI [![arXiv](https://img.shields.io/badge/arXiv-2308.01285-009688.svg)](https://arxiv.org/abs/2308.01285) <br>

**Application-Oriented Programming:**
> **Software Development** <br>
> Software Development: Processes and Performance [![arXiv](https://img.shields.io/badge/researchgate-224101986-009688.svg)](https://www.researchgate.net/publication/224101986_Software_development_Processes_and_performance) <br>
> Model-driven Development of Complex Software: A Research Roadmap [![arXiv](https://img.shields.io/badge/IEEE-4221611-009688.svg)](https://ieeexplore.ieee.org/document/4221611) <br>
> Scaling Large-Language-Model-Based Multi-Agent Collaboration [![arXiv](https://img.shields.io/badge/arXiv-2406.07155-009688.svg)](https://arxiv.org/abs/2406.07155) <br>
> Self-Collaboration Code Generation via ChatGPT [![DOI](https://img.shields.io/badge/DOI-10.1145/3672459-009688.svg)](https://doi.org/10.1145/3672459) <br>
> Codepori: Large-scale System for Autonomous Software Development using Multi-Agent Technology [![arXiv](https://img.shields.io/badge/arXiv-2402.01411-009688.svg)](https://arxiv.org/abs/2402.01411) <br>
> CodeAgent: Autonomous Communicative Agents for Code Review [![ACL](https://img.shields.io/badge/ACL-2024.emnlp--main.632-009688.svg)](https://aclanthology.org/2024.emnlp-main.632) <br>
> Soen-101: Code Generation by Emulating Software Process Models using Large Language Model Agents [![arXiv](https://img.shields.io/badge/arXiv-2403.15852-009688.svg)](https://arxiv.org/abs/2403.15852) <br>
> Prompting Large Language Models to Tackle the Full Software Development Lifecycle: A Case Study [![arXiv](https://img.shields.io/badge/arXiv-2403.08604-009688.svg)](https://arxiv.org/abs/2403.08604) <br>
> Think-on-Process: Dynamic Process Generation for Collaborative Development of Multi-Agent System [![arXiv](https://img.shields.io/badge/arXiv-2409.06568-009688.svg)](https://arxiv.org/abs/2409.06568) <br>
> Multi-Agent Software Development through Cross-Team Collaboration [![arXiv](https://img.shields.io/badge/arXiv-2406.08979-009688.svg)](https://arxiv.org/abs/2406.08979) <br>
> Self-Evolving Multi-Agent Collaboration Networks for Software Development [![arXiv](https://img.shields.io/badge/arXiv-2410.16946-009688.svg)](https://arxiv.org/abs/2410.16946) <br>
> Experiential Co-Learning of Software-Developing Agents [![ACL](https://img.shields.io/badge/ACL-2024.acl--long.305-009688.svg)](https://aclanthology.org/2024.acl-long.305) <br>
> Iterative Experience Refinement of Software-Developing Agents [![arXiv](https://img.shields.io/badge/arXiv-2405.04219-009688.svg)](https://arxiv.org/abs/2405.04219) <br>
> ChatDev: Communicative Agents for Software Development [![ACL](https://img.shields.io/badge/ACL-2024.acl--long.810-009688.svg)](https://aclanthology.org/2024.acl-long.810) <br>
> A Systematic Approach to the Comparison of Roles in the Software Development Processes  
SPICE [![arXiv](https://img.shields.io/badge/researchgate-259779091-009688.svg)](https://www.researchgate.net/figure/Our-Systematic-Approach-for-Investigating-the-Roles-in-Software-Development-Environments_fig1_259779091) <br>
> Emphasizing Human Capabilities in Software Developmen [![arXiv](https://img.shields.io/badge/IEEE-1605185-009688.svg)](https://ieeexplore.ieee.org/document/1605185) <br>

> **Algorithm Engineering** <br>
> AutoKaggle: A Multi-Agent Framework for Autonomous Data Science Competitions [![arXiv](https://img.shields.io/badge/arXiv-2410.20424-009688.svg)](https://arxiv.org/abs/2410.20424) <br>
> Data Interpreter: An LLM Agent for Data Science [![arXiv](https://img.shields.io/badge/arXiv-2402.18679-009688.svg)](https://arxiv.org/abs/2402.18679) <br>
> PyBench: Evaluating LLM Agent on Various Real-World Coding Tasks [![arXiv](https://img.shields.io/badge/arXiv-2407.16732-009688.svg)](https://arxiv.org/abs/2407.16732) <br>
> SELA: Tree-Search Enhanced LLM Agents for Automated Machine Learning [![arXiv](https://img.shields.io/badge/arXiv-2410.17238-009688.svg)](https://arxiv.org/abs/2410.17238) <br>
> AutoML-Agent: A Multi-Agent LLM Framework for Full-Pipeline AutoML [![arXiv](https://img.shields.io/badge/arXiv-2410.02958-009688.svg)](https://arxiv.org/abs/2410.02958) <br>

### 📖GUI Operations
**Prompting-Based Methods:**
> **Single-Modal-Based** <br>
> Mobile-Agent-E: Self-evolving Mobile Assistant for Complex Tasks [![arXiv](https://img.shields.io/badge/arXiv-2501.11733-009688.svg)](https://arxiv.org/abs/2501.11733) <br>
> MobileExperts: A Dynamic Tool-enabled Agent Team in Mobile Devices [![arXiv](https://img.shields.io/badge/arXiv-2407.03913-009688.svg)](https://arxiv.org/abs/2407.03913) <br>
> Mobile-Agent-v2: Mobile Device Operation Assistant with Effective Navigation via Multi-agent Collaboration [![arXiv](https://img.shields.io/badge/arXiv-2406.01014-009688.svg)](https://arxiv.org/abs/2406.01014) <br>
> WebPilot: A Versatile and Autonomous Multi-agent System for Web Task Execution with Strategic Exploration [![arXiv](https://img.shields.io/badge/arXiv-2408.15978-009688.svg)](https://arxiv.org/abs/2408.15978) <br>
> CoLA: A Scalable Multi-agent Framework for Windows UI Task Automation [![arXiv](https://img.shields.io/badge/arXiv-2503.09263-009688.svg)](https://arxiv.org/abs/2503.09263) <br>

> **Multi-Modal-Based** <br>
> Mobile-agent-v: Learning mobile device operation through videoguided multi-agent collaboration  [![arXiv](https://img.shields.io/badge/arXiv-2502.17110-009688.svg)](https://arxiv.org/abs/2408.15978) <br>
> Mobile-Agent-v2: Mobile Device Operation Assistant with Effective Navigation via Multi-agent Collaboration [![arXiv](https://img.shields.io/badge/arXiv-2406.01014-009688.svg)](https://arxiv.org/abs/2406.01014) <br>

**Tuning-Based Methods:**
> **SFT-Based** <br>
> Octo-Planner: On-device Language Model for Planner-Action Agents [![arXiv](https://img.shields.io/badge/arXiv-2406.18082-009688.svg)](https://arxiv.org/abs/2406.18082) <br>
> PC Agent: While You Sleep, AI Works – A Cognitive Journey into Digital World [![arXiv](https://img.shields.io/badge/arXiv-2412.17589-009688.svg)](https://arxiv.org/abs/2412.17589) <br>

> **RL-Based** <br>
> MARLUI: Multi-agent Reinforcement Learning for Adaptive Point-and-Click UIs [![arXiv](https://img.shields.io/badge/arXiv-2209.12660-009688.svg)](https://arxiv.org/abs/2209.12660) <br>
> WebRL: Training LLM Web Agents via Self-evolving Online Curriculum Reinforcement Learning [![arXiv](https://img.shields.io/badge/arXiv-2411.02337-009688.svg)](https://arxiv.org/abs/2411.02337) <br>

### 📖Game Theory and Interactive Games
**Application in Game Theory:**
> **Behavior Evaluation** <br>
> Economics Arena for Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2401.01735-009688.svg)](https://arxiv.org/abs/2401.01735) <br>
> Can Large Language Model Agents Simulate Human Trust Behaviors? [![ICLR](https://img.shields.io/badge/NIPS-proceedings-009688.svg)](https://proceedings.neurips.cc/paper_files/paper/2024/file/1cb57fcf7ff3f6d37eebae5becc9ea6d-Paper-Conference.pdf) <br>
> Can Large Language Models Serve as Rational Players in Game Theory? A Systematic Analysis [![arXiv](https://img.shields.io/badge/arXiv-2312.05488-009688.svg)](https://arxiv.org/abs/2312.05488) <br>
> Playing Games with GPT: What Can We Learn About a Large Language Model from Canonical Strategic Games? [![SSRN](https://img.shields.io/badge/SSRN-4493398-009688.svg)](https://ssrn.com/abstract=4493398) <br>
> Playing Repeated Games with Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2305.16867-009688.svg)](https://arxiv.org/abs/2305.16867) <br>
> Investigating Emergent Goal-like Behaviour in Large Language Models using Experimental Economics [![arXiv](https://img.shields.io/badge/arXiv-2305.07970-009688.svg)](https://arxiv.org/abs/2305.07970) <br>
> Simulating Strategic Reasoning: Comparing the Ability of Single LLMs and Multi-Agent Systems to Replicate Human Behavior [![arXiv](https://img.shields.io/badge/arXiv-2402.08189-009688.svg)](https://arxiv.org/abs/2402.08189) <br>

> **Scenario Application** <br>
> Static Network Structure Cannot Stabilize Cooperation Among Large Language Model Agents [![arXiv](https://img.shields.io/badge/arXiv-2411.10294-009688.svg)](https://arxiv.org/abs/2411.10294) <br>
> Using Large Language Models to Simulate Multiple Humans and Replicate Human Subject Studies [![ICML](https://img.shields.io/badge/ICML-2023-009688.svg)](https://proceedings.mlr.press/v202/aher23a.html) <br>
> The Dynamics of Social Conventions in LLM Populations: Spontaneous Emergence, Collective Biases and Tipping Points [![arXiv](https://img.shields.io/badge/arXiv-2410.08948-009688.svg)](https://arxiv.org/abs/2410.08948) <br>
> Large Language Models Overcome the Machine Penalty When Acting Fairly but Not When Acting Selfishly or Altruistically [![arXiv](https://img.shields.io/badge/arXiv-2410.03724-009688.svg)](https://arxiv.org/abs/2410.03724) <br>
> Take Caution in Using LLMs as Human Surrogates [![PNAS](https://img.shields.io/badge/PNAS-10.1073/pnas.2501660122-009688.svg)](https://doi.org/10.1073/pnas.2501660122) <br>
> Game-Theoretic LLM: Agent Workflow for Negotiation Games [![arXiv](https://img.shields.io/badge/arXiv-2411.05990-009688.svg)](https://arxiv.org/abs/2411.05990) <br>
> Large language models as simulated economic agents: What can we learn from homo silicus? [![arXiv](https://img.shields.io/badge/arXiv-2301.07543-009688.svg)](https://arxiv.org/abs/2301.07543) <br>

> **Capability Enhancement** <br>
> Game-Theoretic LLM: Agent Workflow for Negotiation Games [![arXiv](https://img.shields.io/badge/arXiv-2411.05990-009688.svg)](https://arxiv.org/abs/2411.05990) <br>
> ALympics: Language Agents Meet Game Theory [![arXiv](https://img.shields.io/badge/arXiv-2311.03220-009688.svg)](https://arxiv.org/abs/2311.03220) <br>
> Strategic Reasoning with Language Models [![arXiv](https://img.shields.io/badge/arXiv-2305.19165-009688.svg)](https://arxiv.org/abs/2305.19165) <br>
> Steering Language Models with Game-Theoretic Solvers [![arXiv](https://img.shields.io/badge/arXiv-2402.01704-009688.svg)](https://arxiv.org/abs/2402.01704) <br>

**Application in Interactive Games:**
> **Constrained Interaction Environments** <br>
> Keep Calm and Explore: Language Models for Action Generation in Text-Based Games [![arXiv](https://img.shields.io/badge/arXiv-2010.02903-009688.svg)](https://arxiv.org/abs/2010.02903) <br>
> ReAct: Synergizing Reasoning and Acting in Language Models [![arXiv](https://img.shields.io/badge/arXiv-2210.03629-009688.svg)](https://arxiv.org/abs/2210.03629) <br>
> SwiftSage: A Generative Agent with Fast and Slow Thinking for Complex Interactive Tasks [![arXiv](https://img.shields.io/badge/arXiv-2305.17390-009688.svg)](https://arxiv.org/abs/2305.17390) <br>
> AriGraph: Learning Knowledge Graph World Models with Episodic Memory for LLM Agents [![arXiv](https://img.shields.io/badge/arXiv-2407.04363-009688.svg)](https://arxiv.org/abs/2407.04363) <br>
> ChessGPT: Bridging Policy Learning and Language Modeling [![arXiv](https://img.shields.io/badge/arXiv-2306.09200-009688.svg)](https://arxiv.org/abs/2306.09200) <br>
> PokerBench: Training Large Language Models to Become Professional Poker Players [![arXiv](https://img.shields.io/badge/arXiv-2501.08328-009688.svg)](https://arxiv.org/abs/2501.08328) <br>

> **Open-ended Interaction Environments** <br>
> Plan4MC: Skill Reinforcement Learning and Planning for Open-World Minecraft Tasks [![arXiv](https://img.shields.io/badge/arXiv-2303.16563-009688.svg)](https://arxiv.org/abs/2303.16563) <br>
> Describe, Explain, Plan and Select: Interactive Planning with Large Language Models Enables Open-World Multi-Task Agents [![arXiv](https://img.shields.io/badge/arXiv-2302.01560-009688.svg)](https://arxiv.org/abs/2302.01560) <br>
> MineDreamer: Learning to Follow Instructions via Chain-of-Imagination for Simulated-World Control [![arXiv](https://img.shields.io/badge/arXiv-2403.12037-009688.svg)](https://arxiv.org/abs/2403.12037) <br>
> MP5: A Multi-Modal Open-Ended Embodied System in Minecraft via Active Perception [![arXiv](https://img.shields.io/badge/arXiv-2312.07472-009688.svg)](https://arxiv.org/abs/2312.07472) <br>
> Llama Rider: Spurring Large Language Models to Explore the Open World [![arXiv](https://img.shields.io/badge/arXiv-2310.08922-009688.svg)](https://arxiv.org/abs/2310.08922) <br>
> Odyssey: Empowering Agents with Open-World Skills [![arXiv](https://img.shields.io/badge/arXiv-2407.15325-009688.svg)](https://arxiv.org/abs/2407.15325) <br>
> Motif: Intrinsic Motivation from Artificial Intelligence Feedback [![arXiv](https://img.shields.io/badge/arXiv-2310.00166-009688.svg)](https://arxiv.org/abs/2310.00166) <br>
> Voyager: An Open-Ended Embodied Agent with Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2305.16291-009688.svg)](https://arxiv.org/abs/2305.16291) <br>

## 📗Collective Intelligence 4.0 Era
![Figure 6](https://github.com/d-andelions/awesome-LLM-Driven-Collective-Intelligence/blob/main/figs/6.png)
### 🚢SAIL THE WAY TO THE INTELLIGENCE FUTURE
**Construction of Fundamental Capabilities** <br>
> PacelLM: Brain-Inspired Large Language Models for Long-Context Understanding [![arXiv](https://img.shields.io/badge/arXiv-2506.17310-009688.svg)](https://arxiv.org/abs/2506.17310) <br>
> Dynamic Skill Adaptation for Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2412.19361-009688.svg)](https://arxiv.org/abs/2412.19361) <br>
> Large Language Model Agent: A Survey on Methodology, Applications and Challenges [![arXiv](https://img.shields.io/badge/arXiv-2503.21460-009688.svg)](https://arxiv.org/abs/2503.214)

**Capability Differentiation** <br>
> Predicting Multi-Agent Specialization via Task Parallelizability [![arXiv](https://img.shields.io/badge/arXiv-2503.15703-009688.svg)](https://arxiv.org/abs/2503.15703) <br>
> Multiagent Conversational Online Learning for Adaptive LLM Response Identification [![arXiv](https://img.shields.io/badge/arXiv-2501.01849-009688.svg)](https://arxiv.org/abs/2501.01849) <br>
> Reflective Multi-Agent Collaboration Based on Large Language Models [![arXiv](https://img.shields.io/badge/ACM-10.5555-009688.svg)](https://dl.acm.org/doi/10.5555/3737916.3742313) <br>

**Cognitive Fusion** <br>
> Knowledge Graphs Meet Multi-Modal Learning: A Comprehensive Survey [![arXiv](https://img.shields.io/badge/arXiv-2402.05391-009688.svg)](https://arxiv.org/abs/2402.05391) <br>
> Achieving Unanimous Consensus in Decision Making Using Multiagents [![arXiv](https://img.shields.io/badge/arXiv-2504.02128-009688.svg)](https://arxiv.org/abs/2504.02128) <br>

**Dynamic Organization** <br>
> A Survey on Neural-Symbolic Learning Systems [![arXiv](https://img.shields.io/badge/arXiv-2111.08164-009688.svg)](https://arxiv.org/abs/2111.08164) <br>
> A Dynamic Credit Evaluation Approach Using Sensitivity-Optimized Weights for Supply Chain Finance [![arXiv](https://img.shields.io/badge/hrcak-446415-009688.svg)](https://hrcak.srce.hr/en/clanak/446415) <br>
> GPTSwarm: Language Agents as Optimizable Graphs [![arXiv](https://img.shields.io/badge/arXiv-2402.16823v3-009688.svg)](https://arxiv.org/abs/2402.16823v3) <br>

**Co-evolution** <br>
> Absolute Zero: Reinforced Self-Play Reasoning with Zero Data [![arXiv](https://img.shields.io/badge/arXiv-2505.03335-009688.svg)](https://arxiv.org/abs/2505.03335) <br>
> Generative Agent Simulations of 1,000 People [![arXiv](https://img.shields.io/badge/arXiv-2411.10109-009688.svg)](https://arxiv.org/abs/2411.10109) <br>
> Nature-Inspired Population-Based Evolution of Large Language Models [![arXiv](https://img.shields.io/badge/arXiv-2503.01155-009688.svg)](https://arxiv.org/abs/2503.01155) <br>
> The Society of HiveMind: Multi-Agent Optimization of Foundation Model Swarms to Unlock the Potential of Collective Intelligence [![arXiv](https://img.shields.io/badge/arXiv-2503.05473-009688.svg)](https://arxiv.org/abs/2503.05473) <br>

### ‼️Major Scientific Problems
**Unclear Emergence Mechanisms** <br>
> A defining feature of collective intelligence is emergence, where complex collective behaviors and capabilities surpass those of individual agents, potentially enabling phenomena like creative problem-solving and novel knowledge generation. However, the mechanisms underlying intelligent emergence remain elusive, impeding progress in this field, and research on how these phenomena arise is severely limited, especially within LLM-based collective systems. There is a lack of systematic explanations for the specific manifestations, triggering conditions, and evolutionary dynamics of emergence. Understanding these mechanisms is crucial for developing advanced collective intelligence systems. Future research requires systematic theoretical models to provide a foundation for exploring the transition from weak emergence (simple aggregation) to strong emergence (cognitive and creative breakthroughs).

**Bottlenecks in Continual Learning** <br>
> Current LLM-based collective systems face significant bottlenecks in continual learning, lacking robust long-term memory and dynamic interaction capabilities. This severely restricts their adaptability to complex environments and their ability to continuously evolve critical requirements for solving real-world problems. At the individual level, long-term memory management is inefficient, and knowledge forgetting and updating mechanisms in dynamic environments are underdeveloped, hindering the effective retention of historical experiences. At the collective level, there is a lack of unified memory-sharing architectures, leading to consistency conflicts during cross-entity knowledge transfer. Future research should focus on developing shared memory architectures, efficient information management (filtering, updating, forgetting), and collective-level meta-learning capabilities to enable true “lifelong learning” at the collective level, supporting sustained operation in dynamic scenarios.

**Difficulty in Achieving Consensus** <br>
> As LLM-based collective systems scale, achieving consensus in crossframework and cross-platform collaboration becomes crucial for leveraging specialized capabilities and achieving complex goals. However, there are two key issues hindering the consensus: (1) heterogeneity of LLM entities. Due to the heterogeneous architectures, various training data sources and fragmented protocols of different LLM entities, the bias and misunderstanding persist in the communication among models when facing a complex question, leading to disputes and disagreement; (2) local optimization. Without sufficient interoperability, the LLM entities tend to reach local optimal decisions that deviate from global goals in decentralized architectures, resulting in conflicting decision-making logics and inefficient capability coordination. Future efforts should prioritize establishing unified interaction and coordination standards while developing intelligent middleware to enable seamless interaction and scheduling among heterogeneous LLM entities, overcoming cross-platform collaboration challenges, and robustly achieving consensus to unlock the full potential of distributed collective intelligence.

**Uncontrollable and Unreliable Self-organization and Co-evolution** <br>
> The dynamic decentralized self-organization and unregulated co-evolution that empower collective intelligence also introduce significant challenges in terms of reliability and controllability. Unintended or adversarial emergent behaviors can lead to unpredictable and unmanageable consequences. Ensuring responsible progress towards AGI necessitates stricter ethical reviews, risk control mechanisms, and traceable, transparent decision-making processes. Crucially, system design must prioritize long-term alignment with human values and interests to ensure that development remains controllable, secure, and beneficial to society.

**Constraints of Computational Resources** <br>
 > The high demand for computational resources poses a substantial practical barrier. Driven by parallel inference across multiple large models, collective intelligence inevitably experiences exponential growth in computational and energy consumption as model sizes and task complexities increase, which restricts their widespread deployment and real-world applications. Addressing this issue requires exploring resource-efficient techniques from multiple perspectives, such as optimizing model architectures, implementing heterogeneous scheduling, compressing models, and utilizing lightweight agents. These strategies will enable collective intelligence systems to operate more economically and sustainably

**Incomplete Evaluation Frameworks** <br>
> Evaluating the progress of collective intelligence systems remains a significant challenge. Current metrics predominantly focus on end-to-end task completion, failing to capture the intricate collaboration mechanisms and emergent capabilities that characterize advanced collective intelligence systems. This oversight neglects crucial process factors such as collective structure evolution, cognitive consensus formation, and collaboration efficiency. As a result, there is an urgent need for multi-dimensional evaluation frameworks that incorporate metrics like interaction complexity, division of labor efficiency, policy consistency, and creative problem-solving ability. Such frameworks will provide comprehensive assessments better aligned with the goals of general collective intelligence.

## 📚Conclusion
> Collective intelligence, as an innovative and highly promising path towards AGI, is demonstrating a vast prospect of reshaping the field of artificial intelligence. Recently, the development of the powerful LLM-based entities has injected strong impetus into the development of more advanced collective intelligence framework. Driven by this, the fundamentaloriented collective intelligence, by enhancing data, model, and the reasoning process, has made remarkable progress in terms of performance optimization, efficiency improvement, and enhancement of robustness and security. The applicationriented collective intelligence, on the other hand, has come to the fore when dealing with complex long-range interactive tasks, achieving breakthrough applications in key fields such as scientific discovery, providing innovative and effective solutions for solving complex real-world problems. Looking ahead to future development, in the process of evolving from "augmenting intelligence through collectives" to "creating intelligence through collectives", LLM-based entities are expected to build a new capability system through fundamental capability construction, ability differentiation, cognitive integration, dynamic organization, and co-evolution, enabling efficient adaptation to complex and changing environments and realizing continuous evolution. However, the development of this field faces many serious challenges: the unknown emergence mechanism seriously hinders the in-depth understanding and effective regulation of collective intelligence; the bottleneck in continuous learning limits the long-term improvement of the intelligence level of the collective system; the lack of interoperability greatly restricts the exploration of cross-platform collaboration; the imperfect evaluation system makes it impossible to accurately measure the actual effectiveness of collective collaboration; the increase requirements in computing resource, and the potential risk of safety, reliability, and controllability pose a dual test to technological development and ethical security. Although the road ahead is full of challenges, with the unremitting exploration and in-depth research of the academic and industrial circles, it is expected that these problems will be gradually overcome, the theoretical and technical system of collective intelligence will be continuously improved, the collective intelligence driven by LLM will continue to develop and mature, steadily move towards the grand goal of AGI, and ultimately bring about a more profound transformation and huge value to human society.

