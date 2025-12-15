---
title: "Acoustic Input for Headless Wearables"
permalink: /projects/acoustic-input-headless-wearables/
---

## Overview

A novel **acoustic input mechanism** for Samsung wearable devices that uses **low-intensity sound** and **MFCC + spectrogram modeling** to detect subtle user actions.

Awarded **Samsung A2 patent grade**.

## Why ?
As wearables shrink, screens disappear. I realized that current 'headless' devices rely on voice (not private) or active buttons (bulky). I wondered: Could we repurpose the device's internal microphone—not to hear voice, but to 'feel' activities?
## Problem

Wearables have:

- Limited visual interface
- Severely constrained input surface
- Strong power and compute limits

We wanted to enable **reliable, low-effort input** without adding new hardware.

## Approach *(High-level, NDA-compliant)*

**Note**: *Specific architectural parameters and circuit designs are omitted to comply with Samsung R&D intellectual property regulations. The following is a high-level overview of the methodology.*

- *Hardware*: Used the Samsung Engineering devices' built-in **microphones** as sensors
- *Data Collection*: Captured **low-intensity acoustic events**
- *Preprocessing*: Extracted **MFCCs and spectrogram features** on-device
- *Analyzer*: Trained a lightweight classifier to distinguish input patterns vs noise

## My Contributions

I led this project across the full research lifecycle:

- **Conceptualization**: Proposed  acoustics as a private input modality for  wearables  
- **Prototyping**: Built data collection pipelines and curated labeled acoustic interaction datasets  
- **Algorithm Design**: Developed low-power acoustic feature processing suitable for wearable deployment  
- **Validation**: Demonstrated reliable differentiation between target input and environmental noise  


## Impact

- A2 internal patent grade → high novelty and strategic importance
- Pending patent application filing 
- Demonstrated feasibility of **acoustic sensing as an input channel** for future wearable form factors

## Retrospective: Key Learnings
This project represented a pivotal evolution in my skillset, bridging the gap between theoretical ML and embedded reality. Initially limited in acoustic signal theory, I aggressively upskilled in spectrogram analysis and MFCC extraction, eventually mentoring my team on these implementations. Faced with extreme power constraints, I moved beyond standard training to master knowledge distillation and network pruning, optimizing our models for low powered watches and phones. Beyond technical execution, I developed critical IP strategy skills—learning to defend the commercial viability of 'headless input' against scrutiny from Samsung’s patent council, which ultimately secured the project's A2 Patent Grade.
