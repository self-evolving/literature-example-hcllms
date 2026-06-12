---
title: "How AI Impacts Skill Formation"
description: "Randomized experiments showing that AI assistance can impair skill development and conceptual understanding, even when it delivers short-term productivity gains."
type: paper
citekey: shen2026ai
authors:
  - Judy Hanwen Shen
  - Alex Tamkin
year: 2026
venue: arXiv
url: https://arxiv.org/abs/2601.20245
doi:
status: reference
tags:
  - paper
  - deskilling
  - evaluation
  - future-of-work
---

This paper investigates how AI assistance affects skill acquisition through a randomized experiment in which developers learned a new asynchronous programming library with and without AI help. The key finding is that AI use impairs conceptual understanding, code reading, and debugging abilities — without delivering significant efficiency gains on average. Participants who fully delegated coding tasks showed some productivity improvements, but at the cost of actually learning the library. The study identifies six distinct AI interaction patterns; three that involve active cognitive engagement preserve learning outcomes even when AI assistance is used. The conclusion is that AI-enhanced productivity is not a shortcut to competence, and AI assistance should be carefully integrated into workflows to avoid undermining skill formation, especially in safety-critical domains.

## Relevance to This Survey

This paper is a primary empirical anchor for two threads in [Reflections and New Directions for Human-Centered LLMs](../index.md):

### Chapter 7 — Future of Work ([Responsibly Deploying HCLLMs in the Workforce](../ziems2026reflections/07-applications/03-responsibly-deploying-hcllms-in-the-workforce.md))

Shen & Tamkin's findings provide direct evidence for the **cognitive deskilling** risk discussed in that chapter: when workers delegate tasks wholesale to LLMs, they miss the learning opportunities that build transferable domain expertise. Critically, the paper also shows that this risk is not uniform — the heterogeneity of outcomes across six interaction patterns supports the survey's argument that *how* workers engage with AI (iterative and critical vs. passive delegation) determines whether skill development is preserved or eroded. The paper is cited in the same section alongside work on novice vs. expert reliance patterns, grounding the survey's calls for intentional workflow design.

### Chapter 5 — Evaluation ([Societal-level Evaluation](../ziems2026reflections/05-evaluation/03-societal-level-evaluation.md))

The study exemplifies the randomized controlled trial (RCT) methodology advocated in the Societal-level Evaluation section: it measures not just task-completion speed but long-term conceptual outcomes, uses experimental control to distinguish AI effects from baseline performance, and surfaces behavioral impact patterns across interaction types. It illustrates why the survey argues for going beyond benchmark-based intrinsic evaluation toward extrinsic, longitudinal designs that capture the "sociotechnical gap" between controlled settings and real-world use.
