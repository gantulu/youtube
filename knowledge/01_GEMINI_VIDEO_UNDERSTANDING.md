# Gemini Video Understanding

## Authority
P0-A — Official Google AI for Developers.

## Source
https://ai.google.dev/gemini-api/docs/video-understanding

## What is supported
Gemini Video Understanding can process public YouTube URLs and other documented video inputs. Video understanding uses visual and audio information.

## Temporal processing
Static processing uses 1 FPS by default and supports custom sampling. Rapid motion and quick scene changes can be missed at low sampling rates. Agentic processing is available only on supported current models and should be selected from the current documentation/model catalog.

## Timestamps
Use MM:SS timestamp references when describing moments in the video.

## Project operating rule
Before producing scene output, inspect the complete timeline and verify fast events when the default sampling could miss them. Keep observed evidence separate from inference and unknowns. Never invent visual or audio details.

## Important boundary
This document describes understanding, not video generation.
