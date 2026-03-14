# 📝 Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/).

---

## [1.1.3] - 2026-03-13

### 🐛 Fixed

**Day 2: Building Agents**
- `day2_homework.ipynb` — `chat_with_agent()` Translated English text `session_service` Translated English text constructor arg Translated English text `InMemoryRunner` Translated English text → Translated English text `runner.session_service` pattern (#46)

**Day 3: Evaluation**
- `day3_evaluation.ipynb` — RAGAS evaluation cell Translated English text (embedding setup, Dataset, evaluate() call, try block) Translated English text parse error (#45)

---

## [1.1.2] - 2026-03-07

### 🐛 Fixed

- Heatmap Thai languageTranslated English text □□□ — Translated English text Thai font setup (Garuda) Translated English text heatmap cell (#41)

---

## [1.1.1] - 2026-03-07

### 🐛 Fixed

- GitHub Translated English text render `day1_data_engineering.ipynb` — `metadata.widgets` Translated English text `state` key (#39)

---

## [1.1.0] - 2026-03-06

### 🎉 All Notebooks Error-Free on Colab

Notebooks Translated English text 3 Translated English text + Translated English text Google Colab Translated English text error

### 🐛 Fixed

**Day 1: Data Engineering**
- Thai font Translated English text matplotlib Translated English text □□□ — Translated English text `fonts-thai-tlwg` + `addfont()` (#19, #23, #28)
- Similarity matrix text Translated English text — Translated English text matplotlib heatmap (#30, #32)

**Day 2: Building Agents**
- `InMemoryRunner` Translated English text `session_service` param — Translated English text `runner.session_service` (#16)
- `resp.text.strip()` → NoneType error — Translated English text None check (#17)
- `chat_with_agent` tuple unpacking ValueError — Translated English text return value (#16)
- `%%time` + `await` SyntaxError Translated English text Colab — Translated English text `%%time`

**Day 3: Evaluation**
- `InMemoryRunner` + `session_service` TypeError — Translated English text `runner.session_service` (#26)
- `resp.text.strip()` NoneType — Translated English text None check (#26)

### ✨ Improved

- ASCII diagrams Translated English text Thai text → Translated English text markdown table Translated English text notebook (#21)
- Pipeline diagram Day 1 + Day 2 → Translated English text
- Similarity matrix → heatmap visualization 3 Translated English text (#30)
- Translated English text KMITL Translated English text sample data Translated English text

### 📝 Documentation

- README: Translated English text Known Issues & Fixes section (#33)
- README: Translated English text + Colab note
- Translated English text `.agent/workflows/git-workflow.md` — Translated English text Issue → Branch → PR → Merge

---

## [1.0.0] - 2026-03-06

### 🎉 Initial Release

Workshop Translated English text Agentic RAG Translated English text 3 Translated English texthomeworkTranslated English text

### ✨ Added

**Workshop Notebooks**
- `day1/day1_data_engineering.ipynb` — Dedup, Chunk, Embed, Hybrid Search, Qdrant, Retrieval
- `day2/day2_building_agents.ipynb` — Agent, Tools, RAG Agent, Multi-Agent (Google ADK)
- `day3/day3_evaluation.ipynb` — RAGAS, LLM-as-Judge, A/B Testing, Capstone

**Homework Notebooks**
- `day1/day1_homework.ipynb` — Pipeline Translated English text loop (10 points)
- `day2/day2_homework.ipynb` — Agent + RAG Agent + Workflow (10 points)
- `day3/day3_homework.ipynb` — RAG + Evaluation + Optimization (10 points)
- Anti-cheat: student-specific seeded data generation
- Standardized student info: Translated English text, Translated English text, Translated English text, LINE ID

**Grading System**
- `day1/day1_grading.ipynb` — AI grading Translated English text Gemini 2.5 Pro
- `day2/day2_grading.ipynb` — Duplicate check + CSV/JSON export
- `day3/day3_grading.ipynb` — Automated scoring + download
- `final_grading.ipynb` — 3 Translated English text (Responsibility/Determination/Technical) × 3 Translated English text = /90

**Submission System**
- Google Form × 3 Translated English text (Workshop notebook + Homework notebook upload)
- Google Drive folder structure

**Documentation**
- `README.md` — Translated English text, Translated English text, Translated English text, Translated English textpoints, Tech Stack
- `LICENSE` — CC BY-NC-SA 4.0 (TH + EN)
- `slides_outline.md` — Slide outline 50 slides Translated English text Colab + Form links

### 🐛 Fixed
- numpy binary incompatibility on Colab (#1, #2)
- Docling ONNX model file not found (#3, #4, #5)
- typer version conflict with docling
- Cell ordering in Day 1 Section 1.7-1.9 (#6, #7)
