# Normalized Knowledge — Gemini Notebook / NotebookLM

## Authority
P0 — Official Google Gemini Notebook Help.

## Canonical source
https://support.google.com/gemininotebook/answer/16215270

## Product facts

Gemini Notebook can use imported sources as context for answering questions and completing requests.

Documented source types include:
- Google Docs;
- Google Slides;
- Google Sheets;
- images;
- audio;
- Markdown, text, PDF, CSV, DOCX, and PPTX files;
- web URLs;
- public YouTube URLs with captions.

### YouTube source behavior
- Only public YouTube videos with captions are supported.
- Only the text transcript is imported as the YouTube source.
- Videos without speech are not supported for this YouTube-source workflow.
- A newly uploaded video may be unavailable for import for up to 72 hours.
- If a YouTube video is deleted or made private, its source can be removed from the notebook within 30 days.
- The transcript has a documented 500,000-word ceiling.

### Web URL behavior
For ordinary web URLs, NotebookLM imports the page's text content. Embedded images, videos, and nested pages are not imported as source content.

### Google Drive behavior
Google Drive sources can be imported and are automatically synchronized periodically. Changes to the original Drive document can propagate to the Notebook source.

## Project interpretation

1. NotebookLM is a knowledge/reference layer, not the primary video-understanding engine for visual scene analysis.
2. A YouTube URL added to NotebookLM should not be treated as equivalent to Gemini Video Understanding of the original video because the documented YouTube source imports the transcript text.
3. Canonical project knowledge should therefore be stored as structured Markdown/Docs sources and used by NotebookLM for retrieval and context.
4. Visual video analysis remains a separate Gemini Video Understanding operation.
5. GitHub remains the versioned project-of-record; NotebookLM is the knowledge workspace.

## Consequence for the project

The system should not depend on NotebookLM to preserve frame-level visual evidence from a YouTube Short. It can preserve and retrieve textual knowledge, rules, documentation, and transcripts, while the video analyzer performs the actual multimodal video inspection.
