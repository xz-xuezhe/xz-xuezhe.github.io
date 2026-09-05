---
layout: single
title: "Curriculum Vitae"
description: "Education, research experience, projects, awards, and skills of Zhe Xue, a computer science undergraduate at SUSTech."
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
  - /resume-json
  - /cv-json/
---

[Download CV (PDF)]({{ '/files/cv.pdf' | relative_url }}){: .btn .btn--primary}

Updated September 2026.

## Education

**Southern University of Science and Technology, China**<br>
September 2023 – June 2027 (expected)<br>
B.Eng. candidate in Computer Science and Technology (Turing Class)

- GPA: **3.92/4.00**; Rank: **4/157**
- Peer Tutor, Linear Algebra (Spring & Fall 2024): delivered exam review sessions for fellow students.

## Awards

- **Gold Medal**, 2024 ICPC Asia Chengdu Regional Contest — October 2024
- **Gold Medal**, 2024 ICPC Asia Hong Kong Regional Contest — December 2024
- **Silver Medal**, 2024 ICPC Asia East Continent Final Contest — December 2024

## Research Experience

### Hybrid Sampling for Reliable On-Policy Distillation

<p class="entry-date">May – July 2026</p>

- Developed a likelihood-ratio-guided hybrid sampling rule to selectively replace student-proposed tokens with teacher samples before prefix deviations degrade subsequent teacher supervision.
- Formulated a source-aware dual-divergence objective using reverse KL for retained student tokens and forward KL for teacher corrections, without auxiliary reward or verifier models.
- Built a hybrid rollout pipeline on DAPO-Math-17K by adapting vLLM's speculative-decoding engine; end-to-end training incurred 8.6% runtime overhead over OPD under a matched training-data budget.
- Distilled Qwen3-4B into Qwen3-1.7B, improving macro Avg@8 by 3.25 percentage points and macro Pass@8 by 4.94 percentage points over OPD on AIME 2024/2025 and AMC 2023.

### Uncertainty-Aware Inference for LLM Reasoning

<p class="entry-date">September 2025 – Present</p>

- Characterized temperature-dependent reasoning across four Qwen3 models and five MATH difficulty levels, tracking answer accuracy, ReasonEval validity/redundancy, and Math-Shepherd verification scores.
- Observed sharp degradation beyond model- and difficulty-dependent temperature thresholds; harder problems degraded at lower temperatures.
- Benchmarked majority voting and confidence-weighted aggregation under temperature sweeps, finding that multi-sample gains peaked before high-temperature degradation.
- Investigating model-internal signals of uncertainty to guide adaptive inference for LLM reasoning.

## Projects

### [SysY Compiler](https://github.com/xz-xuezhe/sysy-compiler)

<p class="entry-date">July 2025</p>

- Built a compiler written in Rust for a C-like language, lowering ASTs through Koopa IR to RV32IM assembly.
- Implemented scoped symbol tables, short-circuit control flow, functions, and multidimensional arrays.
- Optimized IR with seven rewrite rules and code generation with a 13-register write-back cache.
- Passed 130 functional tests in both Koopa IR and RISC-V modes, including 20 benchmark programs.

### [RISC-V CPU](https://github.com/xz-xuezhe/RV32-CPU)

<p class="entry-date">April – May 2025</p>

- Designed a five-stage pipelined RV32I CPU in Verilog supporting 38 instructions.
- Handled data/control hazards with forwarding, load-use stalls, static branch prediction, and pipeline flushing.
- Implemented UART loading of instruction/data memory and a three-stage Python deployment toolchain.
- Passed eight Vivado simulation tests and three on-board assembly tests covering core modules, MMIO, and AUIPC.

## Skills

- **Programming:** C++, Python, Rust, Java, Haskell, CUDA
- **Tools:** PyTorch, vLLM, Docker, Git, Bash, LaTeX
- **Languages:** Mandarin (native); English (TOEFL iBT: 5.0/6.0, comparable to 100/120)

## Contact

[{{ site.author.email }}](mailto:{{ site.author.email }}) · [GitHub](https://github.com/xz-xuezhe) · [LinkedIn](https://www.linkedin.com/in/xuez04/)
