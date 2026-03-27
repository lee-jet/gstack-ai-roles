---
name: gstack-ai-roles
description: Elite 6-phase engineering production engine. Orchestrates specialized subagents (Think, Plan, Build, Review, Test, Ship) to deliver production-grade software with Garry Tan's "Boil the Lake" philosophy. Triggers on requests for feature engineering, project initialization, or full-lifecycle management. Uses structured gates for CEO/Staff/QA-level auditing.
version: 1.2.0
---

# 🌌 gstack Specialist: Elite Engineering Engine

This engine implements the **"AI Software Factory"** paradigm. It transforms high-level vision into robust, shippable code through a rigorous sequence of specialized subagent handoffs and "Boil the Lake" engineering standards.

## 🏗️ Operational Units (Phases)

| Phase | Specialization | Central Artifact | gstack Alignment |
| :--- | :--- | :--- | :--- |
| **1. Think** | Strategic Product Alignment | `DESIGN.md` | CEO / Office Hours |
| **2. Plan** | Architectural Blueprint | `PLAN.md` | Eng Manager / Design Audit |
| **3. Build** | Precision Implementation | `Codebase` | Implementer / Designer |
| **4. Review** | Adversarial Audit (CSO) | `Review Report` | Staff Architect / Security |
| **5. Test** | Functional Stress (QA) | `Test Pass` | QA Lead / Browser Ninja |
| **6. Ship** | Release Governance (Retro) | `Deployment` | Ship-Captain / Docs-Eng |

## 🚀 Execution Modes

- **Full Sprint**: "Engineer [feature]" — Runs the complete lifecycle.
- **Partial Sprint**: "Skip Think, start from Plan" — Resumes from artifacts.
- **Single Unit**: `/think`, `/plan`, `/review`, `/ship`.

## 💎 Engineering Guardrails
- **Contract-First**: Zero implementation until the topology and state-machines in `PLAN.md` are locked.
- **Adversarial Audit**: Every change must survive a "Codex-style" multi-model adversarial challenge.
- **Boil the Lake**: Pursue 100% robustness. Handle every edge case. Machines don't tire; don't settle for "good enough."

Refer to `references/prompts.md` for the internal operational instructions (Standard Operating Procedures).
