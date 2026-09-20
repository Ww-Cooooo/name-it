**English** | [简体中文](README.zh-CN.md)

# Name It

> Turn a complex idea into a short, clear, memorable name.

Name It is an open Codex Skill for naming and renaming projects, products, tools, Agents, Skills, features, workflows, repositories, and packages.

It helps when a name is too long, too vague, difficult to remember, misleading, or disconnected from what the thing actually does. Instead of producing a wall of random suggestions, Name It understands the real job, recommends one strong direction, explains a few distinct alternatives, and improves them using your reactions.

## What it does

- Finds the central idea the name should communicate.
- Favors familiar words that reveal the benefit; concise English tool names usually start with two words, unless your brief calls for another style.
- Balances clarity, brevity, accuracy, memorability, and distinctiveness.
- Gives one recommendation before a small set of meaningful alternatives.
- Evaluates names you already have without needlessly replacing them.
- Preserves feedback such as “too long” or “too vague” in the next round.
- Handles bilingual naming considerations when the audience needs them.
- Separates creative judgment from live collision or trademark checks.

Name It does not generate dozens of near-identical options, force obscure acronyms, or turn a naming question into a heavyweight branding process.

## Language

The canonical [SKILL.md](SKILL.md) is written in English so one instruction source remains authoritative across supported Codex use. English and Simplified Chinese READMEs explain the same behavior to users.

The Skill responds in the language of the conversation unless the naming task calls for another language.

Name It currently targets Codex. Other Agent Skill-compatible hosts may be able to read the same structure, but cross-host compatibility is not claimed until verified.

## When to use it

Use Name It when you want to:

- name a new project, product, app, tool, Agent, Skill, or feature;
- shorten a working title without losing its meaning;
- make a name easier to understand or remember;
- choose between existing candidates;
- rename something whose current identity no longer fits;
- settle capitalization, spacing, or a repository/package slug.

Routine code identifiers and simple translation do not need this Skill unless they involve a real naming decision.

## Example

```text
Use $name-it to name this public Codex Skill. It helps Codex think through the full problem but avoids turning small projects into enterprise systems. I want a short English name that people can roughly understand at a glance. Recommend one name first, then give only a few strong alternatives.
```

The response should lead with the best fit, explain why it works, show only genuinely different alternatives, and state whether any live collision check remains to be done.

## Install

If you want Codex to perform the installation after this repository is public, send it this request:

```text
Inspect and install this Codex Skill: https://github.com/Ww-Cooooo/name-it
Only inspect and copy this repository into my personal Skill directory. Do not install dependencies, modify projects, or overwrite, delete, or update an existing Skill. If the target already exists, stop and report its path and source.
After installation, report the actual path and what was copied. I will open a new task separately to verify discovery.
```

You can also clone it manually. Git must already be installed, and the target `name-it` directory must not already exist.

### Windows PowerShell 7

```powershell
$skillRoot = Join-Path $env:USERPROFILE ".agents\skills"
New-Item -ItemType Directory -Force -Path $skillRoot | Out-Null
git clone https://github.com/Ww-Cooooo/name-it.git (Join-Path $skillRoot "name-it")
```

### macOS or Linux

```bash
mkdir -p "$HOME/.agents/skills"
git clone https://github.com/Ww-Cooooo/name-it.git "$HOME/.agents/skills/name-it"
```

After installation, open a new Codex task and ask it to confirm that `name-it` appears in the available Skill list and report the resolved `SKILL.md` path. Use `$name-it` explicitly when you want to guarantee invocation for a particular naming task.

## Boundaries

- Name It does not expand Codex permissions.
- It does not access the network unless a live check is requested and authorized.
- A web search can find obvious collisions, but it is not legal trademark clearance.
- It does not promise domain, package, account, or repository availability without checking the relevant service.
- It does not replace a full brand strategy, identity system, or legal review unless the user separately requests that work.
- This repository contains instructions, display metadata, and prompt-based evaluation fixtures. It contains no executable scripts or dependencies.

## Repository contents

| Path | Purpose |
| --- | --- |
| `SKILL.md` | Canonical Skill instructions loaded after discovery |
| `agents/openai.yaml` | Display metadata and default invocation prompt |
| `evals/evals.json` | Representative naming prompts and expected behavior |
| `README.md` | English project entrypoint |
| `README.zh-CN.md` | Simplified Chinese project entrypoint |

## License

[MIT License](LICENSE)
