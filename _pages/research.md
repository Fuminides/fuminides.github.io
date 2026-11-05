---
layout: page
permalink: /research/
title: Research
description: Some notes about my research interests.
nav: true
nav_order: 1
---

My research focuses on developing AI systems that are both powerful and interpretable. I am particularly interested in bridging the gap between what can be used in a laboratory for benchmark, and what can actually be deployed in real-life settings.

---

## Explainable AI

I am deeply interested in **rule-based learning systems** that produce interpretable decision rules. Unlike black-box models, rule-based classifiers generate explicit IF-THEN rules that practitioners can examine, validate, and trust. I am explicitly interested in those that are particularly simple, and can be validated by humans. My work in this area focuses on developing new applications for these methods and continuous optimization techniques for learning optimal rule bases.

**Fuzzy logic** provides the mathematical foundation for much of this work. It allows us to model imprecise concepts using degrees of membership rather than binary true/false values, which makes it particularly suited for rules that read like the ones people would write. I maintain [Ex-Fuzzy](/software/), a Python library that makes fuzzy logic accessible to the broader machine learning community.

---

## Uncertainty Quantification with Incomplete Information

Real-world data is often incomplete, imprecise, or affected by the chaotic nature of real life processes. My research addresses how to make reliable decisions when working with such data. I am particularly interested in dynamic feature selection, and robust systems with low hardware resources.

---

## AI Safety

A model that is going to act on our behalf should know what it knows. I study the **beliefs that large language models hold** about the state of a problem while they solve it: where that belief lives inside the model, how it changes as new evidence arrives, and how far it is from what a rational observer would conclude. To do this I use games with a hidden state, where the optimal belief is known, and learn a small latent model of the LLM's own transitions between turns. The same setting lets me stress a model with rules, taboos and incentives, and measure when it breaks them.

The first results are in [What does the model think it knows?](https://fuminides.github.io/llm-belief-jepa/), a technical report with a page where you can watch, clue by clue and turn by turn, how Qwen3.5 models update their beliefs against the Bayesian answer and how they play a text dungeon. The code and results are [on GitHub](https://github.com/Fuminides/llm-belief-jepa).

---

## Collaboration

I am always open to collaborations on these topics. If you are interested in working together or have questions about my research, please feel free to [reach out](mailto:j.fumanal-idocin@essex.ac.uk).
