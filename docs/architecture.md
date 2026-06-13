# Architecture — Sutta Nipata

## Overview

Sutta Nipata is a **static multi-page mini site** hosted on GitHub Pages. It is spoke 8 in the hub-and-spoke model under The Dharma Gate portal, following the same architecture as all other DharmaGate scripture sites.

- The **hub** is [The Dharma Gate](https://lugh3456.github.io/DharmaGate/)
- This **spoke** is a standalone repository with its own index and 71 section pages
- The hub links to this site; this site links back via portal bar and footer

HTML + external CSS only. No frameworks, no build tools.

---

## Folder Structure

```
SuttaNipata/
  index.html         <- intro page with vagga-grouped sutta cards (5 vaggas, 71 suttas)
  section1.html      <- Vagga 1, Sutta 1: Uraga
  ...
  section71.html     <- Vagga 5, Sutta 17: Piṅgiya
  css/
    style.css        <- all styles (copied from Dhammapada)
  docs/
    readme.md
    architecture.md  <- this file
    ai-context.md
    plan.md
    roadmap.md
    audit-config.json
    reference.py
  Backup/            <- dated backups
```

---

## Page Structure — Index

```
<portal-bar>           <- link back to DharmaGate
<header.site-header>   <- "Sutta Nipata" title, Chinese subtitle, tradition label
<section.intro>        <- brief description of the text
<main>
  <section.vagga-section> x5   <- one per vagga, each with:
    h2                          <- vagga name (Chinese + English)
    .chapter-grid               <- sutta cards for that vagga
      a.chapter-card            <- sutta number + Chinese name + English name
<footer>
```

---

## Page Structure — Section Pages

```
<portal-bar>                <- link back to DharmaGate
<header.section-header>     <- sutta name (Chinese + English), nav links
<main.section-container>
  section.full-text         <- full primary Chinese text + 🔊 聆听经文 button
  section.line-explanation
    h2                      <- "逐句解释"
    .explanation-card       <- one per verse/passage:
      p.line                <- primary Chinese text (bold)
      p.explanation-zh      <- Chinese explanation (always visible)
      button.toggle-btn     <- "English ▾"
      .detail-content       <- hidden by default:
        p.translation       <- Bhikkhu Bodhi English translation (red)
        p.explanation       <- English commentary (grey)
  section.summary
    h2                      <- "总结 · Summary"
    p.summary-zh            <- Chinese summary
    button.toggle-btn       <- "English ▾"
    .detail-content         <- hidden by default:
      p.explanation         <- English summary
<script>                    <- toggleDetail() + speak()
<footer>
```

---

## CSS Architecture

All styles in `css/style.css` — copied verbatim from Dhammapada. Same design tokens throughout.

---

## Chapter Grid (index.html)

Vagga-grouped layout. Five `<section class="vagga-section">` blocks, each with a vagga heading and a `.chapter-grid` of sutta cards. Each card shows:
- `.chapter-num` — sutta number
- `.chapter-zh` — Chinese sutta name
- `.chapter-en` — English sutta name

---

## Design Tokens

Same as all DharmaGate spokes.

| Token | Value | Usage |
|-------|-------|-------|
| `--red` | `#b83232` | Primary accent, translations |
| `--red-light` | `#d44e4e` | Hover states, headings |
| `--saffron` | `#c8820a` | Chapter number labels |
| `--saffron-lt` | `#e09c2a` | Portal bar links |
| `--ink` | `#1c0f0f` | Header/footer backgrounds |
| `--bg` | `#f7f0e6` | Page background |
| `--text` | `#2d1f1f` | Body text, Chinese explanations |
| `--muted` | `#7a6060` | English text, toggle buttons |
| `--border` | `#e0d0c8` | Card borders, dividers |

---

## Nav Pattern

- First sutta of vagga: prev links to last sutta of previous vagga (or none for section1)
- Last sutta of vagga: next links to first sutta of next vagga (or none for section71)
- Middle suttas: ← prev · 目录 Contents · next →

---

## Special note — Vagga 4 (T0198)

Section pages 39–54 use T0198 义足经 as the Chinese primary text. These pages include a source note in the full-text block attributing the text to Zhi Qian's 义足经. Pages for other vaggas use modern Chinese translation without a source note.

---

## Speech Synthesis

🔊 聆听经文 button reads all primary Chinese text for the sutta. Targets Ting-Ting voice (zh-CN, rate 0.9).

---

## External Dependencies

Google Fonts:
- Noto Serif SC — headings, Chinese primary text
- Noto Sans SC — body text, buttons

No other external dependencies.

---

## Hosting

GitHub Pages via `lugh3456` account.
Repository name: `SuttaNipata`
Live URL (when deployed): `https://lugh3456.github.io/SuttaNipata/`
