---
title: "Acoustic Interaction for Compact Wearables"
permalink: /projects/acoustic-interaction-wearables/
---

## 🚀 Overview

I led the research and prototyping of a **novel input mechanism** for next-generation wearable devices. The project focused on enabling discrete interaction on ultra-compact form factors without relying on physical buttons or traditional touch interfaces.

* **Status:** Awarded **Samsung A2 Patent Grade** (Internal Innovation Award) & Selected for Patent Filing.
* **Role:** Lead Researcher & Software Engineer.

## ❓ Why?
As wearables shrink, display real-estate vanishes. I realized that current **ultra-compact** devices generally rely on voice (not private) or active buttons (bulky).

I observed that people naturally tap surfaces to fidget or signal. I wondered: **Could we repurpose the device's internal acoustic sensors—not to hear voice, but to 'feel' these mechanical activities?**

## 💡 The Approach
*Due to Samsung Research IP regulations, specific technical implementations and sensor architectures are omitted.*

I hypothesized that **structure-borne signals** could serve as a proxy for user intent. Instead of adding new hardware, I developed a software-defined sensing pipeline that repurposes **existing embedded sensors** to detect micro-mechanical interactions (e.g., taps, gestures) on the device chassis.

My contribution focused on the end-to-end pipeline:
* **Data Strategy:** Designed protocols to collect samples of intended user interactions vs. environmental noise.
* **Edge AI:** Developed and optimized a lightweight classification model to run locally on the device, ensuring privacy and low latency.

## 🏆 Impact
* **Innovation:** Validated that software-only solutions can establish a robust input channel on constrained surfaces.
* **Recognition:** The project passed internal novelty searches and was awarded an **A2 Innovation Grade** by the Samsung.
* **Feasibility:** Achieved high detection accuracy in controlled user studies.

## 🧠 Retrospective: Key Learnings
This project represented a pivotal evolution in my skillset, bridging the gap between theoretical ML and embedded reality.

* **Technical Upskilling:** Initially limited in signal theory, I aggressively upskilled in **spectrogram analysis** and **MFCC feature extraction**, eventually mentoring my team on these implementations.
* **Edge Optimization:** Faced with extreme power constraints, I moved beyond standard training to master **knowledge distillation** and **network pruning**, optimizing our models for low-powered wearable chipsets.
* **Strategic Growth:** Beyond technical execution, I developed critical IP strategy skills—learning to defend the commercial viability of **novel input modalities** against scrutiny from the Patent Council, which ultimately secured the project's A2 Grade.