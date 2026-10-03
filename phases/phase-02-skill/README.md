# Phase 2 — Gemini Skill

## Objective
Create the reusable Gemini Skill that operates the YouTube Shorts AI workflow using the canonical Phase 1 knowledge layer.

## Responsibility
The Skill defines how Gemini works: role, operating rules, workflow, evidence discipline, gates, and output contract. It does not duplicate the full knowledge base.

## Inputs
- Public YouTube Shorts URL
- YouTube video ID

## Core pipeline
Input normalization → video identification → full multimodal analysis → evidence classification → global reference → timeline → scene decomposition → generation prompt planning → validation → structured scene blueprint.

## Deliverables
- SKILL.md — canonical reusable Skill
- SKILL_ARCHITECTURE.md — responsibility boundaries
- OUTPUT_CONTRACT.md — output behavior and schema contract
- GATES.md — analysis/validation gates
- CHANGELOG.md

## Source of truth
Phase 1 knowledge is authoritative for product facts and locked project rules. Phase 2 must not silently redefine them.
