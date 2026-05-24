# ML & Deep Learning Formula Cheat Sheets

Compact LaTeX formula references for theory-focused machine learning and deep
learning review.

This repository contains two standalone PDF review sheets designed for quick
mathematical lookup. They emphasize formulas, notation, objectives, update
rules, evaluation quantities, model decisions, tensor shapes where relevant,
and compact derivations without requiring readers to search across full lecture
notes or textbooks.

The content follows the study-material scope covered by each sheet. It is not
intended to be an exhaustive textbook-level reference or a universal catalog of
every machine learning and deep learning topic. Instead, it is a focused
mathematical review resource for beginners and learners who want to strengthen
their theoretical foundation.

These sheets are not tutorials and do not replace complete courses or
textbooks. They are compact references for revision and formula checking.

## Download

| Sheet | Focus | PDF |
| --- | --- | --- |
| Deep Learning Formula Cheat Sheet | Neural networks, optimization, CNNs, sequence models, attention, Transformers, and tensor shapes | [Download PDF](./main.pdf) |
| Machine Learning Formula & Decision Sheet | Regression, classification, evaluation, diagnosis, tree ensembles, clustering, recommenders, and reinforcement learning | [Download PDF](./machine-learning-formula-decision-sheet.pdf) |

## Preview

### Machine Learning Formula & Decision Sheet

<p align="center">
  <img src="assets/preview/machine-learning-contents.png" width="47%" alt="Machine learning preview: contents">
  <img src="assets/preview/machine-learning-lasso.png" width="47%" alt="Machine learning preview: Lasso and Elastic Net formulas">
</p>
<p align="center">
  <img src="assets/preview/machine-learning-roc-auc.png" width="47%" alt="Machine learning preview: PR-AUC and model diagnosis formulas">
  <img src="assets/preview/machine-learning-deep-q.png" width="47%" alt="Machine learning preview: Q-learning and Deep Q Networks">
</p>

### Deep Learning Formula Cheat Sheet

<p align="center">
  <img src="assets/preview/deep-learning-contents.png" width="47%" alt="Deep learning preview: contents">
  <img src="assets/preview/deep-learning-optimization.png" width="47%" alt="Deep learning preview: optimization formulas">
</p>
<p align="center">
  <img src="assets/preview/deep-learning-attention.png" width="47%" alt="Deep learning preview: attention decoder formulas">
  <img src="assets/preview/deep-learning-transformer.png" width="47%" alt="Deep learning preview: Transformer formulas">
</p>

## About the Sheets

### Machine Learning Formula & Decision Sheet

A mathematical reference for machine learning theory and model-based
decisions. It combines objectives, update rules, compact derivations, metric
interpretation, and judgment-style checkpoints for questions where selecting
the correct method matters as much as recalling the formula.

### Deep Learning Formula Cheat Sheet

A compact formula and tensor-shape reference for deep learning. It focuses on
forward computations, losses, gradient flows, optimizer updates,
architecture-specific objectives, and shape rules.

## Coverage

| Machine Learning Formula & Decision Sheet | Deep Learning Formula Cheat Sheet |
| --- | --- |
| Linear, polynomial, and logistic regression | Neural-network notation and forward propagation |
| Cost functions, gradient descent, regularization, Lasso, and Elastic Net | Loss functions, backpropagation, initialization, and optimization |
| Evaluation, ROC-AUC, PR-AUC, bias/variance, and error analysis | Regularization and batch normalization |
| Neural-network foundations, decision trees, bagging, and boosting | CNNs, classic architectures, object detection, and YOLO |
| K-means, anomaly detection, and recommender systems | Face recognition and neural style transfer |
| Reinforcement learning, Bellman equations, Q-learning, and Deep Q Networks | RNN/GRU/LSTM, embeddings, Seq2Seq, attention, and Transformers |

## Design Principles

- Keep entries compact and formula-focused.
- Prefer display mathematics for central objectives and updates.
- Define notation close to the formulas that use it.
- Include shapes where dimensions clarify the computation.
- Include short derivations where they explain an update, metric, or decision rule.
- Prefer concise tables and notes over textbook-length prose.

## Artifacts

| Artifact | Status |
| --- | --- |
| `machine-learning-formula-decision-sheet.pdf` | Available as the current Machine Learning review sheet. |
| `main.pdf` | Available as the current Deep Learning formula sheet. |
| Deep Learning LaTeX source in `main.tex` and `sections/` | Included in this repository and built by GitHub Actions. |

The current tagged Deep Learning draft is
[v0.2.0 - Formula Hierarchy and Core Extensions](https://github.com/Jerry-0821/ml-dl-formula-cheatsheet/releases/tag/v0.2.0).

## Building From Source

The currently included LaTeX source builds the Deep Learning sheet:

```bash
make pdf
```

Manual fallback:

```bash
latexmk -pdf main.tex
```

GitHub Actions builds `main.pdf` and uploads it as the
`deep-learning-formula-cheatsheet-pdf` artifact.

## Source and Scope Policy

Each sheet follows the scope of the study materials used to prepare it.
External references may be used to verify standard formulas, notation, shapes,
or mathematical correctness, but the sheets are not intended to silently
expand into complete textbooks. The goal is a reliable, compact mathematical
review resource within the covered topic range.
