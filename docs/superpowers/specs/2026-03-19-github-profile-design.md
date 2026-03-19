# GitHub Profile README — Design Spec

## Overview

A minimal, one-screen GitHub profile README for `sangagerard` that communicates dual identity (web/mobile engineering + AI/ML) through structure rather than explanation. Follows the principle: "simplicity is the ultimate sophistication."

## Target Feeling

When someone lands on the profile, they should think: *"This person gets it."*

## Structure

### 1. Header

```markdown
# Sanga Gerard

*I build things that work, then I teach machines to think.*
```

- Name as an H1
- Single italic tagline beneath — no job title, no labels

### 2. Duality Table

A two-column markdown table with headers **Build** and **Think**.

**Build column** (Web & Mobile):
- Java · Spring Boot
- PHP · Laravel
- Python · Django · FastAPI
- React Native · Flutter · Ionic

**Think column** (ML & AI):
- PyTorch · Transformers
- scikit-learn · NumPy
- Reinforcement Learning
- NLP · Embeddings · Attention

Each column gets a dedicated final row containing only skill icons. Icons use shields.io badges with `?style=flat-square&logo=<name>&logoColor=white&color=555` format, rendered as `<img>` tags with `height="24"`. Select ~4-5 icons per column for visual symmetry.

Example badge URL:
```
https://img.shields.io/badge/Java-555?style=flat-square&logo=openjdk&logoColor=white
```

**Build icons (5):** Java, Python, PHP, React, Flutter
**Think icons (5):** PyTorch, Python, scikit-learn, NumPy, OpenAI

Note: Python appears in both — that's intentional and honest. OpenAI appears as an icon because it represents the platform/ecosystem the user works within, even though it's not listed as a framework in the text.

### 3. Closing

```markdown
---

*Less noise. More signal.*
```

A horizontal rule followed by a single italic line.

## Intentional Omissions

- No GitHub stats widgets
- No contribution graphs
- No "About Me" paragraph
- No social links section
- No "currently learning" / "fun fact" / "pronouns" boilerplate
- No emoji

## Constraints

- Must fit on one screen without scrolling (desktop viewport)
- Markdown only — no HTML except `<img>` tags for icons
- Icons must be flat/muted style, not colorful badges
- Every word must earn its place

## File

Single file: `README.md` at repository root.
