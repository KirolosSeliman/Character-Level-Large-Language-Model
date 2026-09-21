# Character-Level Large Language Model

Early-stage exploration of a character-level language model, following Andrej Karpathy's
"makemore" series. The notebook loads a dataset of 32,033 names (`names.txt`) and starts
building up the bigram statistics that form the foundation of character-level text
generation.

> Work in progress — the notebook currently covers data loading and bigram exploration.

## Contents

- `CLLLM.ipynb` — Jupyter notebook: loads `names.txt`, inspects the vocabulary, and
  explores character bigram counts with start/end markers (`<S>`, `<E>`)
- `names.txt` — dataset of ~32k names used for training

## Running it

```bash
pip install jupyter numpy
jupyter notebook CLLLM.ipynb
```

## Background

This follows the approach from Karpathy's
[Zero to Hero: makemore series](https://www.youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKc),
starting from the simplest possible model — a bigram character-level language model —
before scaling up to MLPs and transformers.
