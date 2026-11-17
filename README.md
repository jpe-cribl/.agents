# .agents

Agent skills for the jpe-cribl organization's repositories, in the
[Agent Skills](https://agentskills.io) layout.

## Layout

- `skills/<name>/SKILL.md`: one directory per skill.
- `skills.sh.json`: skill groupings.
- `.claude-plugin/marketplace.json`: the Claude Code marketplace for these
  skills.

## Installation

- Claude Code: `claude plugin marketplace add jpe-cribl/.agents`, then install a
  plugin from it.
- Other harnesses: copy or link `skills/<name>` into the harness's skill
  directory, such as `~/.agents/skills`.

## Usage

Each skill states in its `description` when an agent should use it. Call one
directly by name, such as `/<plugin>:<skill>` in Claude Code.

## Contributing

A skill lives in the organization whose repositories it acts on. Write and
check skills with the agentops `skill-builder` and `skill-eval` skills.
Changes arrive by pull request.

## License

Apache-2.0. See [LICENSE](LICENSE).

---

> Part of a [larger ecosystem of repos](https://docs.jacobpevans.com).
