# youtube-transcript-pdf-codex

Codex skill for generating readable PDF transcripts from YouTube videos.

This is a Windows-ready fork/adaptation of the `youtube-transcript-pdf` skill from [aniketpanjwani/skills](https://github.com/aniketpanjwani/skills), originally licensed under MIT.

## What This Fork Adds

- Windows Chrome/Edge detection for PDF rendering.
- UTF-8-safe reading and writing for JSON, TXT, Markdown, HTML, and audit files.
- UTF-8-safe `codex exec` subprocess prompts for non-English transcripts.
- French document labels when captions are detected as French.
- Disabled English topic headings for French transcripts.
- Long dash normalization in YouTube titles.

## Install In Codex

```powershell
python C:\Users\ciram\.codex\skills\.system\skill-installer\scripts\install-skill-from-github.py --repo ulrich-e-r-djidonou/youtube-transcript-pdf-codex --path .
```

Restart Codex after installing.

## Usage

```powershell
python scripts\youtube_transcript_pdf.py "https://www.youtube.com/watch?v=VIDEO_ID" --lang fr --no-whisper --summary-provider extractive
```

The default output directory is `youtube-transcripts/<video_id>/`.

## Attribution

Original skill source: [aniketpanjwani/skills](https://github.com/aniketpanjwani/skills/tree/main/skills/general/youtube-transcript-pdf)

License: MIT, copyright Aniket Panjwani. See [LICENSE](LICENSE).
