---
title: "ClassBot — Intent-Based Course Q&A Chatbot"
permalink: /projects/classbot/
---

## Overview

A lightweight **intent-based chatbot** for answering university course questions. Uses a bag-of-words pipeline with **NLTK preprocessing** and a **Keras feed-forward network** trained on `intents.json`, plus a simple CLI loop for interaction.

**Repo**: [github.com/faiazamin/ClassBot](https://github.com/faiazamin/ClassBot)

## Why?
Students often ask the same course questions repeatedly. I wanted a **small, editable chatbot** that teams can retrain by updating a single intents file—no complex pipelines or external services.

## Problem

- FAQ-style bots are brittle without an easy way to edit intents/responses.
- Many toy bots ship without **retraining scripts**, making updates manual.
- Preprocessing and model artifacts must stay in sync to avoid runtime errors.

## Approach

- **Data-driven intents**: Patterns and responses live in `intents.json`.
- **Preprocessing**: NLTK tokenization + lemmatization → bag-of-words vectors.
- **Model**: Keras/TensorFlow dense network trained via `trainingData.py`; artifacts (`chatbotmodel.h5`, `words.pkl`, `classes.pkl`) feed the CLI runner.
- **CLI**: `main.py` loads artifacts and runs an interactive loop with exit keywords (`bye`, `Goodbye`).

## Key Features

- Editable intents file (`intents.json`) with bundled examples.
- Training script to regenerate model + vocab/class pickles.
- Interactive CLI chatbot for quick demos.
- Clean repo layout: `main.py`, `trainingData.py`, `intents.json`, saved artifacts.

## Tech Stack

- **Python 3.9+**
- **TensorFlow / Keras**
- **NLTK** for tokenization and lemmatization
- **NumPy**

## My Contributions

- Built the preprocessing pipeline (tokenize, lemmatize, bag-of-words).
- Implemented the Keras feed-forward classifier and artifact saving/loading.
- Authored the training script and interactive CLI runner.
- Documented setup, NLTK data requirements, and retraining workflow.

## Setup & Run

- Install deps: `pip install tensorflow nltk numpy`
- Download NLTK data: `python -m nltk.downloader punkt wordnet`
- Run chatbot: `python main.py`
- Retrain after editing intents:
```bash
python trainingData.py
```

## Impact

- Delivers a **modifiable FAQ bot** that teams can refresh by editing one JSON file.
- Keeps preprocessing, model, and artifacts aligned to reduce runtime errors.
