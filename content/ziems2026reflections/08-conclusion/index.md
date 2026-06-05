---
title: "Conclusion"
type: paper-section
paper: ziems2026reflections
tags:
  - paper
  - paper-section
---

The development of large language models has reached a critical juncture. It is no longer sufficient to ask only what these models are capable of doing. We must also grapple with questions such as who is—and is not—involved in and accounted for in the creation of LLMs; what the impacts of these models are at both the individual and societal level; and which values and principles these technologies uphold and promote. This survey examines how such human-centered principles are inherently intertwined with the design, training, and deployment of LLMs.

Ultimately, the trajectory of LLM development must be guided by more than technical benchmarks and capability milestones. The questions of inclusion, impact, and values explored in this survey are not peripheral concerns to be addressed after the fact; they are foundational to what these systems become and who they serve. By centering human-centered principles at every stage of the LLM lifecycle, from design and data curation to training and deployment, researchers and practitioners can work toward models that are not only more capable, but also more equitable, accountable, and aligned with the diverse needs of the people they affect. The path forward demands a broader coalition of voices, a more expansive notion of responsibility, and a sustained commitment to ensuring that progress in AI is measured not only by what these models can do, but by the kind of world their development helps to build.

## Acknowledgments

The idea for this manuscript originated in the Fall 2024 offering of Stanford's CS 329X course on HCLLMs, taught by the instructor Diyi Yang and assistants Rose E. Wang and Caleb Ziems. Diyi Yang developed the initial structure and outline of the paper. The enrolled students collaborated on a first draft of the manuscript as part of their coursework, with each student pair assigned responsibility for drafting a subsection of the survey according to the course assignment structure. The teaching assistants subsequently reviewed, graded, and provided feedback on these drafts. In Winter 2025, a subset of students continued to revise and expand the manuscript under the primary direction of Rose E. Wang and the secondary direction of Caleb Ziems.

Caleb Ziems and Dora Zhao largely re-wrote and restructured the manuscript, with significant conceptual revisions and new chapters, to produce the current version. This revision phase was supported by additional contributions from Sunny Yu and Advit Deepak. All authors reviewed and approved the final manuscript.

The core authors were jointly responsible for deciding on and writing the paper in its final form. The core are as follows:

-   **Diyi Yang** designed the overall structure, chapter outline, and course material that initialized this survey. She supervised the project and provided guidance on the direction and scope of the survey at every stage.

-   **Caleb Ziems** restructured the paper from its initial conception, wrote [Introduction](../01-introduction/) and [Data for HCLLMs](../03-data/), and co-wrote [NLP for HCLLMs](../04-nlp/), [Evaluation](../05-evaluation/), and [Responsible Human-Centered LLMs](../06-responsible/). He also contributed to structuring and reviewing all student drafts, and co-lead the second round of student revisions.

-   **Dora Zhao** restructured the paper from its initial conception, wrote [HCI for HCLLMs](../02-hci/) and [Case Study: HCLLMs and the Future of Work](../07-applications/), and co-wrote [NLP for HCLLMs](../04-nlp/), [Evaluation](../05-evaluation/), and [Responsible Human-Centered LLMs](../06-responsible/). Dora also co-designed the figures.

Additionally, the leadership of this work included:

-   **Rose E. Wang** contributed to structuring and reviewing all student drafts. She led the second round of student revisions.

-   **Matthew Jörke** contributed [From Human-Centered Design Challenges to Technical Artifacts](../02-hci/04-from-human-centered-design-challenges-to-technical-artifacts) and provided suggestions on [HCI for HCLLMs](../02-hci/) more broadly.

-   **Ahmad Rushdi** contributed guidance and final edits.

Student contributions are as follows:

-   **Anshika Agarwal** co-wrote [Quantitative Evaluation](../05-evaluation/01-model-level-evaluations) and edited [Evaluation](../05-evaluation/).

-   **Harshvardhan Agarwal** helped with the course paper and edited [Evaluation](../05-evaluation/).

-   **Gabriela Aranguiz-Dias** co-wrote [Quantitative Evaluation](../05-evaluation/01-model-level-evaluations).

-   **Aditri Bhagirath** helped with the course paper and second-round student edits.

-   **Justine Breuch** co-wrote [Bias and Fairness Evaluation](../05-evaluation/02-human-level-evaluations).

-   **Huanxing Chen** helped with the course paper.

-   **Ruishi Chen** helped with the course paper.

-   **Sarah Chen** co-wrote the first draft of [Interpretable and Explainable HCLLMs](../06-responsible/01-interpretable-and-explainable-hcllms).

