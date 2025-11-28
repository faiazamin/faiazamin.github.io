---
title: "Acoustic Input for Headless Wearables"
permalink: /projects/acoustic-input-headless-wearables/
---

## Overview

A novel **acoustic input mechanism** for headless and ring-like wearable devices that uses **low-intensity sound** and **MFCC + spectrogram modeling** to detect subtle user actions.

Awarded **Samsung A2 patent grade** and selected for **KIPO patent filing**.
##Why
As wearables shrink (smart rings, loops), screens disappear. I realized that current 'headless' devices rely on voice (not private) or active buttons (bulky). I observed that people naturally tap surfaces to fidget or signal. I wondered: Could we repurpose the device's internal microphone—not to hear voice, but to 'feel' these mechanical taps?

## Problem

Headless wearables (e.g., rings, bands, loops) have:

- No screen
- Severely constrained input surface
- Strong power and compute limits

We wanted to enable **reliable, low-effort input** without adding new hardware.

## Approach

- ***Hardware***: Used the watch/phone’s built-in **microphones** as sensors
- ***Data Collection***:Captured **low-intensity acoustic events**
- ***Preprocessing***:Extracted **MFCCs and spectrogram features** on-device
- ***Analyzer***:Trained a lightweight classifier to distinguish input patterns vs noise

## My Contributions

I owned the research lifecycle from ideation to patent filing:

- Ideation: Theorized the use of structure-borne acoustics for input.

- Prototyping: Built the data collection rig and collected 500+ samples of 'tap' vs. 'noise.'

- Algorithm Design: Designed the specific MFCC feature extraction parameters to run on watch or Mobile device.

- Validation: Achieved >95% accuracy in controlled environments.

## Impact

- A2 internal patent grade → high novelty and strategic importance
- Pending patent filing at KIPO
- Demonstrated feasibility of **acoustic sensing as an input channel** for future wearable form factors

## Retrospective: Key Learnings
This project represented a pivotal evolution in my skillset, bridging the gap between theoretical ML and embedded reality. Initially limited in acoustic signal theory, I aggressively upskilled in spectrogram analysis and MFCC extraction, eventually mentoring my team on these implementations. Faced with extreme power constraints, I moved beyond standard training to master knowledge distillation and network pruning, optimizing our models for low powered watches and phones. Beyond technical execution, I developed critical IP strategy skills—learning to defend the commercial viability of 'headless input' against scrutiny from Samsung’s patent council, which ultimately secured the project's A2 Patent Grade.
