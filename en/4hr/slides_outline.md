# 🎓 Slide Outline — Agentic RAG Workshop (3 Days)

---

## 🎯 Slide 0: Workshop Overview (Translated English text Day 1 Translated English textcontent)

### Slide 0-1 — Title
- **Agentic RAG Workshop: From Zero to Hero**
- Translated English text AI Translated English text
- 3 Translated English text | Hands-on | Google Colab

### Slide 0-2 — Roadmap 3 Translated English text
- **Day 1: 📊 Data Engineering Pipeline**
  - Translated English text: Deduplicate → Chunk → Embed → VectorDB → Search
  - Tech: Qdrant, multilingual-e5-large, BM25, PyThaiNLP
  - 🔗 [Translated English text Colab](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day1/day1_data_engineering.ipynb)
- **Day 2: 🤖 Building Agents**
  - Translated English text AI Agent: Agent + Tools → RAG Agent → Multi-Agent
  - Tech: Google ADK, Gemini API, Session Memory
  - 🔗 [Translated English text Colab](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day2/day2_building_agents.ipynb)
- **Day 3: 📏 Evaluation & Optimization**
  - Translated English text: RAGAS, LLM-as-Judge, A/B Testing, Capstone
  - Tech: RAGAS Framework, Prompt Engineering
  - 🔗 [Translated English text Colab](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day3/day3_evaluation.ipynb)

### Slide 0-3 — Translated English textpoints
- **3 Translated English text × 3 Translated English text = 90 points**
- 🤝 **Responsibility (10/Day)** — Translated English text, Translated English text, Run ✅ Translated English text
- 💪 **Determination (10/Day)** — Translated English text, Translated English text parameter, Translated English text, debug
- 💻 **Technical (10/Day)** — Code Translated English text, Translated English text, Translated English text copy
- Translated English text:

  | Translated English text              |  Day 1  |  Day 2  |  Day 3  |   Translated English text   |
  | ---------------- | :-----: | :-----: | :-----: | :-----: |
  | 🤝 Responsibility |   /10   |   /10   |   /10   |   /30   |
  | 💪 Determination  |   /10   |   /10   |   /10   |   /30   |
  | 💻 Technical      |   /10   |   /10   |   /10   |   /30   |
  | **Translated English text**          | **/30** | **/30** | **/30** | **/90** |

### Slide 0-4 — Translated English text
- **Google Colab** — Translated English text code Translated English text cloud (Translated English text)
- **Gemini API** — LLM (2.5 Flash / 2.5 Pro)
- **Google ADK** — Translated English text AI Agent
- **Qdrant** — Vector Database
- Translated English text:
  - Google Account
  - Gemini API Key (Translated English text) → Translated English text Colab Secrets

### Slide 0-5 — Ground Rules
- 🔗 Notebook Translated English text link (Translated English text Colab Translated English text)
- 📤 Translated English texthomeworkTranslated English text Google Form (Download .ipynb → Upload)
- ⏰ Workshop: Translated English text → Translated English text → Translated English texthomework
- ❓ Translated English text → Translated English text!
- ⚠️ Translated English text API Key!

### Slide 0-6 — 📤 Translated English texthomework
- **Translated English text:** Download .ipynb Translated English text Colab → Upload Translated English text Google Form
- Translated English textcontent (Translated English text) + Translated English texthomework

