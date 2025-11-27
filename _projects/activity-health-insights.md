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

## Problem

Wearables collect rich physiological and behavioral data, but:

- Users often see only step counts and generic summaries
- Insights are not tightly linked to **what they were doing** when patterns changed

We aimed to **connect activity context** with **interpretable health feedback**.

## Approach

- Built a **sensor fusion pipeline** combining IMU, PPG, and contextual logs
- Detected **activity segments** (e.g., walking, resting, workout)
- Generated **explanatory insights**, e.g.:

  > “During your evening walk, your heart rate recovered faster than last week — a sign of improving cardio fitness.”

- Designed the system to be **lightweight enough** to run on Galaxy Watches and phones

## My Contributions

- Led model + pipeline design for **activity classification + insight generation**
- Implemented data processing and feature extraction in Python
- Collaborated on UX flows within the Galaxy wearable ecosystem
- Prepared technical documentation and internal demo materials

## Impact

- Recognized and showcased in the **Samsung AI POC Exhibition**
- Helped shape internal thinking around **context-aware health intelligibility** for everyday users