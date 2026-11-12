# Introduction Story Arc

An agent skill for designing, drafting, and revising research-paper Introductions as a clear argument from problem to contribution. It is especially suited to ML/AI and related technical research.

The skill organizes an Introduction into five moves: world and stakes, existing approaches and their shared limitation, the proposed idea, its mechanisms, and the contribution payoff. It keeps claims tied to available evidence and treats the story analogy as a planning aid, not manuscript prose.

## Install for Codex

Clone this repository into your Codex skills directory:

```sh
git clone https://github.com/ARCHIC001/introduction-story-arc.git ~/.codex/skills/introduction-story-arc
```

Restart Codex if needed, then invoke `$introduction-story-arc` in a request. For example:

> Use $introduction-story-arc to diagnose the argument in my Introduction and suggest a revised outline.

Provide the paper's abstract, method, results, references, target venue, and existing Introduction where available. The skill does not replace literature review or verification of empirical claims.

## Contents

- [SKILL.md](SKILL.md) — instructions and evidence guardrails.
- [Worksheet](references/introduction-arc-worksheet.md) — a structured argument and evidence map.
- [Codex interface configuration](agents/openai.yaml).

## License

[MIT](LICENSE).
