# Install

## Claude Code

With the plugin:

```bash
claude plugin marketplace add JuliusBrussee/caveman && claude plugin install caveman@caveman
```

Then verify the active mode:

```bash
cat "${CLAUDE_CONFIG_DIR:-$HOME/.claude}/.caveman-active"
```

## Generic skills CLI

Global user-skill install:

```bash
npx skills add JuliusBrussee/caveman -g
```

Project-local install:

```bash
npx skills add JuliusBrussee/caveman
```

To remove:

```bash
claude plugin uninstall caveman@caveman
npx skills remove caveman
```

## Profiles / versions

- `SKILL.md` — default concise profile
- `SKILL-LITE.md` — lightweight terse version
- `SKILL-ULTRA.md` — aggressive ultra-short version for Claude Code
- `SKILL-WENYAN.md` — compact poetic variant

Use the profile file that matches your preferred response density.

## Supported agents

This repo is designed around the Claude Code skill pattern and compatible tooling that reads `SKILL.md` from the installed skill directory.

For a specific host, use the agent's matching skill profile if supported by the host's installation method.
