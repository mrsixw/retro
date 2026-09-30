---
name: retro
description: Review a completed agent session from its evidence and recommend concrete improvements to navigation, automation, standards, information access, and tool economy. Use when the user asks for a retrospective or lessons learned on finished work. Not for packaging unfinished work for another agent (use handoff).
---

# Retrospective

Recommend small durable controls for problems demonstrated by the completed
work. The output is an evidence-backed improvement list, not a general critique
of the agent or repository.

## Review what happened

Read the primary evidence: the session transcript, commands run and their
output, CI and validation output, corrections, and the final git state. For
each material friction point, classify it as:

- an execution mistake;
- a missing or unclear local convention;
- an absent automated guardrail;
- an information or access problem; or
- unavoidable complexity that should not become policy.

Check whether the issue recurred, could cause material harm, or is already
covered by an existing control.

## Recommend the cheapest reliable control

Prefer the narrowest durable layer that prevents or detects recurrence: an
existing check, repository documentation, a local skill, shared guidance, or
automation. Do not recommend a global rule when a local test or clearer command
would be more reliable.

For each recommendation, state the observed evidence, likely recurrence,
consequence, proposed owner and location, expected benefit, and validation
method. Rank by consequence and confidence. Include useful practices worth
preserving as well as failures worth correcting.

Do not edit the environment unless explicitly requested. One awkward incident
is not sufficient evidence for a universal rule.
