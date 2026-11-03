# Codex Skills

A collection of reusable skills for Codex. Each skill lives in its own folder with instructions, documentation, and usage examples.

[Russian documentation](README.ru.md)

## Skills

| Skill | Description |
| --- | --- |
| [CEO Review](ceo-review/README.md) | Tough, constructive reviews of ideas, results, and reports from a CEO's perspective: business value, strategy, risks, scalability, and clarity. |

## Install a skill

Ask Codex to install the skill using `$skill-installer`. For example:

```text
$skill-installer install ceo-review from https://github.com/ShantaevEB/skills/tree/main/ceo-review
```

Or use the installer from your local Codex installation, specifying the skill folder:

```sh
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo ShantaevEB/skills --ref main --path ceo-review
```

The installer does not overwrite an existing skill with the same name.

## Repository structure

```text
README.md             Skill catalog and installation guide
README.ru.md          Russian documentation
ceo-review/
  README.md           Description, installation, and examples
  SKILL.md            Instructions for Codex
  agents/openai.yaml  Display name and description in the Codex UI
```

## Add a skill

Create a separate folder with a short name in `lowercase-with-hyphens` format. The required file is `SKILL.md`, with `name` and `description` in its YAML frontmatter and instructions for Codex in the body.

Add a README covering the skill's purpose, installation, and an example invocation, then add it to the table above. Include `agents/` metadata, scripts, references, and assets only as needed.
