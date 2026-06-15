# The Pedagogical Revolution — NotebookLM Field Guide

> **100 Strategic Use Cases for NotebookLM in Modern Education**  
> Faculty Excellence · Student Mastery · Strategic AI Integration

A bilingual (EN/ES), interactive, single-file HTML report designed for higher education faculty and students. It documents 100 research-backed use cases for Google NotebookLM, organized by audience and pedagogical purpose, each with a verified MLA 9 source, a feature mapping, and a copy-ready adaptable prompt.

---

## Live Preview

Open `index.html` directly in any modern browser — no server, build step, or dependencies required.

---

## Features

| Feature | Details |
|---|---|
| **100 Use Cases** | 50 Faculty + 50 Student, divided into thematic groups |
| **EN / ES Toggle** | Full bilingual interface; preference saved to `localStorage` |
| **Adaptable Prompts** | One Courier New prompt per use case with `[BRACKETS]` for topic substitution |
| **Copy Button** | One-click clipboard copy for every prompt |
| **MLA 9 Citations** | 17 verified peer-reviewed sources assigned to items by pedagogical relevance |
| **Strategic Matrix** | 10-tool integration table (Gamma, Canva, Anki, PowerPoint, Moodle, etc.) |
| **Save / Print PDF** | Print-safe CSS — cards never split across pages |
| **Author Photo** | Embedded base64 headshot in hero and footer |
| **Sticky Nav** | Language toggle and print button always accessible |
| **Back to Top** | Floating button appears after scrolling |
| **Accessible** | Keyboard-navigable toggles, `aria-expanded`, `aria-pressed`, `focus-visible` outlines, `prefers-reduced-motion` respected |

---

## File Structure

```
├── index.html        # Entire application — self-contained, no external dependencies
└── README.md
```

All CSS, JavaScript, content, and the author photo (base64-encoded) live inside `index.html`. Zero npm packages, zero build tools, zero frameworks.

---

## Use Case Sections

### Section I — Faculty (items 1–50)
| Group | Items |
|---|---|
| Curriculum Design & Content Generation | 1–15 |
| Assessment & Feedback | 16–28 |
| Research & Scholarship | 29–40 |
| Operational Efficiency & Communication | 41–50 |

### Section II — Student (items 51–100)
| Group | Items |
|---|---|
| Comprehension & Clarification | 51–63 |
| Active Study & Retrieval Practice | 64–76 |
| Synthesis & Critical Thinking | 77–89 |
| Personalization, Accessibility & Project Work | 90–100 |

---

## Sources (MLA 9)

17 verified, peer-reviewed sources — each assigned to one or more use cases by thematic relevance:

| Short Label | Full Reference |
|---|---|
| Anderson & Krathwohl 2001 | *A Taxonomy for Learning, Teaching, and Assessing* |
| Ayala & Bechard 2024 | "Reducing Hallucination … via RAG." *NAACL 2024* |
| Belkina et al. 2025 | "Implementing GenAI in Higher Education." *Computers and Education: AI* |
| Bisra et al. 2018 | "Inducing Self-Explanation: A Meta-Analysis." *Educational Psychology Review* |
| CAST 2024 | *UDL Guidelines, Version 3.0* |
| Cepeda et al. 2006 | "Distributed Practice … A Quantitative Synthesis." *Psychological Bulletin* |
| Chi & Wylie 2014 | "The ICAP Framework." *Educational Psychologist* |
| Dunlosky et al. 2013 | "Improving Students' Learning …" *Psychological Science in the Public Interest* |
| Li et al. 2025 | "RAG for Educational Application: A Systematic Survey." *Computers and Education: AI* |
| Mayer 2021 | *Multimedia Learning*, 3rd ed. |
| Nikolic et al. 2023 | "ChatGPT versus Engineering Education Assessment." *European Journal of Engineering Education* |
| Nikolic et al. 2024a | "ChatGPT, Copilot, Gemini, SciSpace and Wolfram …" *Australasian Journal of Engineering Education* |
| Nikolic et al. 2024b | "A Systematic Literature Review … UTAUT Framework." *Australasian Journal of Educational Technology* |
| Roediger & Karpicke 2006 | "Test-Enhanced Learning." *Psychological Science* |
| Rohrer & Taylor 2007 | "The Shuffling of Mathematics Problems …" *Instructional Science* |
| Wiggins & McTighe 2005 | *Understanding by Design*, 2nd ed. |
| Yee et al. 2023 | *ChatGPT Assignments to Use in Your Classroom Today*. UCF OER / STARS |

---

## NotebookLM Features Covered

- Source Grounding (PDF, Docs, Slides, web, YouTube, audio, images, CSV)
- Inline Citations & Excerpts
- Chat (Q&A, comparison, transformation)
- Studio: Audio Overviews, Video Overviews, Mind Maps, Slide Decks (PPTX export), Infographics, Flashcards, Quizzes, Reports, Data Tables
- Saved Notes
- Shared / Public Notebooks

---

## Printing to PDF

1. Click **Save / Print PDF** in the top bar (or `Ctrl/Cmd + P`).
2. Choose **Save as PDF** as the destination.
3. Recommended settings: **Letter**, margins **Default** or **None**, **Background graphics ON**.

Cards, tables, and section headings are protected from mid-page splits via `break-inside: avoid`.

---

## Customization

| What | Where in `index.html` |
|---|---|
| Author name / photo | Search `PHOTO` (base64 `<img>`) and `.photo-info` block in the hero |
| Color palette | `:root` CSS variables at the top of `<style>` |
| Use case content | `data.js`-equivalent objects embedded in the build script (see comments) |
| Spanish translations | `es.js`-equivalent objects in the same section |
| Source list | `SOURCES` object near the top of the `<script>` block |

---

## Browser Compatibility

| Browser | Support |
|---|---|
| Chrome / Edge 90+ | ✅ Full |
| Firefox 90+ | ✅ Full |
| Safari 15+ | ✅ Full |
| Mobile (iOS / Android) | ✅ Responsive |

Clipboard API (`navigator.clipboard`) requires HTTPS or `localhost`; a `document.execCommand('copy')` fallback is included for file:// contexts.

---

## Academic Context

Prepared by **Dr. Victor Garcia-Martinez, MSN, FNP-C, RN**  
Nursing & Biology Faculty — Lone Star College–North Harris  
June 2026

This report was developed as part of a faculty professional development initiative on the responsible integration of source-grounded AI tools in higher education. All 17 cited sources were independently verified prior to inclusion.

---

## License

Content © 2026 Victor Garcia-Martinez. All rights reserved.  
Cited works remain the intellectual property of their respective authors and publishers.  
The source code structure of `index.html` may be reused for non-commercial educational purposes with attribution.
