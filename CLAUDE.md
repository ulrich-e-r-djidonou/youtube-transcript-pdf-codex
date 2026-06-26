# CLAUDE.md

## Project

This repository publishes a Codex skill for creating readable PDF transcripts from YouTube videos.

## Rules

- Keep generated transcripts and PDFs out of Git.
- Keep upstream MIT attribution intact.
- Preserve UTF-8 handling for all transcript, Markdown, JSON, and audit files.
- Keep Windows Chrome/Edge detection working.
- For French captions, keep French document labels and disable English topic headings.

## Verification

```powershell
python -m py_compile scripts\youtube_transcript_pdf.py
```