-   **Advit Deepak** co-wrote [Responsible Human-Centered LLMs](../06-responsible/).

-   **Haocheng Fan** co-wrote [Human-Level Evaluations](../05-evaluation/02-human-level-evaluations)

-   **William Fang** helped with the course paper and second-round student edits.

-   **Cat Gonzales Fergesen** helped with the course paper.

-   **Daniel Frees** co-wrote [Supervised Fine-tuning for HCLLMs](../04-nlp/01-supervised-fine-tuning-for-hcllms).

-   **Tian Gao** co-wrote [Safety Evaluations](../05-evaluation/02-human-level-evaluations).

-   **Ziqing Huang** co-wrote [Safety Evaluations](../05-evaluation/02-human-level-evaluations).

-   **Vishal Jain** co-wrote [Safe HCLLMs](../06-responsible/03-safe-hcllms)

-   **Yucheng Jiang** co-wrote [Human-Level Evaluations](../05-evaluation/02-human-level-evaluations)

-   **Kirill Kalinin** helped with second-round student edits.

-   **Su Doga Karaca** co-wrote [Human-Level Evaluations](../05-evaluation/02-human-level-evaluations) and edited [Evaluation](../05-evaluation/).

-   **Arpandeep Khatua** helped with the course paper and second-round student edits.

-   **Teland La** helped with the course paper.

-   **Isabelle Levent** helped with the course paper.

-   **Miranda Li** helped with the course paper and second-round student edits.

-   **Xinling Li** co-wrote [Consent and Ownership](../03-data/03-consent-and-ownership).

-   **Yongce Li** co-wrote [Expanding Data Sources: Synthetic and Non-Traditional Data](../03-data/04-expanding-data-sources-synthetic-and-non-traditional-data).

-   **Angela Liu** helped with the course paper and second-round student edits.

-   **Minsik Oh** co-wrote [Quantitative Evaluation](../05-evaluation/01-model-level-evaluations), and edited [Evaluation](../05-evaluation/).

-   **Nathan J. Paek** helped with the course paper and second-round student edits.

-   **Anthony Qin** helped with the course paper.

-   **Emily Redmond** co-wrote [Scaling Human Centered LLMs](../04-nlp/03-scaling-human-centered-llms).

-   **Michael J. Ryan** wrote [Pluralism](../04-nlp/05-pluralism) and co-wrote the remainder of [NLP for HCLLMs](../04-nlp/).

-   **Aadesh Salecha** co-wrote [Bias and Fairness Evaluation](../05-evaluation/02-human-level-evaluations).

-   **Xiaoxian Shen** co-wrote [Consent and Ownership](../03-data/03-consent-and-ownership).

-   **Pranava Singhal** helped with the course paper.

-   **Shashanka Subrahmanya** co-wrote [Societal-level Evaluation](../05-evaluation/03-societal-level-evaluation)

-   **Mei Tan** co-wrote [Benchmarks](../05-evaluation/01-model-level-evaluations).

-   **Irawadee Thawornbut** helped with the course paper.

-   **Michelle Vinocour** helped with the course paper.

-   **Xiaoyue Wang** co-wrote [Expanding Data Sources: Synthetic and Non-Traditional Data](../03-data/04-expanding-data-sources-synthetic-and-non-traditional-data)

-   **Zheng Wang** co-wrote [Interpretable and Explainable HCLLMs](../06-responsible/01-interpretable-and-explainable-hcllms).

-   **Henry Jin Weng** helped with the course paper.

-   **Pawan Wirawarn** helped with the course paper.

-   **Shirley Wu** helped with the course paper.

-   **Sophie Wu** co-wrote [Learning from Human Preferences](../04-nlp/02-learning-from-human-preferences).

-   **Yichen Xie** co-wrote [Learning from Human Preferences](../04-nlp/02-learning-from-human-preferences).

-   **Patrick Ye** helped with the course paper and second-round student edits.

-   **Sunny Yu** co-wrote [Quantitative Evaluation](../05-evaluation/01-model-level-evaluations) and [Responsible Human-Centered LLMs](../06-responsible/).

-   **Sean Zhang** helped with the course paper and second-round student edits.

-   **Yutong Zhang** co-designed the figure in [Introduction](../01-introduction/), the figure in [HCI for HCLLMs](../02-hci/), the figure in [Evaluation](../05-evaluation/), the figure in [Responsible Human-Centered LLMs](../06-responsible/).

-   **Cathy Zhou** co-wrote [Supervised Fine-tuning for HCLLMs](../04-nlp/01-supervised-fine-tuning-for-hcllms).

-   **Yiling Zhao** co-wrote [Multilinguality](../04-nlp/06-multilinguality).
