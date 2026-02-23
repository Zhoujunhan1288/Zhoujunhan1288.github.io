---
layout: default
title: 研究成果
permalink: /research/
---

# 研究成果

这里放“对外可读”的内容：项目概览、里程碑、论文/预印本、代码与复现实验入口。  
（你现在还没发表也完全没关系：先从 **Working / In progress** 写起。）

---

## Research Program

### Phase 1 · ConDiff（2026）
- **Goal**：用 continuation/curriculum 思想让探索在“thin-channel / 欠控制”环境中更稳定、更可解释  
- **Core knobs**：β schedule、stage switching、reward shaping robustness、failure mode taxonomy  
- **Envs**：MassPoint（欠控制 x 轴）、Swimmer / Ant（逐步扩展）

---

## Working / In Progress

- **ConDiff: β-annealing for thin-channel exploration**（in preparation）  
  - Status：实验与叙事框架搭建中  
  - Next：baseline 固定 β 完整对齐；stage 切换逻辑验证；做关键消融

---

## Milestones（里程碑）

- [ ] Baseline：固定 β 的 MaxDiff 跑通并稳定复现  
- [ ] Curriculum：分阶段 β 切换无冲突（episode/frame 与 max steps 对齐）  
- [ ] Figure pack：核心图表模板（reward curve / stage trace / success rate）  
- [ ] Draft v1：Introduction + Method + Experiments 骨架

---

## Code / Repro

- GitHub Repo：稍后放链接  
- Repro Notes：建议把关键命令行、seed、配置写在日志里（可追溯）
