# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

This repository contains course materials for **Metasains dalam Psikologi** — a 14-week course on metascience for psychology students at Universitas Airlangga, taught by Rizqy Amelia Zein.

## Context

- Owner: Rizqy Amelia Zein (`amelia.zein@psikologi.unair.ac.id`)
- Language of instruction: **Bahasa Indonesia** (confirmed)
- Audience: mixed S1/S2 psychology students with basic research methods background (NHST, experimental/survey design, effect sizes, reliability)
- This is a content/curriculum project, not a software project

## Project Structure

- `index.qmd` — course outline (the main landing page); do not revert to old statistics content
- `slides/bagian-N.qmd` — slide decks for each bagian, using the `unair-revealjs` format
- `references/` — PDF copies of all assigned readings
- `_quarto.yml` — Quarto website config (output to `docs/`, theme: cosmo/darkly)
- `_extensions/` — Quarto extensions (fontawesome, iconify, unair theme)

## Course Structure

The course has **10 Bagian** across 14 weeks (some bagian span 2 weeks). Use "Bagian" (not "Modul") consistently:

| Bagian | Minggu | Tema |
|--------|--------|------|
| 1 | 1–2 | Apa itu Metasains? |
| 2 | 3–4 | Krisis Replikasi |
| 3 | 5–6 | Praktik Penelitian Bermasalah (QRP) |
| 4 | 7 | Ancaman Sistemis terhadap Sains yang Dapat Direproduksi |
| 5 | 8 | Masalah Pengukuran dan Teori |
| 6 | 9 | Struktur Insentif dan *Publish or Perish* |
| 7 | 10–11 | Sains Terbuka dan Reformasi |
| 8 | 12 | Sains Kolaboratif dan Proyek Many Labs |
| 9 | 13 | Metasains Kritis |
| 10 | 14 | Sintesis dan Masa Depan Metasains |

## Working Conventions

- All written content in **Bahasa Indonesia**
- For slides, use the `unair-revealjs` format (see `slides/bagian-1.qmd` as template)
- For formatted documents, use the `/docx` skill; for PDFs, use the `/pdf` skill
- Slide files follow the naming convention `slides/bagian-N.qmd` and are rendered to `slides/bagian-N.html`
- When adding new bagian to the site, register them in `_quarto.yml` under both `render:` and `website.navbar`
- References go in `references/` as PDFs

## Known Reference Notes

- The file `references/chambers2014.pdf` is **Ioannidis (2014)** (*Addiction*, 110, 9–13), not a Chambers paper — it was misnamed. The correct citation is: Ioannidis, J. P. A. (2014). Why journals must review manuscripts before results are known. DOI: 10.1111/add.12438
- `references/meehl2004.pdf` is a 2004 reprint of Meehl (1978) in *Applied & Preventive Psychology, 11*(1), 1–22. DOI: 10.1016/j.appsy.2004.02.001

## Scope Boundaries

- Course is for **psychology students only** — do not broaden examples to other sciences
- **Do not add psychology of science** as a content area; it is a distinct field and is only mentioned in passing in LO #1 as a contrast to metascience
