# Input Contract

## Accepted input
- Public YouTube Shorts URL
- YouTube video ID

## Normalization
Extract the canonical video ID and retain the original input for traceability.

## Invalid input
If the identifier cannot be resolved to the intended public video, stop before analysis and request a corrected input.

## Important distinction
A YouTube URL in NotebookLM is a knowledge-source workflow and is not equivalent to direct Gemini Video Understanding. The workflow must use the actual video-analysis capability for frame-level scene work.
