# GitHub Profile README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create a minimal, one-screen GitHub profile README that communicates dual identity (web/mobile + AI/ML) through a two-column layout.

**Architecture:** Single `README.md` file using markdown with `<img>` tags for shields.io badges. Two-column table structure with "Build" and "Think" columns. Flat-square muted badges at 24px height.

**Tech Stack:** Markdown, shields.io badges, HTML `<img>` tags

**Spec:** `docs/superpowers/specs/2026-03-19-github-profile-design.md`

---

### Task 1: Create README.md with header

**Files:**
- Create: `README.md`

- [ ] **Step 1: Create README.md with the header section**

```markdown
# Sanga Gerard

*I build things that work, then I teach machines to think.*
```

- [ ] **Step 2: Verify rendering**

Open `README.md` and confirm the H1 and italic tagline render correctly.

---

### Task 2: Add the duality table

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Add the two-column table with text rows**

Append below the tagline:

```markdown

| Build | Think |
|---|---|
| Java · Spring Boot | PyTorch · Transformers |
| PHP · Laravel | scikit-learn · NumPy |
| Python · Django · FastAPI | Reinforcement Learning |
| React Native · Flutter · Ionic | NLP · Embeddings · Attention |
```

- [ ] **Step 2: Verify table renders as two balanced columns**

---

### Task 3: Add icon badge rows to the table

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Add Build icons row**

Add a final row to the table. The Build cell contains these badges as `<img>` tags with `height="24"`:

```html
<img src="https://img.shields.io/badge/Java-555?style=flat-square&logo=openjdk&logoColor=white" height="24"> <img src="https://img.shields.io/badge/Python-555?style=flat-square&logo=python&logoColor=white" height="24"> <img src="https://img.shields.io/badge/PHP-555?style=flat-square&logo=php&logoColor=white" height="24"> <img src="https://img.shields.io/badge/React_Native-555?style=flat-square&logo=react&logoColor=white" height="24"> <img src="https://img.shields.io/badge/Flutter-555?style=flat-square&logo=flutter&logoColor=white" height="24">
```

- [ ] **Step 2: Add Think icons row**

The Think cell in the same row contains:

```html
<img src="https://img.shields.io/badge/PyTorch-555?style=flat-square&logo=pytorch&logoColor=white" height="24"> <img src="https://img.shields.io/badge/Python-555?style=flat-square&logo=python&logoColor=white" height="24"> <img src="https://img.shields.io/badge/scikit--learn-555?style=flat-square&logo=scikitlearn&logoColor=white" height="24"> <img src="https://img.shields.io/badge/NumPy-555?style=flat-square&logo=numpy&logoColor=white" height="24"> <img src="https://img.shields.io/badge/OpenAI-555?style=flat-square&logo=openai&logoColor=white" height="24">
```

- [ ] **Step 3: Verify badges render correctly with consistent spacing**

---

### Task 4: Add closing section

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Add horizontal rule and closing line**

Append below the table:

```markdown

---

*Less noise. More signal.*
```

- [ ] **Step 2: Final review — confirm entire README fits one screen and all elements render**

---

### Task 5: Initialize git and commit

**Files:**
- All files in repository

- [ ] **Step 1: Initialize git repository**

```bash
git init
```

- [ ] **Step 2: Commit the README**

```bash
git add README.md
git commit -m "feat: add minimal GitHub profile README"
```

- [ ] **Step 3: Commit the design docs**

```bash
git add docs/
git commit -m "docs: add design spec and implementation plan"
```
