---
layout: page
title: "Square Tree, or How To Pack 200 X-mas Trees"
description: "Distributed Geometric Packing via Crystallographic Lattices."
img: /assets/img/logo_trees.jpg
importance: 2
category: work
---

[GitHub repository](https://github.com/akaliutau/square-tree)

**SquareTree** is a high-performance computational geometry engine designed to solve non-convex packing problems (inspired by the [Santa 2025 Challenge](https://www.kaggle.com/competitions/santa-2025)). Unlike traditional heuristic solvers that rely on random stochastic search, SquareTree leverages **crystallographic lattice theory** to identify optimal "locking" configurations.

We utilize a **Modified Sparrow Search Algorithm (SSA)** adapted specifically for fixed-dimension square bins. While the original Sparrow heuristic ( [Gardeyn et al.](https://arxiv.org/abs/2509.13329) ) excels at *strip packing* (minimizing infinite length) via random initialization, our engine introduces a **"Seeded Crystal"** capability. Rather than beginning with high-entropy random placement, the solver accepts a pre-loaded, geometrically derived lattice structure. This allows the optimization pipeline to bypass the chaotic "cold start" phase and immediately focus on high-density relaxation.
