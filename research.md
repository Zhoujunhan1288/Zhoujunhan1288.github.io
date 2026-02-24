---
layout: default
title: Research
permalink: /research/
---

<div class="hero">
  <h1>Research</h1>
  <p>
    Public-facing research overview, milestones, working papers, and reproducibility notes.
    This page tracks the long-term research program rather than daily progress.
  </p>
</div>

<div class="section"></div>

## Research Program

<div class="research-card">

### Phase 1 · ConDiff (2026)

**Core Idea**  
Continuation / curriculum mechanisms for stabilizing exploration in thin-channel or underactuated environments.

**Key Questions**
- How does β scheduling reshape the exploration manifold?
- Can staged continuation reduce failure modes in sparse/delayed reward regimes?
- What is the structural difference between fixed-β and staged-β training?

**Experimental Platforms**
- MassPoint (underactuated x-axis setting)
- Swimmer / Ant (progressive scaling)

</div>

<div class="section"></div>

## Working Papers / In Progress

<div class="research-card">

### ConDiff: β-Annealing for Thin-Channel Exploration  
*Status: In preparation*

- Experimental framework constructed
- Baseline fixed-β replication underway
- Stage-switch logic validation in progress
- Failure mode categorization under refinement

**Next Steps**
- Align fixed-β baseline results
- Validate stage switching (episode/frame vs max steps)
- Produce core ablation plots
- Draft Introduction + Method section

</div>

<div class="section"></div>

## Milestones

<div class="milestone-list">

- ☐ Baseline: Stable reproduction of fixed-β MaxDiff  
- ☐ Curriculum: Stage-switch without training conflict  
- ☐ Figure Pack: Reward curves · Stage trace · Success rate  
- ☐ Draft v1: Introduction + Method + Experiments skeleton  

</div>

<div class="section"></div>

## Code & Reproducibility

<div class="research-card">

- GitHub Repository: (coming soon)
- Reproducibility Notes: seeds, configs, and command-line records linked in Research Log
- Experimental traceability maintained through staged logging

</div>
