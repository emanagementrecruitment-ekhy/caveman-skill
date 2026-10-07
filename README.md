# Caveman

Ultra-short coding agent instructions for Claude Code and compatible agents.

This repository packages a minimal, no-fluff instruction set that keeps code, commands, paths, and error strings exact while trimming filler prose.

## Included profiles

- `SKILL.md` — default balanced concise mode
- `SKILL-LITE.md` — lighter, still readable
- `SKILL-ULTRA.md` — aggressive ultra-short mode for Claude Code
- `SKILL-WENYAN.md` — terse poetic/compact variant

## Install

Claude Code plugin:

```bash
claude plugin marketplace add JuliusBrussee/caveman && claude plugin install caveman@caveman
```

Global skills install:

```bash
npx skills add JuliusBrussee/caveman -g
```

Project-local install:

```bash
npx skills add JuliusBrussee/caveman
```

## Verify

```bash
ls ~/.claude/skills/caveman
```

Or for the plugin mode file:

```bash
cat "${CLAUDE_CONFIG_DIR:-$HOME/.claude}/.caveman-active"
```

## Use

Start a new session and ask the agent a question. The answer is shorter, but code and exact strings stay intact.

## Notes

This package is intentionally opinionated: it removes preambles, reduces filler, and keeps technical detail high.
