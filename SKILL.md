---
name: introduction-story-arc
description: >-
  Design, draft, diagnose, or revise a research-paper Introduction using a
  high-tension five-move story arc: field world, shared limitation, proposed
  break, mechanism, and contribution payoff. Use for Introduction outlines,
  paragraph rewrites, research storytelling, or gap-to-method alignment in
  ML/AI and adjacent technical papers. Keep the RPG analogy as an internal
  planning aid, not as paper prose; do not use this skill for generic grammar
  polishing or acceptance prediction.
---

# Introduction Story Arc

Build an Introduction as a compact research argument, not a literature diary.
The reader should move through one causal-feeling intellectual arc:

> **A worthwhile world exists → its current rules leave a consequential gap →
> this paper introduces the capability that addresses that gap → the capability
> works through identifiable mechanisms → the paper earns a precise payoff.**

The “RPG story” analogy is an internal planning device: world-building,
conflict, protagonist, ability mechanics, and end-of-game achievements. Do not
put game metaphors into the manuscript unless the user explicitly wants a
popular-facing style.

## When this skill applies

Use it when the user asks to:

- write, restructure, or diagnose a paper Introduction;
- turn a research idea, abstract, or method description into a compelling gap-
  to-contribution narrative;
- align background, related work, method preview, and contribution bullets;
- reduce defensive, list-like, or project-log writing in an Introduction.

Do not use it as a substitute for a literature review, statistical analysis,
claim verification, or a full-paper acceptance prediction. Pair it with the
available evidence and with the user's actual target venue and page budget.

## Operating contract

1. **Start from the paper's strongest defensible value.** Identify the one
   problem the paper changes, the unit at which it changes it, and the evidence
   that can support that change. Do not invent a stronger problem merely to make
   the story dramatic.
2. **Separate evidence layers.** Mark each input as observed/implemented,
   derived from data, proposed design, or future hypothesis. A persuasive arc
   cannot convert a proposal into a result.
3. **Preserve claim scope.** “First,” “solves,” “guarantees,” “general,” and
   causal language require direct support. Replace them with narrower language
   or flag them for verification when the evidence is not present.
4. **Use representative prior work as a conversation.** Select two or more
   meaningful camps, methods, or lines of work only when they clarify the gap.
   Do not produce an exhaustive citation parade.
5. **Make every paragraph earn the next one.** End each move with the
   unresolved question that the next move answers. Remove paragraphs that do
   not change the reader's model of the problem.

For each draft, first produce a compact argument map before prose:

```text
world/problem → importance → representative approaches → shared gap
→ proposed idea → mechanism preview → evidence/payoff → contributions
```

## The five-move template

### Move 1 — World and stakes (usually one paragraph, about four sentences)

**Purpose:** orient the reader from the field to the paper's exact setting and
make the problem worth solving.

- Sentences 1–3 narrow from the broad field to the specific subproblem.
- Sentence 4 states why the subproblem matters: a failure mode, scientific
  bottleneck, operational cost, or attribution/safety consequence.
- Prefer concrete nouns and a named setting over “AI is transforming...”
  generalities.
- The last sentence should create stakes without previewing every module.

**Diagnostic:** Can a reader answer “what world are we in?” and “why should I
care?” after this paragraph?

### Move 2 — Existing approaches and the shared conflict (often 3+1+2 sentences)

**Purpose:** show that the gap is real, shared, and consequential—not that
individual prior papers are wrong.

- Sentences 1–3 summarize two representative approaches or camps, one idea per
  sentence; cite them in argumentative groups.
- Sentence 4 is the pivot: “Despite this progress, they share...” or an
  equivalent precise transition.
- Sentences 5–6 unpack the common limitation and its consequence for the paper's
  target outcome.
- Critique the abstraction or missing interface, not the competence of prior
  authors.
- If approaches solve different subproblems, state the boundary rather than
  forcing a false common flaw.

**Diagnostic:** Is there one shared limitation that the proposed method can
actually address? If not, revise the gap before writing the method paragraph.

### Move 3 — Proposed idea / protagonist entrance (usually five sentences)

**Purpose:** answer the shared limitation directly with a memorable method
thesis.

- Sentence 1 explicitly bridges from the gap: “We address this by...”
- Sentences 2–4 preview the core representation, protocol, or operation in
  reader-level terms; defer implementation minutiae.
- Sentence 5 states the key advantage as a conditional, evidence-compatible
  claim—not an unsupported universal promise.
- Name the unit of intervention: artifact, interface, protocol, training signal,
  estimator, or evaluation design.

**Diagnostic:** Could a reader explain in one sentence why this idea targets the
previous paragraph's exact failure?

### Move 4 — Mechanism and innovation (usually five sentences)

**Purpose:** make the method believable by showing how its parts solve the gap.

- Sentence 1 names the operational contract or central mechanism.
- Sentences 2–4 introduce the core components in the order a run uses them;
  each component must map to one part of the shared limitation.
- Sentence 5 explains the cooperation among components and previews the
  evaluation or verification path.
