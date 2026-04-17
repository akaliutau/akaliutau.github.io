---
layout: page
title: "DynaVisR: Benchmark for Visual Reasoning in Dynamic Environments"
description: "A benchmark to reduce shortcutting by requiring models to solve a coupled reasoning problem in complex dynamic environment."
img: /assets/img/logo_dinavisr.jpg
importance: 1
category: work
---

[GitHub repository](https://github.com/akaliutau/dynavisr-bench)

The trajectory of AI research has arrived at a critical methodological impasse where traditional evaluation paradigms possess diminishing utility for gauging true cognitive capabilities. Current large language models routinely saturate static, knowledge-based examinations, achieving human-expert or superhuman scores on prominent benchmarks such as the Massive Multitask Language Understanding (MMLU) and HumanEval datasets. However, despite this apparent mastery of crystallized knowledge, these same frontier models experience catastrophic failures when subjected to novel, dynamic problem-solving environments that require fluid intelligence, continuous adaptation, and rigorous cognitive control. This growing divergence between benchmark success and actual reasoning capability has birthed a false sense of proximity to Artificial General Intelligence (AGI), masking severe architectural deficits in dynamic adaptability and true comprehension.

Recent empirical studies explicitly demonstrate that modern models often rely on surface-level pattern matching and statistical approximations rather than genuine logical inference. The ["Illusion of Thinking"](https://machinelearning.apple.com/research/illusion-of-thinking) by Apple researchers revealed that advanced Large Reasoning Models (LRMs) suffer from severe accuracy collapse as compositional complexity scales, including those that are explicitly engineered to generate extensive intermediate deliberation traces prior to answering. In heavy computational tasks, such as the Tower of Hanoi puzzle, models exhibit a counter-intuitive scaling limit. As problem difficulty increases, these models initially increase their deliberative effort, but upon reaching a critical complexity threshold, they counterintuitively reduce their reasoning effort and abandon the problem entirely. 

To accurately measure progress toward AGI and overcome the "jaggedness" of current model capabilities, novel benchmarks must force models into interactive, dynamically generated environments where memorization is impossible. In our benchmark we use exactly such approach. 

DynaVisR is a 100% synthetic benchmark and dataset.
Each sample is a synthetic billiard world with a ball, a rectangular table, and named rectangular obstacles (`A–D`). 
The solver must mentally simulate the ball’s reflections while also applying visibility rules that change after specific bounce counts. 
At a queried moment, the solver must identify the next hit object, determine which obstacles are visible, 
and recover the bottom-to-top order of the visible overlapping subset.

The benchmark is designed to catch the nuances of visual reasoning in clean, yet complex and dynamic controlled environment.

See the whole story [here](https://www.kaggle.com/competitions/kaggle-measuring-agi/writeups/dynamic-visual-reasoning)
