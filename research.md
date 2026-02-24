---
layout: default
title: Research
permalink: /research/
---

<div class="hero">
  <h1>Research</h1>
  <p>
    Public-facing overview of long-term research directions, milestones,
    working papers, and reproducibility structure.
  </p>
</div>

<div class="section"></div>

<h2>Research Program</h2>

<div class="research-card">

  <h3>Phase 1 · ConDiff (2026)</h3>

  <p>
    <strong>Core Idea</strong><br>
    Continuation / curriculum mechanisms for stabilizing exploration
    in thin-channel or underactuated environments.
  </p>

  <p><strong>Key Questions</strong></p>
  <ul>
    <li>How does β scheduling reshape the exploration manifold?</li>
    <li>Can staged continuation reduce failure modes in sparse or delayed reward regimes?</li>
    <li>What structural differences emerge between fixed-β and staged-β training?</li>
  </ul>

  <p><strong>Experimental Platforms</strong></p>
  <ul>
    <li>MassPoint (underactuated x-axis setting)</li>
    <li>Swimmer / Ant (progressive scaling)</li>
  </ul>

</div>

<div class="section"></div>

<h2>Working Papers / In Progress</h2>

<div class="research-card">

  <h3>ConDiff: β-Annealing for Thin-Channel Exploration</h3>

  <p><em>Status: In preparation</em></p>

  <ul>
    <li>Experimental framework constructed</li>
    <li>Baseline fixed-β replication underway</li>
    <li>Stage-switch logic validation in progress</li>
    <li>Failure mode categorization under refinement</li>
  </ul>

  <p><strong>Next Steps</strong></p>
  <ul>
    <li>Align fixed-β baseline results</li>
    <li>Validate stage switching (episode/frame vs max steps)</li>
    <li>Produce core ablation plots</li>
    <li>Draft Introduction + Method section</li>
  </ul>

</div>

<div class="section"></div>

<h2>Milestones</h2>

<div class="milestone-list">
  <ul>
    <li>☐ Stable reproduction of fixed-β MaxDiff</li>
    <li>☐ Stage-switch without training conflict</li>
    <li>☐ Figure Pack: reward curves · stage trace · success rate</li>
    <li>☐ Draft v1: Introduction + Method + Experiments skeleton</li>
  </ul>
</div>

<div class="section"></div>

<h2>Code & Reproducibility</h2>

<div class="research-card">

  <ul>
    <li><strong>GitHub Repository:</strong> (coming soon)</li>
    <li><strong>Reproducibility:</strong> seeds, configs, and command logs linked in Research Log</li>
    <li><strong>Traceability:</strong> staged logging and experiment tracking maintained</li>
  </ul>

</div>
