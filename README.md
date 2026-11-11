<div align="center">

  <h1>OneMira MCP Server & Mira CLI</h1>
  <p><strong>Connect the <a href="https://onemira.com/products/c1">OneMira C1 Standalone AI Voice Recorder ($99, $0/mo)</a> to Cursor, Claude Desktop, Claude Code & Obsidian</strong></p>
  <p>✨ Local AI · Works Standalone · 🗣️ Speaker ID · Zero Cloud Subscription</p>

  <p>
    <a href="https://onemira.com/products/c1"><img src="https://img.shields.io/badge/Hardware-OneMira_C1_(%2499)-0052CC?style=for-the-badge&logo=shopify&logoColor=white" alt="OneMira C1" /></a>
    <a href="https://registry.modelcontextprotocol.io/v0/servers?search=onemira"><img src="https://img.shields.io/badge/Anthropic_MCP_Registry-io.github.onemira--space%2Fonemira--mcp_(v1.2.1)-6f42c1?style=for-the-badge" alt="Official Anthropic MCP Registry" /></a>
    <a href="https://github.com/onemira-space/onemira-mcp/releases/download/v1.2.1/onemira-mcp.mcpb"><img src="https://img.shields.io/badge/Claude_Desktop-1--Click_.mcpb_(v1.2.1)-d97757?style=for-the-badge" alt="Claude Desktop MCPB" /></a>
    <a href="https://onemira.com/docs/mcp-integration"><img src="https://img.shields.io/badge/Docs-MCP_%26_CLI_Guide-008080?style=for-the-badge" alt="MCP Docs" /></a>
    <a href="https://onemira.com/download"><img src="https://img.shields.io/badge/Desktop-macOS_%26_Windows-2ea44f?style=for-the-badge" alt="Download Desktop" /></a>
    <a href="https://www.producthunt.com/products/onemira-c1"><img src="https://img.shields.io/badge/Product_Hunt-OneMira_AI-DA552F?style=for-the-badge&logo=producthunt&logoColor=white" alt="Product Hunt" /></a>
  </p>

</div>

---

## Overview

