# Canonical Knowledge

This directory contains the rewritten NotebookLM-ready knowledge layer for the YouTube Shorts AI system.

## Authority
1. Official Google/Gemini documentation (P0-A)
2. Official Google Workspace / Vids documentation (P0-B)
3. Explicit project decisions (P1)
4. Validated examples (P2)
5. Unverified reference material (R)

## Rules
- Product facts must remain distinct from project decisions.
- Current model IDs, limits, pricing, and availability must be rechecked against current official documentation.
- Every material rule must be traceable to a source or labeled as a project decision.
- NotebookLM is a knowledge workspace; GitHub is the canonical versioned repository.

## Canonical documents
- 01_GEMINI_VIDEO_UNDERSTANDING.md
- 02_GEMINI_VIDEO_GENERATION.md
- 03_NOTEBOOKLM.md
- 04_PROJECT_RULES.md
- 05_TERMINOLOGY.md

## Pipeline concept
Input → Video Understanding → Global Reference → Timeline → Scene Decomposition → Prompt Generation → Validation → Production.