| Day   | 🔗 Translated English texthomeworkTranslated English text Colab                                                                                                                  | 📤 Translated English texthomework (Google Form)                              |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------- |
| Day 1 | [day1_homework.ipynb](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day1/day1_homework.ipynb) | [Translated English texthomework Day 1](https://forms.gle/R7EXvPvUfZ286CVh8) |
| Day 2 | [day2_homework.ipynb](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day2/day2_homework.ipynb) | [Translated English texthomework Day 2](https://forms.gle/xTQ5eVNKa4fcQVKb8) |
| Day 3 | [day3_homework.ipynb](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day3/day3_homework.ipynb) | [Translated English texthomework Day 3](https://forms.gle/yLVHh4YVVt3miogm8) |

- ⚠️ Translated English text 1 Translated English text (Translated English text)
- ✅ Run "Translated English text" Translated English text!

---

## 📅 Day 1: Data Engineering Pipeline

### Slide 1 — Title
- **Agentic RAG Workshop: From Zero to Hero**
- Day 1: Data Engineering Pipeline

### Slide 2 — Workshop Overview
- 3 Translated English text?
  - Day 1: Data → VectorDB (Translated English text)
  - Day 2: Agent + Tools
  - Day 3: Evaluation + Capstone
- Translated English text Pipeline: Raw → Chunk → Embed → Store → Retrieve → Answer

### Slide 3 — RAG Translated English text?
- **R**etrieval-**A**ugmented **G**eneration
- LLM Translated English text → Translated English text "Translated English text" context Translated English text
- RAG = Translated English text + Translated English text
- Translated English text: LLM-only vs RAG

### Slide 4 — Setup
- 🔗 Translated English text Notebook: `[Translated English text Colab](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day1/day1_data_engineering.ipynb)`
- Translated English text API Key Translated English text Colab Secrets: `GOOGLE_API_KEY`
- ⚠️ Translated English text API Key!

### Slide 5 — Deduplication
- Translated English text?
- MD5/SHA256 Hash → fingerprint Translated English text
- 💡 Observation: Hash Translated English text = contentTranslated English text 100%

### Slide 6 — Chunking
- Translated English text? (LLM Translated English text context limit)
- 3 Translated English text:
  - Fixed-size: Translated English text
  - Recursive: Translated English text
  - Semantic: Translated English textcontent
- 💡 Observation: chunk_size vs overlap tradeoff

### Slide 7 — Thai Tokenization
- Thai languageTranslated English text
- PyThaiNLP `word_tokenize()`
- Translated English text: "Translated English text" → ["Translated English text","Translated English text"]

### Slide 8 — Embedding
- Translated English text → Vector (Translated English text)
- Model: `multilingual-e5-large` (Translated English text)
- Translated English text: Translated English text → Vector Translated English text
- Cosine Similarity: Translated English text

### Slide 9 — Hybrid Search
- Dense Search: Embedding (Translated English text)
- Sparse Search: BM25 (Translated English text)
- Hybrid = Dense + Sparse → Translated English text
- 💡 Observation: Dense Translated English text synonym, Sparse Translated English text keyword

### Slide 10 — Vector Database (Qdrant)
- Translated English text DB Translated English text? → Translated English text "Translated English text" Translated English text keyword
- Qdrant: in-memory, Translated English text, Translated English text
- Collection → Points (vector + payload)

### Slide 11 — Indexing & Retrieval
- Indexing: Chunk → Embed → Store Translated English text Qdrant
- Retrieval: Query → Embed → Search → Top-K results
- Translated English text: Full Pipeline Flow

### Slide 12 — 🧪 Translated English text
- Translated English text notebook Translated English text
- Translated English text chunk_size, top_k Translated English text
- 15 Translated English text

### Slide 13 — Translated English text Day 1
- Translated English text: Dedup → Chunk → Embed → VectorDB → Search
- 💡 Key Takeaways:
  - Chunk size Translated English text RAG
  - Hybrid Search Translated English text
  - Embedding model Translated English textThai language

### Slide 14 — homework Day 1
- 🔗 Translated English texthomework: `[Translated English text Colab](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day1/day1_homework.ipynb)`
- 📤 Translated English texthomework: [Google Form Day 1](https://forms.gle/R7EXvPvUfZ286CVh8)
- Translated English text Pipeline Translated English text (10 points)
- Download .ipynb → Upload Translated English text Form
- Deadline: [Translated English text]

---

## 📅 Day 2: Building Agents with Google ADK

### Slide 1 — Title
- **Agentic RAG Workshop: From Zero to Hero**
- Day 2: Building Agents with Google ADK

### Slide 2 — Translated English text Day 1 + Setup
- Pipeline: Raw → Chunk → Embed → VectorDB → Search
- Translated English text: Translated English text "Agent" Translated English text
- 🔗 Translated English text Notebook: `[Translated English text Colab](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day2/day2_building_agents.ipynb)`

### Slide 3 — Agent vs Chatbot
- Chatbot: Translated English text-Translated English text script
- Agent: Translated English text → Translated English text → Translated English text → Translated English text
- Translated English text: Input → Think → Act → Observe → Answer

### Slide 4 — Google ADK
- Agent Development Kit
- Translated English text Agent Translated English text Python Translated English text
- Components: Agent + Instruction + Tools + Model

### Slide 5 — Agent Translated English text
- `LlmAgent(name, model, instruction)`
- Instruction = "Translated English text" Translated English text Agent
- Translated English text Agent

### Slide 6 — Tools (Function Tools)
- Agent Translated English text Tools
- `FunctionTool`: Translated English text Python function → Agent Translated English text
- Translated English text: Translated English text, Translated English text, Translated English text
- 💡 Observation: docstring Translated English text! Agent Translated English text docstring Translated English text

### Slide 7 — Gemini API Parameters
- `temperature`: Translated English text creative (0=Translated English text, 1=Translated English text)
- `top_k`, `top_p`: Translated English text
- `max_output_tokens`: Translated English text

### Slide 8 — RAG Agent
- Translated English text Agent + VectorDB Translated English text Day 1
- Tool: `search_knowledge(query)` → Translated English text Qdrant
- Agent Translated English text: Translated English text

### Slide 9 — Multi-Agent Systems
- Agent Translated English text? → Translated English text Agent Translated English text
- 4 patterns:
  - Sequential: Translated English text A → B → C
  - Parallel: Translated English text A + B + C
  - Loop: Translated English text
  - LLM Routing: AI Translated English text Agent Translated English text

### Slide 10 — Sequential vs Parallel
- Sequential: Translated English text (Translated English text → Translated English text → Translated English text)
- Parallel: Translated English text (Translated English text 3 Translated English text)
- Translated English text

### Slide 11 — Session Memory
- Agent Translated English text
- `InMemorySessionService`
- Translated English text: Translated English text Agent Translated English text context

### Slide 12 — Agentic RAG
- Translated English text: RAG + Multi-Agent + Memory
- Translated English text: Study Assistant Translated English text + Translated English text + Translated English text
- 💡 Observation: Translated English text RAG Translated English text = Agent Translated English text

### Slide 13 — 🧪 Translated English text
- Translated English text Agent + Custom Tool Translated English text
- 15 Translated English text

### Slide 14 — Translated English text Day 2
- Agent = AI Translated English text + Translated English text
- Multi-Agent = Translated English text Agent Translated English text
- Agentic RAG = Agent + RAG + Memory

### Slide 15 — homework Day 2
- 🔗 Translated English texthomework: `[Translated English text Colab](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day2/day2_homework.ipynb)`
- 📤 Translated English texthomework: [Google Form Day 2](https://forms.gle/xTQ5eVNKa4fcQVKb8)
- Translated English text 4 Translated English text: Agent+Tool, RAG Agent, Workflow, Translated English text
- Download .ipynb → Upload Translated English text Form
- 10 points | Deadline: [Translated English text]

---

## 📅 Day 3: Evaluation & Optimization

### Slide 1 — Title
- **Agentic RAG Workshop: From Zero to Hero**
- Day 3: Evaluation & Optimization

### Slide 2 — Translated English text Day 1-2 + Setup
- Day 1: Data → VectorDB → Search
- Day 2: Agent → RAG Agent → Multi-Agent
- Day 3: "Translated English text?"
- 🔗 Translated English text Notebook: `[Translated English text Colab](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day3/day3_evaluation.ipynb)`

### Slide 3 — Translated English text?
- "Translated English text" ≠ "Translated English text"
- Translated English text: Hallucination, Translated English text, Translated English text
- Translated English text → Translated English text

### Slide 4 — RAGAS Metrics
- **Faithfulness**: Translated English text context Translated English text?
- **Answer Relevancy**: Translated English text?
- **Context Precision**: context Translated English text?
- **Context Recall**: Translated English text context Translated English text?
- Translated English text: 4 metrics quadrant

### Slide 5 — Auto Eval Dataset
- Translated English text Gemini
- Input: Translated English text → Output: Translated English text + Translated English text + context
- Translated English text → Translated English text

### Slide 6 — LLM-as-Judge
- Translated English text LLM Translated English text LLM
- Prompt: "Translated English textpoints 1-5 Translated English text..."
- Translated English text: Translated English text rule Translated English text
- Translated English text: Translated English text bias, Translated English text prompt Translated English text

### Slide 7 — Agent Testing
- Tool Selection Accuracy: Agent Translated English text tool Translated English text?
- Response Quality: Translated English text?
- Test Cases: ≥ 5 Translated English text → Translated English text pass rate

### Slide 8 — A/B Testing
- Translated English text 2 configs:
  - A: chunk_size=200, top_k=3
  - B: chunk_size=500, top_k=5
- Translated English text → Translated English text
- 💡 Observation: Translated English text

### Slide 9 — Prompt Engineering
- Before vs After
- Translated English text: Role, Few-shot, Chain-of-Thought, Constraints
- Translated English text: prompt Translated English text → pointsTranslated English text

### Slide 10 — Optimization Strategies
- 5 Translated English text:
  1. Chunk size / overlap
  2. Embedding model
  3. Top-K / Search method
  4. Prompt template
  5. Model parameters (temperature)
- Translated English text!

### Slide 11 — 🧪 Translated English text
- Translated English text pipeline → Translated English text Before/After
- 15 Translated English text

### Slide 12 — ⭐ Capstone Project
- Translated English text: Data + Agent + Evaluation
- Translated English text RAG Agent Translated English text
- Translated English text: points, Translated English text, Before/After

### Slide 13 — Translated English text 3 Translated English text
- Day 1: 📊 Data Engineering → Translated English text
- Day 2: 🤖 Agent Building → AI Translated English text
- Day 3: 📏 Evaluation → Translated English text
- Translated English text: Full Pipeline Translated English text

### Slide 14 — What's Next?
- Production: Deploy Translated English text Cloud Run / Vertex AI
- Advanced: Fine-tuning, Knowledge Graph, Hybrid Agent
- Community: Translated English text Issue, Translated English text PR Translated English text!

### Slide 15 — homework Day 3 + Translated English text Final
- 🔗 Translated English texthomework: `[Translated English text Colab](https://colab.research.google.com/github/megacare-dev/agentic_rag_workshop/blob/main/day3/day3_homework.ipynb)`
- 📤 Translated English texthomework: [Google Form Day 3](https://forms.gle/yLVHh4YVVt3miogm8)
- homework 10 points | Download .ipynb → Upload Translated English text Form
- Deadline: [Translated English text]
- Translated English text 3 Translated English text × 3 Translated English text = 90 points:
  - 🤝 Responsibility (30)
  - 💪 Determination (30)
  - 💻 Technical (30)

### Slide 16 — Thank You
- _"The best way to learn AI is to build with AI."_
