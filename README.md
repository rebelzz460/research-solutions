# research-solutions

A goal-first research skill for coding agents. Audit constraints, inspect mature implementations, compare alternatives, seek counterexamples, and verify real workflows.

一个从真实目标出发的方案研究 skill：升维理解目标 → 必要时确认 → 探索方案 → 选择路径 → 验证结果。

## Install / 安装

Copy `SKILL.md` into your agent's `skills/research-solutions/` directory. For Codex, the default user location is `~/.codex/skills/research-solutions/SKILL.md`. Keep existing customizations before replacing an installed copy.

The skill is written in Chinese. It is self-contained; Retro is optional and used only when available and appropriate.

## Use / 使用

Invoke `$research-solutions` with a problem, desired outcome, and any non-negotiable constraints.

> $research-solutions 我想用向量数据库做文档检索。请先确认真实目标和必要约束，检查现有实现，再比较方案并验证。

It can also be selected automatically by agents that support skill discovery. Use it for open-ended solution research, route comparisons, or reassessing a failed approach. Routine execution and simple fact lookups do not need the full workflow.

## What it changes / 行为

- Distinguishes hard constraints, preferences, proposed means, and inherited assumptions.
- Asks before widening the solution space when the user's intended boundary is unclear.
- Checks the existing project and original implementation before building.
- Compares adoption, reuse, extension, composition, and custom development.
- Defines evidence that could overturn the preferred route.
- Separates theoretical support, implementation evidence, and observed execution.
- Captures lessons at meaningful milestones without treating retrospective suggestions as permission.

## Review cases / 检查场景

| Request | Expected behavior |
| --- | --- |
| “必须使用 SQLite，离线运行。” | Keep SQLite and offline operation as hard constraints. |
| “我想用向量数据库，但只需要快速查到合同条款。” | Clarify whether the database is required before dependent route selection. |
| “原项目似乎已经支持这个功能。” | Inspect the implementation, examples, and tests before rebuilding. |
| “补丁加了很多，指标仍不达标。” | Test the failing assumption and reconsider the route. |
| “论文说可行，但这里无法运行。” | Report the evidence gap; do not claim local usability. |
| “只修复已确定方案中的一个拼写错误。” | Perform the small edit directly. |

These are manual review scenarios, not a claim of measured model performance.

## Acknowledgments / 致谢

The concise steps, conditional references, and emphasis on improving the agent's environment are inspired by Matt Pocock's [skills](https://github.com/mattpocock/skills), particularly the locally available Retro and writing-for-agents workflows. This is an independent skill, not an official Matt Pocock project.

## License

MIT. See [LICENSE](LICENSE).
