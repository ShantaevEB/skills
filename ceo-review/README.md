# CEO Review

A skill for critically reviewing ideas, results, and reports from the perspective of an experienced, pragmatic, and demanding CEO. It helps identify weak points and prepare material for leadership, board, or investor discussions.

[Russian documentation](../README.ru.md#ceo-review)

## What it reviews

- **Business value and ROI:** impact on profit, costs, or market share; whether the result justifies the resources invested.
- **Strategic focus:** alignment with the company's long-term goals and priorities.
- **Risks and bottlenecks:** legal, reputational, technical, and operational threats.
- **Scalability:** economics, quality, and manageability as the solution expands.
- **Clarity and presentation:** whether the problem, result, and proposed decision can be understood in two minutes.

The skill separates facts from assumptions, does not invent missing metrics, and directs criticism at the material. When evidence is incomplete, it provides a provisional assessment and identifies what needs to be substantiated.

## Response format

1. **CEO Verdict:** Approved, Needs revision, or Rejected, with the main reason.
2. **Blunt Critique:** the most important weaknesses and blind spots.
3. **Questions from Leadership:** 3–4 questions to address before presenting the material further.
4. **Action Steps:** specific improvements in priority order.

Reviews use the user's language unless another language is requested.

## Installation

Send this request in Codex:

```text
$skill-installer install ceo-review from https://github.com/ShantaevEB/skills/tree/main/ceo-review
```

Or run the local installer:

```sh
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo ShantaevEB/skills --ref main --path ceo-review
```

## Usage example

```text
$ceo-review
Critically review my proposal to automate request processing.
Below are the goal, current costs, implementation budget, expected impact, and pilot plan:
[paste your material]
```

For a substantive review, include company goals, baseline metrics, costs, timelines, and success criteria. Early ideas are also welcome: missing information will be addressed in the questions from leadership.

When invoked without material, the skill replies: "CEO mode activated." The activation message is translated to the user's language when appropriate.

## Files

- [`SKILL.md`](SKILL.md) — skill instructions.
- [`agents/openai.yaml`](agents/openai.yaml) — metadata for the Codex UI.

The skill does not require external services or additional dependencies.
