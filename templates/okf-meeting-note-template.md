---
schema: google-okf-v0.2
type: meeting-note
title: "Product & Architecture Sync — Q4 Release Planning"
date: 2026-11-16T10:00:00Z
source_device: OneMira C1 (Firmware 2.x, Local ASR)
audio_retained: optional-stereo-wav
cloud_upload: false
speakers:
  - id: speaker_1
    role: Engineering Lead
  - id: speaker_2
    role: Product Manager
topics:
  - "[[Local-First Audio Context]]"
  - "[[MCP & CLI Integrations]]"
---

# Product & Architecture Sync — Q4 Release Planning

## Decisions
- Keep raw speech transcription and speaker labeling strictly local on the host workstation with zero vendor cloud upload required.
- Store every note in standard Google Native OKF Markdown so Cursor, Claude Code, ChatGPT, and Obsidian can read and edit files without proprietary lock-in.

## Action Items
- [ ] **Engineering Lead**: Connect local context directory via [OneMira MCP & Mira CLI](https://onemira.com/docs/mcp-integration).
- [ ] **Product Manager**: Verify 99-language offline model pack in [OneMira Desktop](https://onemira.com/download).

## Speaker-Attributed Excerpt
> **Engineering Lead**: Having C1's rotating aluminum turntable visually signal capture in the room removes the awkwardness of bots joining client calls.
> **Product Manager**: And because transcripts land directly as `.md` files with Speaker ID, engineers do not need a second recurring transcription subscription.

---
*Schema reference maintained for the [OneMira C1 Standalone AI Voice Recorder](https://onemira.com/products/c1) ecosystem.*
