# 5511-a3-nn-transformers

## Installation & Running

1. From the project root, install the pinned dependencies via `uv sync` (it reads `pyproject.toml` and `uv.lock`).
2. Open `src/nn_transformers.ipynb` with your preferred Jupyter interface (`jupyter lab`/`notebook`) to train or evaluate the models and inspect the experiments.

## Project Structure

```
.
├── data/                      # data references described in data.md
├── output/                    # generated artifacts (training loss plots, metrics, etc.)
├── src/
│   └── nn_transformers.ipynb  # notebook implementing FFNN and transformer experiments from scratch
├── LICENSE
├── README.md
├── pyproject.toml
└── uv.lock                    # lockfile kept in sync via `uv sync`
```

## Overview

This assignment implements both a textbook feed-forward neural network (FFNN) and a transformer-style architecture from scratch, focusing on NLP use cases. The notebook loads the datasets documented in `data/data.md`, codes up the model layers and training loops manually, and visualizes training dynamics such as the saved `transformers_training_loss.png`. Outputs such as logs, figures, and checkpointed weights live in `output/` so you can compare experiments or continue training later.
