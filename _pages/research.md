---
layout: page
permalink: /research/
title: research
description: My main research interests and ongoing work
nav: true
nav_order: 1
---

My research focuses on developing AI systems that are both powerful and interpretable. I am particularly interested in bridging the gap between high-performing machine learning models and human-understandable decision-making processes.

---

## Rule-Based Learning

I am deeply interested in **rule-based learning systems** that produce interpretable decision rules. Unlike black-box models, rule-based classifiers generate explicit IF-THEN rules that practitioners can examine, validate, and trust.

My work in this area focuses on **continuous optimization techniques** for learning optimal rule bases. Traditional approaches often rely on combinatorial search, but continuous formulations enable the use of gradient-based methods and evolutionary algorithms to find better solutions more efficiently.

**Key aspects of my work:**

- Genetic algorithms for fuzzy rule optimization
- Differentiable rule learning approaches
- Balancing rule accuracy with interpretability
- Penalty-based aggregation for rule combination

**Related publications:**
{% bibliography --query @*[title ~= rule] %}

---

## Explainable Classification

A central theme in my research is **explainable classification**: building classifiers that not only achieve high accuracy but also provide meaningful explanations for their predictions.

I believe that for AI to be deployed responsibly in critical domains like healthcare, law, and security, we need models that humans can understand and verify. My work on [Ex-Fuzzy](/exfuzzy/) directly addresses this need by providing a toolkit for creating explainable fuzzy classifiers.

**Research directions:**

- Fuzzy rule-based classifiers with linguistic interpretability
- Post-hoc explanation methods for deep learning
- Ensemble methods with explainable components (e.g., the Krypteia ensemble)
- Visual explanations for image classification

**Related publications:**
{% bibliography --query @*[title ~= Explainable || title ~= xai || title ~= interpretable] %}

---

## Uncertainty Quantification with Incomplete Information

Real-world data is often incomplete, imprecise, or affected by various sources of uncertainty. My research addresses how to make reliable decisions when working with such data.

I am particularly interested in:

- **Interval-valued data**: When measurements have inherent bounds of uncertainty
- **Fuzzy representations**: When categories have gradual rather than sharp boundaries
- **Aggregation under uncertainty**: Combining multiple uncertain sources of information

This work has applications in brain-computer interfaces, medical diagnosis, and any domain where data quality varies.

**Related publications:**
{% bibliography --query @*[title ~= Interval || title ~= uncertainty || title ~= aggregation] %}

---

## Fuzzy Logic

**Fuzzy logic** provides the mathematical foundation for much of my work. It allows us to model imprecise concepts using degrees of membership rather than binary true/false values, making it particularly suited for human-centric AI applications.

My contributions to fuzzy logic include:

- **Fuzzy integrals**: Generalizations of the Sugeno and Choquet integrals for data fusion
- **Fuzzy clustering**: Using fuzzy membership for community detection and anomaly detection
- **Interval-valued fuzzy sets**: Extensions that capture additional uncertainty in membership degrees
- **Type-2 fuzzy systems**: Handling uncertainty about the fuzzy sets themselves

I maintain [Ex-Fuzzy](/exfuzzy/), a Python library that makes fuzzy logic accessible to the broader machine learning community.

**Related publications:**
{% bibliography --query @*[title ~= Fuzzy || title ~= fuzzy] %}

---

## Collaboration

I am always open to collaborations on these topics. If you are interested in working together or have questions about my research, please feel free to [reach out](mailto:j.fumanal-idocin@essex.ac.uk).
