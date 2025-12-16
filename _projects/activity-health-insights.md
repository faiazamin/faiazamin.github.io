---
title: "Context-Aware Health Insights for Wearables"
permalink: /projects/context-aware-health/
---

## 🚀 Overview

I architected and prototyped an **activity-aware recommendation system** that fuses physiological sensing (PPG) with physical context (IMU) to deliver personalized health insights.

* **Status:** Showcased at **Samsung AI POC Exhibition** (Internal R&D Showcase).
* **Role:** Ideation Lead & Algorithm Engineer.

## ❓ Why?
Wearables today suffer from a **"Data Rich, Insight Poor"** paradox. They are excellent at logging 10,000 steps, but often fail to tell the user *what to do* with that data.

I realized that for a wearable to be a true health companion, it needs to shift from a passive "Quantified Self" tracker to an active **"Guided Self" agent**—one that anticipates user needs before they even ask.

## 📉 The Problem
Building a recommendation engine for a wrist-worn device presented three unique HCI challenges:

1.  **The Cold Start:** How to provide meaningful advice to a brand-new user with zero historical data?
2.  **Context Blindness:** A high heart rate means 'exercise' in the gym, but 'stress' in a board meeting. Simple sensors often fail to distinguish these states.
3.  **Notification Fatigue:** Generic "Time to move!" alerts are often ignored. We needed hyper-personalization to ensure engagement.

## 💡 The Approach
*Due to Samsung Research IP regulations, specific algorithmic weights and proprietary logic are omitted.*

I designed a **Multi-Layer Data Fusion** engine to determine user intent:

* **Physiological Layer:** Aggregates heart rate variability and intensity metrics.
* **Physical Layer:** Analyzes IMU (inertial measurement unit) data to classify micro-activities.
* **Situational Layer:** Leverages device state to infer social context (ensuring data privacy by processing entirely on-device).

**The Hybrid Inference Strategy:**
To solve the "Cold Start" problem, I implemented a multimodal learning model. The system initially bootstraps using **heuristic clinical best practices**, then seamlessly transitions to **collaborative filtering** as user interaction data accumulates, progressively tailoring the timing of insights to individual behavior.

## 🛠️ My Contributions
I owned the logic design and collaborated on the Proof of Concept (PoC) development:

* **Algorithm Design:** Designed the 'Activity Context' logic that differentiates between 'sedentary work' (mental focus) and 'sedentary relaxation' (leisure), allowing for context-appropriate interventions.
* **Data Strategy:** Curated a baseline dataset to power the initial heuristic models.
* **Edge Optimization:** Engineered the inference engine to run efficiently on **resource-constrained wearable APs** (Application Processors), ensuring zero impact on battery life.

## 🏆 Impact
* **Recognition:** Selected for showcase at the **Samsung AI POC Exhibition**, demonstrating the potential for next-gen health features.
* **Thought Leadership:** Helped shape internal R&D thinking around **"context-aware health intelligibility"**—moving the product strategy from simple data logging to actionable intelligence.

## 🧠 Retrospective: Key Learnings
Navigating the complexity of this system taught me to synthesize diverse sensor streams into coherent user context.

* **Adaptive Systems:** I learned that an effective recommendation engine must balance immediate utility (heuristics) with long-term personalization (learning).
* **Communication:** Showcasing this work at the AI Exhibition honed my ability to translate complex **sensor fusion concepts** into compelling narratives for diverse stakeholders—a capability I view as essential for impactful research.