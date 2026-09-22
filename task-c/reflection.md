# Task C — Research Reflection

> **BAFAD Accelerated Research Track · Fall 2026**
> Complete **after** finishing Tasks A and B.

---

## Instructions

Write your responses directly in this file (replace the placeholder text).
Aim for **150–200 words total** across both questions.
Be specific — reference your actual experience with the data and code.

---

## Question 1 — Connecting the Work to Research

*After completing Tasks A and B, how does hands-on data exploration relate to the research problem described in **Anomaly Detection in Tactical Sensor Streams** (the document you read before the Canvas quiz)?*

Consider: What patterns did you observe in the SMAP data? How might those patterns complicate or inform the design of an autoencoder-based anomaly detector?

**Your response (75–100 words):**

Hands-on exploration connects the sensor-stream anomaly-detection problem to observable patterns. In Task A, 24 of 500 timesteps were labelled anomalous, but their channel 00 values overlapped the normal range. The heatmap also showed repeating structure across channels. An autoencoder would therefore need to learn normal relationships and temporal patterns, rather than simply flag large individual values. Training on normal data and validating reconstruction-error thresholds could help. Task B reinforced that filtering and missing-value handling affect statistical conclusions, so preprocessing choices also need careful checks in an anomaly-detection pipeline.

---

## Question 2 — Self-Assessment of Readiness

*What specific gaps in your current knowledge — Python skills, statistics concepts, or ML background — do you expect to encounter if you join the research group? What is your plan for addressing them?*

Be honest. There are no wrong answers — this helps us plan the onboarding schedule.

**Your response (75–100 words):**

I would describe my current experience as intermediate. To prepare for the research group, I plan to strengthen the transition from exploratory analysis to building and evaluating machine-learning models. My next study priorities are time-window preparation, autoencoder training, and choosing anomaly thresholds without using test data. I also plan to practice pandas grouped operations and check how missing values affect results. I will work through small reproducible examples, compare model predictions with known labels, and keep notes on errors and questions to discuss during onboarding.

---

*Submission: commit this file to your fork and include it in the GitHub repo URL you submit on Canvas.*
