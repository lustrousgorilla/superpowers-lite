# Superpowers Lite

Superpowers Lite is a trimmed Codex plugin fork of [Superpowers](https://github.com/obra/superpowers). It keeps the development workflows that are useful for planning, TDD, debugging, verification, code review, subagent execution, and finishing development branches while removing bootstrap, feedback-receiving, skill-authoring, and non-Codex harness material.

The fork source is <https://github.com/lustrousgorilla/superpowers-lite>.

## Motivation

The principal motivation for this fork is excluding the `superpowers` bootstrap skill, named `using-superpowers` upstream, because it forces excessive usage of token-expensive skills. Superpowers Lite keeps the concrete workflow skills available for deliberate use while removing the always-on enforcement layer.

## Included Superpowers

This fork includes these Superpowers:

- `systematic-debugging`
- `test-driven-development`
- `subagent-driven-development`
- `verification-before-completion`
- `requesting-code-review`
- `writing-plans`
- `dispatching-parallel-agents`
- `brainstorming`
- `executing-plans`
- `using-git-worktrees`
- `finishing-a-development-branch`

## Removed Superpowers

This fork removes these Superpowers:

- `using-superpowers`
- `receiving-code-review`
- `writing-skills`

`requesting-code-review` is intentionally included because it appeared in the requested include list, even though it was also named in the removal sentence.

## Removed Non-Essential Repository Material

The fork also removes repository material that is not needed for this Codex-focused plugin:

- Claude, Cursor, Gemini, and OpenCode harness metadata
- Hook scripts and sync/version scripts
- Historical docs, plans, specs, release notes, and tests
- Contribution/code-of-conduct files that referenced removed workflows

## Layout

```text
.codex-plugin/plugin.json
assets/
skills/
README.md
LICENSE
```

## Install Locally

Use the repository as a local Codex plugin from:

```bash
/Users/gabriel/code/ai/plugins/superpowers-lite
```

## License

MIT License. See [LICENSE](LICENSE).
