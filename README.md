# Evidentia

**From literature to traceable reasoning.** Evidentia is a literature reasoning workspace for researchers who need more than storage and summaries. It connects **claims**, **evidence**, **conditions** and **source context**, so the path from reading to writing stays visible.

**Live app:** https://OWNER.github.io/REPO/ (install it from the browser address bar to use it as an app)

## What you can do (V0.1)

- **Projects**: a research question, themes and open questions
- **Papers**: method, context, findings and limitations; BibTeX import
- **Claims**: link evidence as *support*, *qualify* or *tension*, with snippet and page/section
- **Claim Scope Check**: put the claim beside what the evidence actually covers, with prompts for over-broad wording. The researcher decides.
- **Synthesis**: an evidence map (claims × papers), plus consensus, tension, conditions and open questions
- **Outline**: arrange claims into sections and export Markdown with references
- **Research Memory**: before → after history of the question and claims, with the reason for each change

Seven interface languages: English, 中文, Español, 日本語, Français, Deutsch, 한국어.

## Principles

- Evidence first: important claims point back to source evidence.
- Human judgment: no automatic verdicts, quality scores or "research gap" claims.
- Local-first: projects stay in your browser and are never uploaded. Export or import JSON to move them between devices.
- Public, non-sensitive research material only.

## Tech

A single static `index.html` (vanilla JS, no build step), plus a web app manifest and a service worker for install and offline use. Hosted on GitHub Pages.

---

Working prototype · Student-led independent project · Not an official institutional website
