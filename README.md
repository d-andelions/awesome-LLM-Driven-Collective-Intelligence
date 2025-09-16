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
- [Collective Intelligence 1.0 and 2.0 Era](#collective-intelligence-1.0-and-2.0-era)
  - [Data-Level Enhancement](#data-level-enhancement)
  - [Model-Level Enhancement](#model-level-enhancement)
  - [Inference-Level Enhancement](#inference-level-enhancement)
- [Collective Intelligence 3.0 Era](#application-oriented-ci)
  - [Scientific Discovery & Autonomous Research](#scientific-discovery)
  - [Embodied Intelligence](#embodied-intelligence)
  - [Social Science Research](#social-science-research)
  - [Auto-Programming](#auto-programming)
  - [GUI Operations](#gui-operations)
  - [Game Theory & Interactive Games](#game-theory--interactive-games)
- [Collective Intelligence 4.0 Era](#future-challenges)
- [Contributing](#contributing)

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
> 
