# SRL-MPC

**Shape-Aware Reinforcement Learned Model Predictive Control**

[Project Website](https://hanruihua.github.io/srl_mpc_project/) ·
[Paper](https://arxiv.org/abs/2608.21175) ·
[Demonstrations](https://hanruihua.github.io/srl_mpc_project/#demonstrations)

[Ruihua Han](https://hanruihua.github.io/)<sup>1</sup>,
[Rui Gao](https://github.com/hfr2015)<sup>2</sup>,
[Zhe Liu](https://happinesslz.github.io/)<sup>1</sup>,
[Xinyi Wang](https://lawliet9666.github.io/)<sup>3</sup>,
[Chang Chen](https://scholar.google.com/citations?hl=en&user=1jx4TqkAAAAJ)<sup>1</sup>,
[Shuai Wang](https://siat-invs.com/)<sup>4</sup>,
[Qi Hao](https://cse.sustech.edu.cn/faculty/~haoq/)<sup>2</sup>,
[Jia Pan](https://ai.hku.hk/people/academic-staff/jpan)<sup>1</sup>, and
[Hengshuang Zhao](https://hszhao.github.io/)<sup>1</sup>

<sup>1</sup>The University of Hong Kong ·
<sup>2</sup>Southern University of Science and Technology ·
<sup>3</sup>University of Michigan ·
<sup>4</sup>Shenzhen Institutes of Advanced Technology

> **TL;DR:** SRL-MPC combines shape-aware high-order control barrier functions
> (HOCBFs) with reinforcement learning for online MPC parameter adaptation,
> enabling safe and efficient navigation of heterogeneous robot shapes in dense
> crowds without geometry simplification or policy retraining.

## Overview

SRL-MPC is a distributed navigation framework for heterogeneous robot crowds.
It derives compact geometric separation features (GSFs) from circular and
convex-polygon footprints, then uses a learned policy to adapt interpretable
planning parameters from the local crowd geometry. This combines the
adaptability of reinforcement learning with explicit, model-based MPC control.

## Demos

The GIF previews play directly in the README; click one to open the full MP4.
The simulation clips are held-out randomized episodes shown at 2× speed. The
full collection is available in the
[demo gallery](https://hanruihua.github.io/srl_mpc_project/#demonstrations).

| Dense crowd: 25 robots | OOD: nonconvex unions | Real-world comparison |
|:---:|:---:|:---:|
| [<img src="assets/demos/random-polygon-n25.gif" alt="SRL-MPC navigating a dense crowd of 25 randomly shaped robots" width="300">](https://hanruihua.github.io/srl_mpc_project/assets/demo/density/random-polygon-n25.mp4) | [<img src="assets/demos/nonconvex-union.gif" alt="SRL-MPC navigating an out-of-distribution nonconvex-union scenario" width="300">](https://hanruihua.github.io/srl_mpc_project/assets/demo/ood/nonconvex-union.mp4) | [<img src="assets/demos/platform-comparison.gif" alt="Real-world comparison of navigation methods" width="300">](https://hanruihua.github.io/srl_mpc_project/assets/demo/real-world/platform-comparison.mp4) |

## Architecture

<p align="center">
  <img src="https://hanruihua.github.io/srl_mpc_project/assets/architecture.png"
       alt="SRL-MPC architecture from crowd geometry through learned MPC parameter adaptation to robot control"
       width="100%">
</p>

## Code

The source code will be released upon acceptance of the paper. 
