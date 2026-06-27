# Project Log

## 2026-06-26

Created a public repository dedicated to the corrected `youtube-transcript-pdf` Codex skill.

Source:

- Repository: `https://github.com/aniketpanjwani/skills`
- Path: `skills/general/youtube-transcript-pdf`
- License: MIT

Corrections included:

- Windows Chrome/Edge detection.
- UTF-8-safe file reads and writes.
- UTF-8-safe `codex exec` subprocess prompts.
- French labels for French captions.
- Disabled English topic headings for French captions.
- Long dash normalization in YouTube titles.

Validation:

- `python -m py_compile scripts\youtube_transcript_pdf.py`
- PDF generation smoke test validated on Windows.
