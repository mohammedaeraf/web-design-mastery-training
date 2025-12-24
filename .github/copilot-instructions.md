# Copilot instructions — Web Design Mastery 🎯

Purpose: Short, actionable guidance to help an AI coding agent make safe, high-value changes in this teaching-focused static site repository.

## Quick repo snapshot

- Static teaching materials: demos/ (self-contained HTML examples), tutorials/ (how-to markdown), syllabus/ (course plan).
- No build system, package.json, or CI present — files are intended to be opened in a browser or served statically.

## Big picture (what matters)

- This repo demonstrates common header/hero/layout patterns using **Bootstrap 5** (CDN) and **AOS** for scroll animations. Example: `demos/academy-adv.html` and `tutorials/professional-header-hero.md`.
- Primary goal: readable, copy-pasteable examples for students. Keep edits minimal and pedagogical.

## Patterns & conventions to preserve 🔧

- Self-contained demo files: keep CSS in the `<head>` (small examples), keep necessary CDN links (Bootstrap, AOS) intact.
- Theme vars: demos use CSS variables like `--fla-primary`, `--fla-secondary`, `--fla-light` — reuse rather than hard-coding new color values.
- Header conventions: logo left, nav right, ≤6 items, CTA as `btn btn-primary` (see `tutorials/professional-header-hero.md`).
- Hero pattern: `<section class="hero">` + `.hero-bg` absolute background + `.hero-content` with z-index; animations via `data-aos` and `AOS.init({ duration: 900, once: true })`.
- Images: local assets live in `demos/img/`; prefer descriptive `alt` text and responsive sizes.

## How to preview & verify changes ✅

- Quick: Open `demos/*.html` directly in a browser for simple checks.
- Recommended (serves file URLs correctly):
  - Python: `python -m http.server 8000` (run from repo root) and open http://localhost:8000/demos/
  - Node: `npx serve .` or use VS Code Live Server extension.
- Manual checks: verify responsiveness with DevTools, confirm animations run, and check console for missing CDN or asset 404s.

## Making changes (practical rules) 📋

- Keep demos self-contained and minimal; do not introduce complex build tooling unless the change justifies it.
- When adding a new example:
  - Add `demos/<descriptive-name>.html` following existing naming and structure.
  - Add corresponding tutorial docs in `tutorials/` explaining the pattern and code snippets.
  - If a new course module is introduced, update `syllabus/syllabus.md` accordingly.
- PRs should be small and focused. Include at least one screenshot and a short description of behavior/learning objective.

## What NOT to do ❌

- Don’t remove or change CDN links (Bootstrap, AOS) to private forks or different major versions without a clear reason and a test plan.
- Don’t add heavy dependencies or a complex build pipeline without discussing rationale in the PR.

## Helpful files to inspect

- `demos/academy-adv.html` — canonical header + hero example (AOS usage, theme variables).
- `tutorials/professional-header-hero.md` — canonical teaching narrative and sample code.
- `syllabus/syllabus.md` — course structure and learning outcomes.

If anything here is unclear or you want a different level of detail (more code examples, stricter PR rules), tell me — I can iterate. ✅
