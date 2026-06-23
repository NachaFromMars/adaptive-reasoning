# adaptive-reasoning — Right-sized thinking for every task

> Automatically gauges how hard a request really is, then dials reasoning effort up or down to match. No more burning deep-thinking cycles on trivial asks — or under-thinking the hard ones.

[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://github.com/NachaFromMars)

## Overview
adaptive-reasoning is a lightweight meta-skill that scores incoming tasks for complexity and selects an appropriate reasoning level before the agent responds. It evaluates each request across several dimensions and produces a single 0–10 score, which maps to a response strategy ranging from fast answers to extended thinking. This keeps simple work snappy while ensuring complex, high-stakes, or novel problems get the deliberation they deserve. It runs in the background on any sufficiently complex user message.

## Features

| Dimension | Score |
|---|---|
| Multi-step logic | +3 |
| Ambiguity | +2 |
| Code architecture | +2 |
| Math | +2 |
| Novel problem | +1 |
| High stakes | +1 |

**Thresholds:**
- **≤ 2** → fast response
- **3–5** → standard response
- **6–7** → consider reasoning (🧠 indicator)
- **≥ 8** → activate extended thinking (🧠🔥 indicator)

## Usage / Quick Start
The skill activates automatically. When a message arrives, it computes the complexity score, picks the matching mode, and surfaces a visual indicator (🧠 at 6–7, 🧠🔥 at ≥ 8). No commands or configuration required.

## Trigger Keywords (OpenClaw)
any complex user message

## Related Skills
- [brainstorm](https://github.com/NachaFromMars/brainstorm) — fast idea generation that pairs well with calibrated reasoning

---
Part of the [NachaFromMars](https://github.com/NachaFromMars) OpenClaw skill ecosystem.
