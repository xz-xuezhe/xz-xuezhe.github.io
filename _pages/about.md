---
permalink: /
title: "About Me"
description: "Zhe Xue is a computer science undergraduate at SUSTech working on reliable LLM reasoning, uncertainty-aware inference, and on-policy distillation."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am an undergraduate in Computer Science and Technology (Turing Class) at **Southern University of Science and Technology (SUSTech)**, expecting to graduate in June 2027 with a B.Eng.

My research focuses on **reliable reasoning in large language models**, including uncertainty-aware inference and on-policy distillation. I also enjoy building systems, from compilers to processors, and competing in programming contests.

## Research

### Hybrid Sampling for Reliable On-Policy Distillation

<p class="entry-date">May – July 2026</p>

Developed a likelihood-ratio-guided sampling rule that selectively replaces student-proposed tokens with teacher samples, together with a source-aware objective using reverse KL for student tokens and forward KL for teacher corrections. The method requires no auxiliary reward or verifier models.

Distilling Qwen3-4B into Qwen3-1.7B improved macro **Avg@8 by 3.25 percentage points** and **Pass@8 by 4.94 percentage points** over on-policy distillation (OPD) on AIME 2024/2025 and AMC 2023. The vLLM-based hybrid rollout pipeline incurred **8.6% runtime overhead** under a matched training-data budget.

### Uncertainty-Aware Inference for LLM Reasoning

<p class="entry-date">September 2025 – Present</p>

Studying how sampling temperature affects reasoning across four Qwen3 models and five MATH difficulty levels. Experiments tracked answer accuracy, reasoning validity and redundancy, and verification scores, and compared majority voting with confidence-weighted aggregation.

Observed model- and difficulty-dependent temperature thresholds beyond which reasoning degrades sharply; harder problems degraded at lower temperatures. I am investigating model-internal uncertainty signals to guide adaptive inference.

## Selected Projects

### [SysY Compiler](https://github.com/xz-xuezhe/sysy-compiler)

<p class="entry-date">July 2025 · Rust · Compilers</p>

A compiler for a C-like language, lowering ASTs through Koopa IR to RV32IM assembly. Supports scoped symbols, short-circuit control flow, functions, and multidimensional arrays, with seven IR rewrite rules and a 13-register write-back cache. Passed 130 functional tests in both Koopa IR and RISC-V modes, including 20 benchmark programs.

### [RISC-V CPU](https://github.com/xz-xuezhe/RV32-CPU)

<p class="entry-date">April – May 2025 · Verilog · Computer Architecture</p>

A five-stage pipelined RV32I CPU supporting 38 instructions, with forwarding, load-use stalls, static branch prediction, and pipeline flushing. Includes UART memory loading and a three-stage Python deployment toolchain. Validated with eight Vivado simulation tests and three on-board assembly tests.

## Education

**Southern University of Science and Technology, China**<br>
September 2023 – June 2027 (expected)

- B.Eng. candidate in Computer Science and Technology (Turing Class)
- **GPA: 3.92/4.00 · Rank: 4/157**
- Peer Tutor, Linear Algebra (Spring & Fall 2024): delivered exam review sessions for fellow students.

## Selected Awards

- **Gold Medal**, 2024 ICPC Asia Chengdu Regional Contest
- **Gold Medal**, 2024 ICPC Asia Hong Kong Regional Contest
- **Silver Medal**, 2024 ICPC Asia East Continent Final Contest
