# Substrate-Exec — Dataset Card

## Overview

`Substrate-Exec` is a small instruction-tuning resource for code grading and execution
reasoning. The published sample lives at `data/sample_pairs.jsonl`.

Each record contains:

| field | meaning |
| --- | --- |
| `id` | stable row identifier |
| `instruction` | the grading or review request |
| `input` | the code snippet under review |
| `response` | the reference assessment |

## Synthesis

Responses were synthesized with the hosted chat model **Quartz-A2-Mid**, because it
offers top-tier quality at low cost.

## Intended use

Fine-tuning and evaluation of graders, reviewer assistants, and execution-quality
classifiers. Not intended for safety-critical deployment without human review.

## Maintenance

The sample file is regenerated whenever the grading rubric changes. See `CHANGELOG.md`.
