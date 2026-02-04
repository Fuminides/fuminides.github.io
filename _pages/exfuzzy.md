---
layout: page
permalink: /exfuzzy/
title: Ex-Fuzzy
description: A Python library for explainable AI through fuzzy logic programming
nav: true
nav_order: 4
---

**Ex-Fuzzy** is a modern, explainable fuzzy logic library for Python that I developed together with [Prof. Javier Andreu-Perez](https://scholar.google.com/citations?user=example). It provides comprehensive capabilities for explainable artificial intelligence through fuzzy logic programming, with a focus on accessibility and visualization.

## Key Features

- **Explainable AI**: Create interpretable models using fuzzy association rules that humans can understand and verify
- **Rich Visualizations**: Built-in tools for visualizing fuzzy sets, membership functions, and rule bases
- **Scikit-learn Compatible**: Follows the scikit-learn API for seamless integration with existing ML pipelines
- **High Performance**: Optional GPU support for computationally intensive tasks
- **Comprehensive Support**: Classification, regression, and rule mining capabilities
- **Multiple Fuzzy Set Types**: Support for Type-1, Interval Type-2, and General Type-2 fuzzy sets

## Installation

```bash
pip install ex-fuzzy
```

## Quick Example

```python
from ex_fuzzy import evolutionary_fit as gfs
from ex_fuzzy import utils

# Load your data
X_train, y_train, X_test, y_test = utils.load_data()

# Create and train a fuzzy classifier
fuzzy_clf = gfs.FuzzyRulesClassifier()
fuzzy_clf.fit(X_train, y_train)

# Get interpretable rules
print(fuzzy_clf.print_rules())

# Make predictions
predictions = fuzzy_clf.predict(X_test)
```

## Links

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  <div class="repo p-2">
    <a href="https://github.com/Fuminides/ex-fuzzy">
      <i class="fab fa-github"></i> GitHub Repository
    </a>
  </div>
  <div class="repo p-2">
    <a href="https://fuminides.github.io/ex-fuzzy/">
      <i class="fas fa-book"></i> Documentation
    </a>
  </div>
  <div class="repo p-2">
    <a href="https://pypi.org/project/ex-fuzzy/">
      <i class="fab fa-python"></i> PyPI Package
    </a>
  </div>
</div>

---

## Papers Using Ex-Fuzzy

### Core Library Paper

**Ex-Fuzzy: A Library for Symbolic Explainable AI Through Fuzzy Logic Programming** (Neurocomputing, 2024)
*Fumanal-Idocin & Andreu-Perez*
The foundational paper describing the library's architecture, capabilities, and design philosophy. Introduces the scikit-learn compatible API and visualization tools.

---

### New Methods Implemented in Ex-Fuzzy

**A Fast Interpretable Fuzzy Tree Learner** (arXiv, 2025)
*Fumanal-Idocin, Fernandez-Peralta & Andreu-Perez*
Introduces a novel fuzzy decision tree algorithm optimized for speed and interpretability. The implementation is available in Ex-Fuzzy as an alternative to rule-based classifiers.

**Compact Rule-Based Classifier Learning via Gradient Descent** (arXiv, 2025)
*Fumanal-Idocin, Fernandez-Peralta & Andreu-Perez*
Implements gradient-based optimization for learning compact fuzzy rule bases, extending Ex-Fuzzy beyond genetic algorithms to differentiable learning.

**Reliable Classification with Conformal Learning and Interval-Type 2 Fuzzy Sets** (FUZZ-IEEE, 2025)
*Fumanal-Idocin & Andreu-Perez*
Combines conformal prediction with Interval Type-2 fuzzy sets for uncertainty-aware classification. Extends Ex-Fuzzy's IT2 capabilities with reliability guarantees.

**Crisp Complexity of Fuzzy Classifiers** (FUZZ-IEEE, 2025)
*Fernandez-Peralta, Fumanal-Idocin & Andreu-Perez*
Proposes new complexity metrics for fuzzy classifiers. Uses Ex-Fuzzy to empirically study the relationship between rule complexity and model performance.

---

### Applications Using Ex-Fuzzy

**ArtXAI: Explainable Artificial Intelligence Curates Deep Representation Learning for Artistic Images Using Fuzzy Techniques** (IEEE Trans. Fuzzy Systems, 2023)
*Fumanal-Idocin, Andreu-Perez, Cordón, Hagras & Bustince*
Uses Ex-Fuzzy to provide explainable classification of artistic images by learning fuzzy rules over deep learning embeddings. Demonstrates how fuzzy rules can interpret neural network representations.

**Interpreting Contrastive Embeddings in Specific Domains with Fuzzy Rules** (FUZZ-IEEE, 2024)
*Fumanal-Idocin, Jamalifard & Andreu-Perez*
Applies Ex-Fuzzy to interpret contrastive learning embeddings (e.g., CLIP) using domain-specific fuzzy rules, bridging black-box representations with human-understandable concepts.

---

### Comparison and Benchmarking

**Efficient Online Generation of Fuzzy Measures via Aggregation Functions** (Information Fusion, 2026)
*Gonzalez-Garcia, Horanská, Beliakov & Bustince*
Uses Ex-Fuzzy as a baseline for comparing fuzzy measure generation methods, demonstrating the library's utility as a benchmarking tool in the fuzzy systems community.

---

## News and Updates

- **2025**: New fuzzy tree learner and gradient-based optimization methods added
- **2025**: Three papers accepted at FUZZ-IEEE 2025 using Ex-Fuzzy
- **2024**: Ex-Fuzzy 2.0 released with improved performance and new features
- **2024**: Core library paper published in [Neurocomputing](https://doi.org/10.1016/j.neucom.2024.128048)
- **2023**: ArtXAI paper published in IEEE Trans. Fuzzy Systems
- **2023**: Initial public release on PyPI

---

## Citation

If you use Ex-Fuzzy in your research, please cite:

```bibtex
@article{FUMANALIDOCIN2024128048,
  title = {Ex-Fuzzy: A library for symbolic explainable AI through fuzzy logic programming},
  journal = {Neurocomputing},
  pages = {128048},
  year = {2024},
  author = {Javier Fumanal-Idocin and Javier Andreu-Perez},
  doi = {https://doi.org/10.1016/j.neucom.2024.128048}
}
```

---

## Contributing

Ex-Fuzzy is open source under the AGPL v3 license. Contributions, bug reports, and feature requests are welcome on [GitHub](https://github.com/Fuminides/ex-fuzzy/issues).

If you are a BSc/MSc student looking for thesis projects, I am actively supervising work on extending Ex-Fuzzy functionalities. Feel free to [contact me](mailto:j.fumanal-idocin@essex.ac.uk).
