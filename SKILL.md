---
name: solution-research
description: Use for open-ended problem exploration, technical research, architecture comparisons, and solution selection. Trigger when the user seeks implementation ideas, compares technical approaches, looks for alternatives, or proposes an initial idea that may have a better solution. Do not trigger for simple factual questions, error fixes, or routine execution when both the requirements and approach are fully settled.
---

# Solution Research

Help the user research and select solutions through the following four stages. Do not treat the technical approach the user initially names as the only option.

## Steps

1. **Analyze the problem and confirm boundaries**
   - Separate the **real objective**, **hard constraints** (environment, cost, and minimum compatibility requirements), and **adjustable assumptions** (implementation choices the user mentions in passing).
   - **Confirmation gate:** If missing key constraints would send the research in fundamentally different directions, do a minimal preliminary investigation, identify 2–3 concrete decision points, and ask the user to clarify. **Pause any lengthy comparison** until then. If the context is sufficient to narrow the scope, proceed directly to the next stage.

2. **Abstract the need and research across domains**
   - Remove unnecessary restrictions and restate the problem as “core needs + required capabilities.” Research the host's native capabilities, mature open-source implementations, established patterns, and alternatives from other domains in parallel.
   - **Evidence and counterexamples:** Actively research failures, limitations, and maintenance pitfalls for each direction. Use primary sources (documentation, source code, and recorded test results) to distinguish verified facts from inference. Do not judge quality by popularity or novelty.

3. **Apply the constraints and narrow the options**
   - Evaluate candidates against the user's actual constraints. Prioritize how effectively they solve the problem, then compare maturity, cost, complexity, and maintenance risk.
   - **Default selection ladder:** Strictly screen in this order: “reuse built-in capabilities or existing configuration → adopt a mature open-source implementation → combine or adapt components with lightweight changes → develop a custom solution.” Move to the next level only when the preceding one cannot meet a key requirement.

4. **Deliver a decision recommendation**
   - Present only the most valuable candidates. For each, explain its main strengths and weaknesses, suitable conditions and key limitations, recommendation rationale, and supporting evidence.
   - Give a clear first choice while preserving the user's final decision.
