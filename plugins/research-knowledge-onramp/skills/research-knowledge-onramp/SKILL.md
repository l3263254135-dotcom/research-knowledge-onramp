---
name: research-knowledge-onramp
description: Use when the user needs to enter a new course, paper, method family, technical field, or thesis topic from local files, PPTs, textbooks, articles, or notes; when they need research-first onboarding, paper critique, method comparison, novelty framing, baseline selection, proposal sketching, or a course pack explained at undergraduate, graduate, and doctoral levels.
---

# Research Knowledge Onramp

## Overview

Turn the user's materials into a research-first onramp. Work like a paper mentor and proposal assistant: first make the topic legible, then comparable, then designable.

## Core Workflow

1. Classify the task as coursework, research, or mixed.
2. Prefer local source material first.
3. Build a source map: core, support, supplemental, and uncertain.
4. Produce the first-pass deliverable.
5. Split the result into source-backed facts, informed inferences, and open questions.
6. Deepen with three-level explanation.
7. End with next actions, baselines, risks, or a compressed version if needed.

## Output Ladder

For every important concept, method, or paper, include:

- What problem it solves
- Formal definition
- Why the mechanism works
- Where it stops working
- How it is used in coursework or research
- Common limitations and failure cases
- One next question worth asking

Always explain at three levels when the user is learning from scratch:

- **本科层**: whiteboard-level intuition
- **研究生层**: mechanism, assumptions, and evaluation logic
- **博士层**: boundary, novelty, critique, and improvement direction

## Mentor Outputs

Use these default shapes when the user needs research help:

- `research onramp pack`: field map, concept map, method lineage, data/tasks/metrics, and reading order
- `paper mentor brief`: problem, claims, novelty, evidence, assumptions, baselines, limits, and follow-up papers
- `proposal starter pack`: research gap, question, hypothesis, minimal viable experiment, baselines, metrics, risks, and expected contribution
- `method boundary card`: what the method is good at, where it fails, how to compare it, and what a better version would need

## Evidence Discipline

Every research-facing output should visibly separate:

- `source-backed`: directly supported by the provided material
- `inference`: reasonable synthesis or interpretation
- `to verify`: claims, numbers, or comparisons that need more evidence

## Modes

### Coursework mode

Use when the user wants exam prep, chapter review, or a study pack.
Default to:

- course map
- chapter-by-chapter explanation
- formula meaning and variable notes
- calculation templates
- memorization version at the end

### Research mode

Use when the user wants to understand a paper, a method family, or a new research area.
Default to:

- knowledge map
- terminology map
- method lineage
- literature reading order
- research questions
- gaps and limitations
- possible project directions

### Paper mentor mode

Use when the user gives a paper, abstract, or reading list and wants more than a summary.
Default to:

- the real research problem
- what is actually new
- what evidence supports the claims
- what assumptions are hidden
- what baselines matter
- what would need to be reproduced or challenged next

### Proposal assistant mode

Use when the user has a topic idea, thesis direction, or method curiosity.
Default to:

- research gap
- candidate question
- hypothesis
- baseline set
- dataset or evidence plan
- evaluation metrics
- failure risks
- minimum viable study plan

### Mixed mode

Use when the user wants both study and research.
Default to a research-first onramp, then compress into exam or handoff form if requested.

## Guardrails

- Use local sources first.
- Do not flatten distinct methods into one generic summary.
- Separate facts, inferences, and open questions.
- Do not invent novelty or claim a gap without showing what it is relative to.
- Keep original files intact unless the user explicitly asks to overwrite.
- For append-only requests, add only the requested tail section.
- Prefer one strong example over many weak ones.
- When compressing to exam notes or slides, keep the research lineage intact instead of creating a second inconsistent story.

## References

Read the relevant reference only when needed:

- `references/source-intake-and-priority.md`
- `references/coursework-mode.md`
- `references/research-mode.md`
- `references/paper-mentor-mode.md`
- `references/proposal-advisor-mode.md`
- `references/paper-reading-and-deconstruction.md`
- `references/research-design-and-gap-finding.md`
- `references/output-skeletons.md`
- `references/usage-playbook.md`

## Example

User: "I need to learn this new topic from zero and also understand what research questions are still open."

Response shape:

1. Build a first-pass research onramp pack.
2. Explain the core concepts at three levels.
3. Summarize the method landscape and boundaries.
4. List the best next papers or subtopics.
5. Offer an exam or presentation compression if needed.