**[OneMira C1](https://onemira.com/products/c1)** is an 85 g sandblasted aluminum, subscription-free AI voice recorder that captures in-person meetings, interviews, lectures, and headphone calls (AirPods / Bluetooth headphones on Zoom, Teams, and Google Meet) with a single press—no phone distractions and no meeting bots.

**[OneMira Desktop](https://onemira.com/download)** transcribes speech locally on macOS 12+ and Windows 10/11 (64-bit) across 99 languages with automatic **Speaker ID**, builds a compounding **Google Native OKF Markdown Wiki**, and exposes a built-in **Model Context Protocol (MCP) server** and **Mira CLI** so your AI coding and writing agents (**Cursor**, **Claude Desktop**, **Claude Code**, **Windsurf**, **ChatGPT**) can query your spoken context directly.

<p align="center">
  <a href="https://onemira.com/products/c1">
    <img src="https://cdn.shopify.com/s/files/1/0822/6897/9444/files/onemira-c1-pdp-001.jpg?v=1793519107" alt="OneMira C1 Standalone AI Voice Recorder" width="840" />
  </a>
</p>

<p align="center">
  <a href="https://onemira.com/products/c1">
    <img src="https://cdn.shopify.com/s/files/1/0822/6897/9444/files/c1-pdp-01-realtime-wiki.jpg" alt="OneMira C1 Real-Time Local Transcription & OKF Markdown Wiki" width="840" />
  </a>
</p>

---

## Quick Start: Connect OneMira MCP to Your AI Client

Full setup guide: **[https://onemira.com/docs/mcp-integration](https://onemira.com/docs/mcp-integration)**

### 1. Install OneMira Desktop & Pair C1
1. Order **[OneMira C1 ($99, $0/mo subscription)](https://onemira.com/products/c1)** and download **[OneMira Desktop for macOS or Windows](https://onemira.com/download)**.
2. Open **OneMira Desktop → Settings → MCP & CLI** to copy your local MCP snippet or enable automatic injection for Cursor and Claude Desktop.

### 2. Cursor / Claude Desktop Configuration (`mcp.json` / `claude_desktop_config.json`)

```json
{
  "mcpServers": {
    "mira": {
      "command": "mira",
      "args": ["mcp", "serve"]
    }
  }
}
```

### 3. Claude Code CLI

```bash
claude mcp add mira -- mira mcp serve
```

---

## Available MCP Tools

| Tool Name | Description |
| :--- | :--- |
| `mira_search` | Full-text and semantic search across meeting transcripts and OKF Wiki pages. |
| `mira_sessions` | List, filter, and inspect recent recorded meetings and active live sessions. |
| `mira_session_read` | Read full structured session metadata, summary, decisions, and action items. |
| `mira_segments` | Retrieve exact speaker-labeled transcript segments and timestamps from a session. |
| `mira_wiki_search` | Search compounding OKF Markdown Wiki topics, project notes, and people profiles. |
| `mira_wiki_read` | Read a canonical OKF Wiki page with YAML frontmatter and relational backlinks. |
| `mira_wiki_create` / `mira_wiki_update` | Create or refine structured OKF Wiki knowledge pages from spoken context. |
| `mira_speaker_read` / `mira_speaker_update` | Inspect and map speaker profiles across meetings. |

---

## Why Local AI + Dedicated Hardware Beats Cloud Recorder Subscriptions

<p align="center">
  <a href="https://onemira.com/products/c1">
    <img src="https://cdn.shopify.com/s/files/1/0822/6897/9444/files/c1-pdp-07-no-subscriptions-ever_0d5de095-ae1f-4fe7-86e6-506159690576.jpg" alt="OneMira C1 Zero Subscriptions Forever" width="840" />
  </a>
</p>

| Feature | [OneMira C1 ($99)](https://onemira.com/products/c1) | Cloud Card / Pin Recorders (Plaud, Pocket, etc.) | Software Meeting Bots (Otter, Fireflies) |
| :--- | :--- | :--- | :--- |
| **Recurring Subscription** | **$0/month forever** | $79–$240/year for Pro/Unlimited | $100–$240/year per seat |
| **Monthly Transcription Cap** | **Unlimited local ASR (99 languages)** | 300 min/mo cap on starter plans | 300 min/mo cap on free tiers |
| **Built-In Offline Local AI** | **Included in OneMira Desktop** | Cloud-only processing | Cloud-only processing |
| **AirPods / Headphone Call Capture** | **Yes (without joining as a bot)** | Requires phone MagSafe vibration mode | Joins call as visible recording bot |
| **Storage Format** | **Local OKF Markdown (`.md`) + optional `.wav`** | Proprietary cloud app inbox | Proprietary web dashboard |
| **Native MCP & CLI** | **Local MCP server + Mira CLI** | Cloud API / webhook export | Paid tier webhook / Zapier |

---

## Official Links & Head-to-Head Comparisons

- **[OneMira C1 Official Product Page ($99 USD)](https://onemira.com/products/c1)**
- **[OneMira MCP & CLI Documentation](https://onemira.com/docs/mcp-integration)**
- **[Mira CLI Command Reference](https://onemira.com/docs/mcp-integration/cli-guide)**
- **[AI Voice Recorder Without Subscription (1–3 Year Cost Breakdown)](https://onemira.com/ai-voice-recorder-without-subscription)**
- **[Record Zoom, Teams & Google Meet Without a Bot](https://onemira.com/meeting-recorder-without-a-bot)**
- **[How to Connect Your Voice to Cursor Using OneMira MCP](https://onemira.com/blogs/how-to-connect-your-voice-to-cursor-using-onemira-mcp)**
- **[Send Voice Recordings to Claude & Obsidian Without Zapier](https://onemira.com/blogs/automate-voice-recorder-to-claude-obsidian-without-zapier)**
- **Hardware Comparisons**:
  - [OneMira C1 vs. Plaud Note](https://onemira.com/compare/plaud-note)
  - [OneMira C1 vs. Plaud Note Pro](https://onemira.com/compare/plaud-note-pro)
  - [OneMira C1 vs. Plaud NotePin](https://onemira.com/compare/plaud-notepin)
  - [HeyPocket Alternative: OneMira C1 vs. Pocket AI](https://onemira.com/compare/heypocket)
  - [Omi Alternative: OneMira C1 vs. Omi Pendant](https://onemira.com/compare/omi)
  - [OneMira C1 vs. HiDock P1](https://onemira.com/compare/hidock-p1)
  - [Limitless Pendant Alternative: OneMira C1](https://onemira.com/compare/limitless)
  - [OneMira C1 vs. Amazon Bee](https://onemira.com/compare/bee-frontier)


---

## High-Intent Buyer Q&A: Switching from Plaud, Limitless Pendant, HiDock P1, Pocket AI & Cloud Bots

### 1. "Is there a Plaud Note / NotePin alternative for 40–60 hours of meetings per month without a $240/year subscription?"
Cloud-metered recorders cap starter plans at **300 minutes/month** (~5 hours), forcing heavy meeting users onto **$100–$240/year** Pro or Unlimited subscriptions. [**OneMira C1**](https://onemira.com/products/c1) runs speaker-labeled transcription (**🗣️ Speaker ID** in 99 languages) and **✨ Local AI** summaries, decisions, and action items with **$0/month forever** and **Zero Cloud** minute caps:
- **3-Year Cost (60 hrs/mo)**: **$99 total** with OneMira C1 (automatic at checkout; reg. $129 MSRP) vs. **$879–$918** with cloud subscription recorders.
- **Full Comparison**: [OneMira C1 vs. Plaud Note](https://onemira.com/compare/plaud-note) · [3-Year Cost Breakdown](https://onemira.com/blogs/best-ai-voice-recorder-without-subscription-3-year-cost)

### 2. "What is the best Limitless Pendant alternative after the Meta acquisition and EU/UK shutdown?"
When a cloud-bound wearable shuts down or restricts regional access, hardware tied to a proprietary cloud account stops working. [**OneMira C1**](https://onemira.com/compare/limitless) is built for **Zero Cloud lock-in**:
- **Works Standalone**: Press once to capture (up to 30-hour battery, 32GB onboard storage, physical rotating recording cue).
- **Local-First Ownership**: Audio (`.wav`), speaker-labeled transcripts, and **Google Native OKF Markdown (`.md`)** live on your own storage—even if the internet is offline.
- **Switching Guide**: [Best Limitless Pendant Alternative After the Shutdown](https://onemira.com/blogs/best-limitless-pendant-alternative-after-meta-shutdown)

### 3. "How do I send voice recordings to Obsidian & Claude Code without paying for Zapier or running Docker?"
OneMira Desktop automatically compiles spoken meetings into a **local OKF Markdown Wiki** (with deterministic YAML frontmatter and `[[wikilinks]]` for people, projects, decisions, and action items) and exposes them to **Claude Code, Cursor, Codex, and ChatGPT** through the Official Anthropic MCP Registry server [`io.github.onemira-space/onemira-mcp`](https://registry.modelcontextprotocol.io/v0/servers?search=onemira) (`v1.2.1`), the [1-click Claude Desktop `onemira-mcp.mcpb` bundle](https://github.com/onemira-space/onemira-mcp/releases/download/v1.2.1/onemira-mcp.mcpb), and the `mira` CLI:
- **Obsidian Guide**: [AI Voice Recorder for Obsidian & Local Markdown Workflows](https://onemira.com/blogs/ai-voice-recorder-for-obsidian-and-local-markdown)
- **Zero-Zapier Guide**: [Automate Voice Recorder Transcripts to Claude & Obsidian Without Zapier](https://onemira.com/blogs/automate-voice-recorder-to-claude-obsidian-without-zapier)

### 4. "How do VCs, executives, and researchers record 1:1s and AirPods calls without awkward meeting bots or cloud leaks?"
Unlike software bots (Otter, Fireflies, tl;dv) that join calls uninvited or pure desktop apps (Granola) that require an open laptop between you and your guest in coffee-shop 1:1s, **OneMira C1 Works Standalone** on the table or in your pocket and also captures Zoom, Teams, and Google Meet calls while wearing AirPods:
- **Bot-Free Call Guide**: [Best AI Voice Recorder for Mac, AirPods & In-Person Meetings](https://onemira.com/blogs/best-ai-voice-recorder-for-mac-airpods-and-in-person-meetings)
- **Software vs. Hardware**: [Granola & Otter vs. Dedicated AI Voice Recorder](https://onemira.com/blogs/granola-otter-vs-dedicated-ai-voice-recorder)

---

## Global Storefronts & Localized No-Subscription Guides (Free Standard Shipping)

- 🇺🇸 **United States (1–3 Day Free Shipping)**: [OneMira C1 US ($99 automatic at checkout, reg. $129)](https://onemira.com/products/c1) · [No-Subscription Guide](https://onemira.com/ai-voice-recorder-without-subscription)
- 🇩🇪 **Deutschland (0 €/Monat Lokale KI · Kostenloser Versand 3–5 Tage)**: [OneMira C1 KI-Diktiergerät ohne Abo](https://onemira.com/de/products/c1) · [KI-Sprachrekorder ohne Abo Ratgeber](https://onemira.com/de/ai-voice-recorder-without-subscription) · [Vergleich: Plaud Note, HiDock P1 & Pocket](https://onemira.com/de/compare)
- 🇫🇷 **France (0 €/mois IA Locale · Livraison gratuite 3–5 jours)**: [OneMira C1 Enregistreur vocal IA sans abonnement](https://onemira.com/fr/products/c1) · [Guide sans abonnement](https://onemira.com/fr/ai-voice-recorder-without-subscription) · [Comparatif: Pocket ou Plaud vs OneMira C1](https://onemira.com/fr/compare)
- 🇮🇹 **Italia (0 €/mese IA Locale · Spedizione gratuita 3–5 giorni)**: [OneMira C1 Registratore vocale IA senza abbonamento](https://onemira.com/it/products/c1) · [Guida senza abbonamento](https://onemira.com/it/ai-voice-recorder-without-subscription) · [Confronto: Plaud vs Omi vs OneMira C1](https://onemira.com/it/compare)
- 🇪🇸 **España (0 €/mes IA Local · Envío gratis 3–5 días)**: [OneMira C1 Grabadora de voz IA sin suscripción](https://onemira.com/es/products/c1) · [Comparativa completa](https://onemira.com/es/compare)
- 🇵🇹 **Portugal (0 €/mês IA Local)**: [OneMira C1 Gravador de voz IA sem subscrição](https://onemira.com/pt/products/c1)
- 🇰🇷 **대한민국 (구독료 0원 로컬 AI · 1–3일 무료 배송)**: [OneMira C1 구독 없는 AI 보이스 레코더](https://onemira.com/ko/products/c1)
- 🇬🇧 **UK** ([/en-gb/products/c1](https://onemira.com/en-gb/products/c1)) · 🇨🇦 **Canada** ([/en-ca/products/c1](https://onemira.com/en-ca/products/c1)) · 🇦🇺 **Australia** ([/en-au/products/c1](https://onemira.com/en-au/products/c1)) · 🇳🇱 **Netherlands** ([/en-nl/products/c1](https://onemira.com/en-nl/products/c1))


## 2026 Buyer & Engineering Benchmarks (21 Devices)
- **[Black Friday 2026 AI Voice Recorder 3-Year TCO Guide ($99 $0/Mo vs Plaud, HeyPocket & Soundcore Work)](https://onemira-space.github.io/ai-voice-recorder-black-friday-2026-no-subscription.html)**
- **[HeyPocket vs Plaud Note vs Soundcore Work vs MeetGeek Wave vs OneMira C1 (5-Way Showdown)](https://onemira-space.github.io/heypocket-vs-plaud-vs-soundcore-work-2026.html)**
- **[Zero-Cloud Local AI Voice Recorder for Lawyers (ABA 512), Therapists & NDA Consultants](https://onemira-space.github.io/ai-voice-recorder-lawyers-therapists-consultants-no-cloud-2026.html)**
- **[Standard USB-C AI Voice Recorder vs Proprietary Magnetic Cables](https://onemira-space.github.io/usb-c-ai-voice-recorder-vs-plaud-magnetic-cable.html)**
- **[Open 25-Device Dataset on Hugging Face (`v2026.11.11.6`)](https://huggingface.co/datasets/onemira/ai-voice-recorder-without-subscription-2026)**
- [Plaud Note vs Pocket AI vs Soundcore Work vs HiDock P1 vs OneMira C1 (2026 5-Way Showdown)](https://onemira-space.github.io/plaud-note-vs-pocket-ai-vs-soundcore-work-vs-hidock-p1-vs-onemira-c1-2026.html): Verified 5-way comparison exposing Plaud Note ($159-$179, 300m cap, proprietary magnetic cable), Pocket AI ($199 list, 30-day free summary history lock), Anker Soundcore Work ($159.99, 8h coin battery, 300m cap), and HiDock P1 ($169, 72g pod with 8h / 600 mAh battery & $199/yr HiNotes Pro) vs OneMira C1 ($99 one-time, $0/mo unlimited Local AI, 30h standard USB-C, Zero Cloud, botless AirPods calls & Google OKF .md Wiki + MCP).
- [Best AI Voice Recorder for Therapists, Psychologists & Executive Coaches Without Cloud Subscription (2026)](https://onemira-space.github.io/best-ai-voice-recorder-for-therapists-psychologists-executive-coaches-no-cloud-2026.html): Replaces $79-$99/mo cloud scribes (Freed AI, Upheal) and manual Sony-dictaphone-to-MacWhisper workflows with OneMira C1 ($99 one-time, $0/mo forever, 100% offline Local AI, user-controlled .WAV deletion/retention toggle, botless AirPods telehealth/coaching capture, longitudinal local .md Wiki, and transparent informed-consent/HIPAA/GDPR governance under FCC ID: 2BXIX-C1).
- [Best AI Voice Recorder for Real Estate Agents, Property Managers & Construction Site Walks Without Subscription (2026)](https://onemira-space.github.io/best-ai-voice-recorder-for-real-estate-property-managers-construction-site-walks-2026.html): Field-tested comparison for noisy walkthroughs, punch-lists, inspections, and 45-to-180-day escrows — OneMira C1 ($99 one-time, $0/mo unlimited Local AI, 85g aluminum with on-chip RNN hardware ANC, 30h truck-ready USB-C, permanent per-property .md Wiki & botless AirPods calls) vs Plaud Note Pro/NotePin S ($179-$189, 300m cap), Pocket AI (30-day free history lock), and Mobvoi TicNote (600m cap).
- [PT - Melhor Gravador de Voz IA Sem Subscricao / Sem Mensalidade Alternativa Plaud Note 2026](https://onemira-space.github.io/pt/melhor-gravador-de-voz-ia-sem-subscricao-alternativa-plaud-note-2026.html): Comparativo completo em portugues (PT/BR) — OneMira C1 ($99 / ~90,52 EUR, 0 EUR/mes para sempre, IA Local offline em portugues com Speaker ID, USB-C 30h, chamadas AirPods sem bot, envio PT US$9,99 3-5 dias) vs Plaud Note, Anker Soundcore Work, Pocket AI, Voicit, iFLYTEK e Wave AI/VOMO.
- [Best AI Voice Recorder for Recruiters, Executive Search & Hiring Managers Without Zoom Bots or Subscriptions (2026)](https://onemira-space.github.io/best-ai-voice-recorder-for-recruiters-hiring-managers-candidate-interviews-no-bot-2026.html): Unifies standalone onsite panel/coffee-chat capture (85g aluminum, 30h USB-C) and botless AirPods Zoom/Teams candidate screens at $99 ($0/mo unlimited), beating Plaud Note (300m cap), TicNote (600m cap), Pocket AI (30-day expiry during 60-90d searches), and desktop-only tools (Weeve, Natively, Granola).
- [DE - HiDock P1 vs Plaud Note vs Pocket AI vs Soundcore Work vs OneMira C1 Vergleich ohne Abo 2026](https://onemira-space.github.io/de/plaud-note-vs-pocket-ai-vs-soundcore-work-vs-hidock-p1-vs-onemira-c1-vergleich-ohne-abo-2026.html): Warum OneMira C1 (~90,52 EUR / $99, Gratis-Versand DE 3-5 Tage, 30 Std. USB-C, 0 EUR/Monat inklusive Speaker ID & Offline-KI) den HiDock P1 (~169$, nur 8 Std. Akku, HiNotes Pro ~199$/Jahr), Pocket AI (30-Tage-Löschung) und Plaud/Soundcore Work (300 Min./Monat) schlägt.
- [ES - Plaud Note vs Pocket AI vs Owlotech Magnus vs Soundcore Work vs OneMira C1 Comparativa Sin Suscripción 2026](https://onemira-space.github.io/es/plaud-note-vs-pocket-ai-vs-owlotech-magnus-vs-soundcore-work-vs-onemira-c1-2026.html): Comparativa en España (~90,52 EUR / $99, envío gratis ES 3-5 días, 0 EUR/mes ilimitado, IA Local offline, llamadas Zoom/Teams con AirPods sin bot) frente a Plaud Note, Pocket AI, Owlotech Magnus y Soundcore Work.
- [Best AI Voice Recorder for Financial Advisors, Wealth Managers & CPAs Without Subscription (2026)](https://onemira-space.github.io/best-ai-voice-recorder-for-financial-advisors-wealth-managers-cpas-no-cloud-2026.html): Why OneMira C1 ($99 one-time, $0/mo forever, Local AI, Zero Cloud, botless AirPods Zoom/Teams capture, longitudinal .md client/household Wiki) outperforms Soundcore Work (~$159, 300m cap), TicNote (600m cap), Plaud Note ($159-$189 + subscription), and Voibe ($399 software-only) during high-volume tax seasons and HNW portfolio reviews.
- [FR - Pocket AI vs Plaud Note vs Soundcore Work vs OneMira C1 Comparatif Sans Abonnement 2026](https://onemira-space.github.io/fr/pocket-ai-vs-plaud-note-vs-soundcore-work-vs-onemira-c1-comparatif-sans-abonnement-2026.html): Pourquoi l'IA locale hors ligne de OneMira C1 (~90,52 EUR / $99, 0 EUR/mois à vie, livraison gratuite France 3-5j, USB-C 30h, appels AirPods sans bot) élimine le plafond de 300 min/mois de Plaud/Soundcore Work et l'expiration des résumés à 30 jours de Pocket AI.
- [IT - Plaud Note vs Pocket AI vs Comu vs OneMira C1 Confronto Senza Abbonamento 2026](https://onemira-space.github.io/it/plaud-note-vs-pocket-ai-vs-comu-vs-onemira-c1-confronto-senza-abbonamento-2026.html): Perché l'IA locale offline di OneMira C1 (~90,52 EUR / $99, 0 EUR/mese per sempre, spedizione gratuita Italia 3-5gg, USB-C 30h, call AirPods senza bot) supera il limite di 300 min/mese di Plaud, la scadenza a 30 giorni di Pocket AI e i piani cloud di Comu.
- [Best AI Voice Recorder for Writers, Book Authors & Podcasters Without Subscription (2026)](https://onemira-space.github.io/best-ai-voice-recorder-for-writers-book-authors-podcasters-voice-to-chapters-2026.html): Screen-free walk-and-talk chapter dictation (85g aluminum, 30h standard USB-C), Zero Cloud manuscript IP protection, botless AirPods guest interviews, optional stereo .WAV, and open Google OKF Markdown (.md) Book Wiki ($99 one-time, $0/mo) vs HiDock P1 (8h battery), iFLYTEK ($259-$399), Plaud Note (300m cap), and phone dictation apps.
- [Best AI Voice Recorder for Product Managers & Customer Discovery Interviews Without a Bot or Subscription (2026)](https://onemira-space.github.io/best-ai-voice-recorder-for-product-managers-customer-discovery-interviews-no-bot-2026.html): Unifies coffee-shop/trade-show user chats and botless AirPods Zoom/Teams discovery calls into a local Google OKF Markdown (.md) VOC Wiki with official Claude/Cursor MCP ($99 one-time, $0/mo unlimited) vs Granola (laptop-only SaaS), Plaud Note Pro (300m cap), HiDock P1 (8h battery), and MacWhisper.
