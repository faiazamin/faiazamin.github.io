---
title: "Acoustic Input for Headless Wearables"
permalink: /projects/acoustic-input-headless-wearables/
---

## Overview

A novel **acoustic input mechanism** for headless and ring-like wearable devices that uses **low-intensity sound** and **MFCC + spectrogram modeling** to detect subtle user actions.

Awarded **Samsung A2 patent grade** and selected for **KIPO patent filing**.

## Problem

Headless wearables (e.g., rings, bands, loops) have:

- No screen
- Severely constrained input surface
- Strong power and compute limits

We wanted to enable **reliable, low-effort input** without adding new hardware.

## Approach

- Use the watch/phone’s built-in **microphones** as sensors
- Emit or capture **low-intensity acoustic events**
- Extract **MFCCs and spectrogram features** on-device
- Train a lightweight classifier to distinguish input patterns vs noise

## My Contributions

- Designed the **signal processing pipeline** (MFCC + spectrogram)
- Implemented data collection app and logging
- Built the training + evaluation pipeline in Python/TensorFlow
- Optimized feature extraction and model runtime under tight budgets

## Impact

- A2 internal patent grade → high novelty and strategic importance
- Pending patent filing at KIPO
- Demonstrated feasibility of **acoustic sensing as an input channel** for future wearable form factors