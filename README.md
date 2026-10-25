# Solution Research

[中文说明](README.zh-CN.md)

An agent skill for open-ended research and solution selection. It separates objectives from assumptions, searches across domains, and compares candidates against the user's actual constraints.

The English [SKILL.md](SKILL.md) is the installable skill. The [Chinese README](README.zh-CN.md#完整中文翻译) includes its complete Chinese translation.

## Install

Copy `SKILL.md` into your agent's `skills/solution-research/` directory.

For Codex, use `~/.codex/skills/solution-research/SKILL.md`. If you installed an earlier version as `research-solutions`, replace that installation with `solution-research` to avoid duplicate skills.

## Use

Invoke `$solution-research` with your question and any known constraints. Agents that support automatic skill discovery can also select it for relevant requests.

## Workflow

1. Analyze the problem and confirm boundaries.
2. Abstract the need and research across domains.
3. Apply the constraints and narrow the options.
4. Deliver a decision recommendation.

The skill applies to implementation ideas, technical and architecture comparisons, alternatives, and potentially better approaches to an initial proposal. It excludes simple factual questions, error fixes, and routine execution with settled requirements and a settled approach.

## Acknowledgments

The writing approach was inspired by Matt Pocock's [skills](https://github.com/mattpocock/skills), including Retro and writing-for-agents. This is an independent project.

## License

[MIT](LICENSE).
