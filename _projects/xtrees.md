---
layout: page
title: "Square Tree, or How To Pack 200 X-mas Trees"
description: "Distributed Geometric Packing via Crystallographic Lattices."
img: /assets/img/logo_trees.jpg
importance: 2
category: work
---

[GitHub repository](https://github.com/akaliutau/square-tree)

**SquareTree** is a scalable computational geometry engine for solving hard non-convex packing problems, inspired by the [Santa 2025 Challenge](https://www.kaggle.com/competitions/santa-2025). Its core advantage is speed: instead of spending compute on slow, chaotic exploration, it uses geometric structure to reach near-optimal configurations remarkably quickly.

We utilize a **Modified Sparrow Search Algorithm (SSA)** adapted specifically for fixed-dimension square bins. While the original Sparrow heuristic ( [Gardeyn et al.](https://arxiv.org/abs/2509.13329) ) excels at *strip packing* (minimizing infinite length) via random initialization, our engine introduces a **"Seeded Crystal"** capability. Rather than beginning with high-entropy random placement, the solver accepts a pre-loaded, geometrically derived lattice structure. This allows the optimization pipeline to bypass the chaotic "cold start" phase and immediately focus on high-density relaxation.

The result is a packing engine designed for **scalable performance** - finding excellent solutions fast, with fixed compute budget, and making difficult geometric search practical at larger problem sizes (for example, packing 1000s non-convex shapes with deep caves, similar to above).


