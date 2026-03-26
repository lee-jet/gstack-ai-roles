# gstack Specialist Prompt Template Architecture Analysis

This report provides a deep dive into the 13 extracted gstack specialist role prompts, revealing the engineering philosophy, common patterns, and differentiated designs for various roles.

---

## 1. Core Commonalities

Despite different responsibilities, all templates follow a unified "Meta-Architecture":

### A. Mission-Driven Start
Every file begins with `# Role: [Role Name]`, immediately followed by a **Mission** statement. This sets the primary identity and goal priority (e.g., CEO prioritizes product value, EM prioritizes technical rigor).

### B. "Boil the Lake" Philosophy
Most templates explicitly or implicitly include a requirement to "ensure response completeness." This is the core spirit of gstack: leave no stone unturned, perform a ground-up search, and dive deep into every issue.

### C. Phased Execution
All core roles avoid single-prompt execution, instead following a **Phase 1 -> Phase 2 -> Phase 3** linear or cyclic workflow.
- **Phase 1: Orientation/Audit**
- **Phase 2: Execution/Analysis**
- **Phase 3: Verification/Summary**

### D. Hard Constraint Enforcement (Important Rules)
At the end of every template is an `Important Rules` section for setting technical red lines (e.g., strictly no Force Push, zero tolerance for Secrets) and behavioral standards (e.g., anti-sycophancy).

---

## 2. Differentiated Design

Differentiation is reflected in **Cognitive Modes**, **Tool Focus**, and **Output Styles**:

### A. Cognitive Mode Comparison
| Role Type | Core Focus | Typical Mindset |
| :--- | :--- | :--- |
| **Strategic (CEO/PM)** | Product Value, Scope, UX | "10-Star Experience", "Nuclear Scope Challenge" |
| **Management (EM/Arch)** | Arch Consistency, Tech Debt, Coverage | "Analyze before Fix", "Modular/Atomic" |
| **Audit (CSO/QA/Review)** | Risk, Bugs, Security, Edge Cases | "Finding Cracks", "Regression Test Driven" |
| **Creative (Designer)** | Visual Soul, Cohesion, Creative Risk | "Aesthetic Calibration", "Pixel-Perfect Alignment" |

### B. Specialized Tool Configuration
- **Visual Roles** (QA/Designer): Heavy use of `Chromium/Browse` for real-time rendering comparison.
- **Logic Roles** (EM/Reviewer/CSO): Heavy reliance on `Grep`, `Git log`, and `Diff` analysis.
- **Analytical Roles** (Retro/Performance): Focus on `Git` data mining and metric calculation.

### C. Output Differentiation
- **CEO**: Produces Proposals, Vision Descriptions, and "Expand/Cut" decisions for implementation plans.
- **EM/Reviewer**: Produces Audit Reports, improvement suggestions, and specific code fixes.
- **Designer/QA**: Produces Screen Comparisons, Visual Scorecards, and UI Specs (`DESIGN.md`).

---

## 3. Architecture Summary

The architecture of gstack prompt templates is effectively a **"Protocol for Packaging Software Engineering Experience."** It achieves this through:
1. **Identity Anchoring** (Role Definition)
2. **Process Refinement** (Operational Phases)
3. **Tool Empowerment** (Specific CLI Calls)
4. **Cultural Rooting** (Philosophies like Boil the Lake)

By transforming vague "Vibe Coding" into a **highly repeatable, auditable industrial development process**.

---
