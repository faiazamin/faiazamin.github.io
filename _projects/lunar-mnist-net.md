---
title: "Lunar MNIST Net — Minimal PyTorch Trainer"
permalink: /projects/lunar-mnist-net/
---

## Overview

A lean **PyTorch MNIST model + training helper** with a pytest-backed harness. Provides a ready-to-import `MNISTNet` and a `train()` helper so examples and tests run directly from the repo root.

**Repo**: [github.com/faiazamin/lunar_mnist_net](https://github.com/faiazamin/lunar_mnist_net)

## Why?
I wanted a **tiny, reproducible MNIST baseline** to share patterns for structuring small research repos: clean package exports, testable entry points, and zero-friction setup for new contributors.

## Problem

- Many toy MNIST repos lack **tests** and **import-stable packaging**, causing `ModuleNotFoundError` when running from root.
- Onboarding should be **one command** (`pytest`) without puzzling over PYTHONPATH tweaks.

## Approach

- Packaged the code under `src/` with exports that alias cleanly to `src.*` from repo root.
- Wrote a **single training helper** (`train()`) that returns a model instance for tests/examples.
- Added **pytest coverage** to enforce import discipline and catch regressions.

## Key Features

- `MNISTNet` implementation in `src/model.py`.
- `train()` helper in `src/train.py` used by tests and examples.
- Pytest suite under `test/` runnable from the repository root.
- Guidance for fixing common import issues without manual PYTHONPATH edits.

## Tech Stack

- **Python 3.8+**
- **PyTorch** (CPU or CUDA)
- **pytest**

## My Contributions

- Authored the `MNISTNet` model and the training helper.
- Structured the package so `from src.*` imports work from repo root.
- Wrote pytest cases to keep the model/train loop verifiable.
- Documented setup, troubleshooting, and contributor expectations.

## Setup & Run

- Create/activate a venv, then install: `pip install torch torchvision pytest`.
- Run tests: `pytest -q` from the repo root.
- Example usage:
```python
from src.train import train
from src.model import MNISTNet

model = train()
print(hasattr(model, "forward"))
```

## Impact

- Offers a **minimal, testable MNIST baseline** for quick experimentation or teaching.
- Demonstrates repo structure patterns that avoid import pain and keep examples reproducible.
