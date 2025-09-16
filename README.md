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
> Collective intelligence [![arXiv](https://img.shields.io/badge/springer-10.1007-009688.svg)](https://link.springer.com/article/10.1007/s12599-010-0114-8) <br>