- Keep only details needed to understand novelty, not a miniature Methods
  section. Use notation only if it reduces ambiguity.

For each component, fill this relation before drafting:

```text
component → operation → failure mode addressed → observable evidence
```

A component without a distinct failure mode or observable consequence is likely
scaffolding, not an Introduction-level innovation.

### Move 5 — Contribution payoff (three to four bullets)

**Purpose:** close the narrative with independently checkable achievements.

Use parallel, verb-led bullets. A useful default set is:

1. **Concept/method:** We formulate or introduce the new problem framing or
   artifact-level principle.
2. **Mechanism/protocol:** We design the mechanism that addresses the stated
   gap and specify what it exposes or constrains.
3. **Evidence/evaluation:** We build the benchmark, instrumentation, dataset,
   or paired evaluation that tests attribution and outcome.
4. **Finding/application (only if supported):** We report the measured result,
   boundary, or reusable artifact with its exact scope.

Use verbs such as *formulate, introduce, bind, instrument, reconstruct,
separate, measure, compare,* and *reveal*. Avoid noun stacks like “a novel,
robust, general framework.” Every bullet must be independently meaningful and
map back to a problem or mechanism already introduced.

## Citation and tension rules

- Build citation “camps”: group papers by the strategy they use and state the
  distinction between groups.
- Prefer “Prior work provides X, while another line provides Y; neither makes
  Z observable under this setting” over A/B/C inventory prose.
- The gap is a shared abstraction-level limitation, missing interface, or
  evaluation blind spot—not a claim that prior work is useless.
- Use a real transition at the paragraph boundary: progress → common gap →
  response. If the transition can be deleted without changing meaning, the
  tension is probably missing.
- Keep one dominant conflict. Multiple unrelated “gaps” make the method look
  like a bundle of features.

## Evidence and language guardrails

Before finalizing any sentence, classify it:

- **Background:** supported by field knowledge/citations.
- **Prior-work relation:** supported by the cited papers.
- **Proposal:** what this paper intends to introduce.
- **Derived result:** computed from the paper's data or evaluation.
- **Interpretation:** an explanation bounded by the design.

Then enforce:

- Do not write “first,” “state of the art,” “proves,” “guarantees,” or
  “across domains” without checking the relevant literature or experiment.
- Do not use an all-pass or non-significant result as automatic non-inferiority.
- Do not call exposure, loading, invocation, or co-occurrence evidence of
  governance; distinguish assigned condition, observed exposure, action/effect,
  and independent verification when those states matter.
- Report missing evidence as unknown rather than zero, success, or compliance.
- If the user supplies simulated or planned results, label them as design
  placeholders and keep them out of empirical contribution claims.

## Revision workflow

1. **Extract:** write the one-sentence problem, stakes, common gap, proposed
   unit, mechanism, and strongest supported payoff.
2. **Map:** fill the five moves and the component-to-failure-mode table.
3. **Stress-test:** check that Move 3 directly answers Move 2, Move 4 explains
   Move 3, and each contribution bullet has evidence or an explicit proposal
   label.
4. **Draft:** write concise publication prose with citation groups and explicit
   transitions. Keep the analogy invisible in the final text.
5. **Audit:** run the checklist below; identify unsupported claims separately
   from style opportunities.
6. **Deliver:** if revising text, put the copy-ready replacement first; then
   provide a short rationale, evidence gaps, and optional variants.

For a manuscript rewrite, inspect the actual abstract, title, method, results,
venue constraints, and references before asserting that the Introduction is
aligned. Do not replace technical content with a generic template.

## Introduction self-check

- [ ] Paragraph 1 narrows from field to concrete setting and ends with stakes.
- [ ] Paragraph 2 uses representative prior-work camps, not a citation list.
- [ ] A single shared limitation is explicitly named and consequential.
- [ ] Paragraph 3 answers that limitation in its first sentence.
- [ ] The proposed unit and advantage are concrete and scope-bounded.
- [ ] Paragraph 4 maps each mechanism to a failure mode and observable evidence.
- [ ] Contribution bullets use verbs and correspond to earlier claims.
- [ ] No paragraph is a detached literature summary, method dump, or result dump.
- [ ] The Introduction does not claim more than the experiments or citations can
      support.
- [ ] Unknown, proposed, derived, and observed states are not conflated.
- [ ] The final sentence or contribution block makes the paper's payoff easy to
      retrieve.

## Output format

For an outline, return:

1. one-sentence thesis;
2. the five-move argument map;
3. paragraph-by-paragraph purpose and transition;
4. contribution bullets;
5. evidence/claim risks and missing inputs.

For a rewrite, return the copy-ready Introduction first (normally in a `tex`
fence if the user requests LaTeX), followed by:

- a compact map from each paragraph to the gap and evidence;
- claims that need verification or narrowing;
- at most two alternative opening or contribution variants when useful.

Read `references/introduction-arc-worksheet.md` when a structured worksheet,
example diagnosis, or component-to-evidence table would materially improve the
current task.
