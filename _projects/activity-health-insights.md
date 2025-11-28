---
title: "Activity-Based Health Insight Recommendation for Galaxy Watch"
permalink: /projects/activity-health-insights/
---

## Overview

An **activity-aware health insight system** that fuses:

- IMU (activity, movement)
- PPG (heart rate, intensity)
- Pressure & contextual data (Samsung Health)

to deliver **personalized health insights** on Galaxy Watches and phones.

Showcased at the **Samsung AI POC Exhibition (SRBD)**.

## Why ?
Wearables today suffer from a 'Data Rich, Insight Poor' paradox. They are excellent at logging 10,000 steps, but terrible at telling you what do with them. I realized that for a wearable to be a true health companion, it needs to shift from a passive Quantified Self tracker to an active Guided Self agent—anticipating user needs before they ask.

## Problem

Building a recommendation engine for a wrist-worn device presented three unique challenges:

- *The Cold Start*: How to provide meaningful advice to a brand-new user with zero historical data?
- *Context Blindness*: A high heart rate means 'exercise' in the gym, but 'stress' in a meeting. Simple sensors cannot distinguish this context.
- *Notification Fatigue*: Generic 'Time to move!' alerts are often ignored. We needed hyper-personalization to ensure user engagement.

## Approach
**Note**: *Specific algorithmic weights and proprietary logic are omitted to comply with Samsung R&D intellectual property regulations. The following is a high-level overview of the methodology.*

*Data Fusion* (Input Layers): The engine aggregates three concurrent data streams:

- Physiological Layer: Samsung Health Data.
- Physical Layer: IMU data to classify micro-activities.
- Situational Layer: visuals, acoustics, app data.
  
*Adaptive Inference* (The Intelligence): To solve the "Cold Start" problem for new users, I implemented a Hybrid Learning Strategy. The system initially uses heuristic bootstrapping based on clinical best practices, then seamlessly transitions to collaborative filtering as user interaction data accumulates, tailoring the timing of insights to individual behavior.


## My Contributions

I ideated the process and actively collaborated in PoC development:

- *Algorithm Design*: Designed the 'Activity Context' logic that differentiates between 'sedentary work' and 'sedentary relaxation.'
- *Data Preparation*: Gathered dataset for generalized 'best practices'
- *On-Device Optimization*: Engineered the inference engine to run efficiently on the Galaxy Watch’s limited processor, ensuring zero impact on battery life.


## Impact

- Recognized and showcased in the **Samsung AI POC Exhibition**
- Helped shape internal thinking around **context-aware health intelligibility** for everyday users

## Retrospective: Key Learnings
Navigating the complexity of this system taught me to synthesize diverse sensor streams into coherent user context, moving beyond static rules to design adaptive 'Cold Start' workflows that evolve with the user. I learned that an effective recommendation engine must balance immediate utility (heuristics) with long-term personalization (learning). Beyond the technical architecture, showcasing this work at the Samsung AI POC Exhibition honed my public speaking and communication skills, teaching me to translate complex sensor fusion concepts into compelling narratives for diverse stakeholders—a capability I view as essential for impactful research.
