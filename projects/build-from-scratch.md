# 15 Projects to Build From Scratch

Each project has a clear goal, a reason it matters, milestones so you can finish it, and a write-up idea. Every one ends in something people can **use**, and that is what makes a project worth showing.

**Rules for every project here:**
- Public GitHub repo from day 1, with a README following [../05-document-and-blog.md](../05-document-and-blog.md)
- A live demo, a `pip install`, or a downloadable release
- At least one blog post when you reach v1

---

## 🟢 Beginner

### 1. Evidence-Based Health Tips Site (open-source, community-driven)
- **What:** A static website of health tips where *every* tip must cite a peer-reviewed source or an official guideline (WHO, NHS, CDC). Anyone can add tips by pull request.
- **Why it matters:** Fights health misinformation. You also become a **maintainer**: you review PRs, write the contributing guide and label good first issues.
- **Stack:** Astro or Hugo + Markdown, GitHub Pages, GitHub Actions to check that every tip has a source link.
- **Milestones:**
  1. 20 tips across 4 categories (sleep, nutrition, exercise, mental health), each with a source
  2. Search + tag filtering
  3. CI check that rejects tips without citations
  4. `CONTRIBUTING.md` + 10 `good first issue`s; get 5 outside contributors
- **Stretch:** Translations into other languages; a "myth vs fact" section.
- **Blog post:** "How I built and ran my first open-source community project."

### 2. Personal Habit & Wellness Tracker (privacy-first)
- **What:** Track water, sleep, steps and mood. All data stays on the device.
- **Why it matters:** Teaches full product thinking: UX, data modeling, offline storage and charts.
- **Stack:** React Native / Flutter, or a PWA with IndexedDB; Chart.js or Recharts.
- **Milestones:** log entries → streaks & reminders → weekly insights dashboard → export to CSV.
- **Blog post:** "Designing a privacy-first health app."

### 3. CLI Productivity Tool, Published to PyPI
- **What:** A command-line tool that automates something you do often (organize downloads, rename lecture files, summarize git activity, Pomodoro timer with stats).
- **Why it matters:** You learn packaging, versioning, testing and CI, the full life of a library.
- **Stack:** Python + Typer/Click, pytest, GitHub Actions, PyPI.
- **Milestones:** working script → package with `pyproject.toml` → tests + CI → published v1.0 → 10 users.
- **Blog post:** "From script to PyPI package in a weekend."

### 4. Campus Utility App
- **What:** Something your university is missing: a book exchange, lost and found, a study-room finder, or a course-review board.
- **Why it matters:** Real users close by give you fast feedback, and it shows impact you can measure.
- **Stack:** Next.js + Supabase/Firebase, deployed on Vercel.
- **Milestones:** MVP for one dorm or club → auth + moderation → 100 users → hand over to a student club so it keeps running.

### 5. Data Story From Your Own Data
- **What:** Export your own data (wearable, Spotify, screen time, Google Takeout) and build an interactive analysis.
- **Why it matters:** You practice data cleaning, visualization and storytelling, which every field needs.
- **Stack:** Python, pandas, Plotly/Altair, Quarto or Streamlit.
- **Blog post:** "What a year of my sleep data taught me."

---

## 🟡 Intermediate

### 6. Food Label / Nutrition Explainer
- **What:** Scan a barcode or a photo of an ingredients label. The app explains the nutrition in plain language and flags allergens.
- **Why it matters:** Combines OCR or computer vision, an open API, and a useful health product. You can contribute fixes back to Open Food Facts.
- **Stack:** Open Food Facts API, Tesseract/PaddleOCR or a vision model, FastAPI, mobile or web frontend.
- **Milestones:** barcode lookup → OCR for unknown products → allergen and diet flags → submit missing products back to Open Food Facts.

### 7. RAG Assistant With Real Evaluation
- **What:** A chatbot that answers questions over a document set (course handbook, university policies, medical guidelines) and **cites its sources**.
- **Why it matters:** RAG is everywhere. What makes yours stand out is **evaluation**: a test set of question–answer pairs and measured accuracy.
- **Stack:** an open embedding model, a vector DB (FAISS, Chroma or pgvector), an open or API LLM, Gradio UI, an eval set of 100+ questions.
- **Milestones:** naive RAG → citations → eval harness → compare 3 chunking/retrieval strategies with numbers → deploy on HF Spaces.
- **Blog post:** "I measured my RAG system. Here's what actually helped."

### 8. Fine-Tune a Small Model for a Low-Resource Task
- **What:** Fine-tune a small open LLM or speech model (LoRA) for an under-served language, dialect or niche domain.
- **Why it matters:** This is real ML engineering, and the result is useful to a community. Publish the model and dataset on Hugging Face.
- **Stack:** Transformers, PEFT, datasets, Weights & Biases, HF Hub.
- **Milestones:** collect/clean data → baseline → LoRA fine-tune → evaluate against the baseline → model card + dataset card → demo Space.

### 9. Posture & Break Coach (on-device vision)
- **What:** A desktop app that uses the webcam with an on-device pose model to remind you to fix your posture and take breaks. No video leaves the machine.
- **Why it matters:** Covers real-time ML, privacy, and desktop app packaging.
- **Stack:** MediaPipe or a small pose model, Python + PyQt or Electron, ONNX Runtime.

### 10. A Reusable GitHub Action or VS Code Extension
- **What:** A dev tool other developers install, such as a docs link checker, a README badge generator or a "good first issue" labeler bot.
- **Why it matters:** Your users are developers, so you get real feedback through issues and stars.
- **Milestones:** working action → published on the Marketplace → used by 10 repos.

---

## 🔴 Advanced

### 11. Build a Deep Learning Framework From Scratch
- **What:** Write autograd, tensors, layers and an optimizer, then train a small CNN or transformer with **your own** framework.
- **Why it matters:** Nothing teaches ML internals better. A well-explained version is a strong portfolio piece.
- **Reference to learn from:** [karpathy/micrograd](https://github.com/karpathy/micrograd), [tinygrad](https://github.com/tinygrad/tinygrad).
- **Milestones:** scalar autograd → tensor autograd (NumPy) → MLP on MNIST → CNN → optional GPU support (CuPy or Triton).
- **Blog post:** a series, one post per milestone.

### 12. Train a Small GPT From Scratch
- **What:** Implement and train a small transformer language model on a dataset you choose (e.g., text in your language), then study how it behaves.
- **Reference:** [karpathy/nanoGPT](https://github.com/karpathy/nanoGPT).
- **Milestones:** tokenizer → model → training loop → evaluation → ablations (model size, data size, context length) with plots.

### 13. LLM Inference Optimizer
- **What:** Take a small model and make it faster: quantization, KV cache, batching, speculative decoding. Benchmark every step.
- **Why it matters:** Inference efficiency is one of the most valuable ML skills right now.
- **Stack:** PyTorch, llama.cpp/GGUF, ONNX, profiling tools.

### 14. Federated / Privacy-Preserving Health Model
- **What:** Simulate several "hospitals" and train a model on a public medical dataset without sharing raw data. Compare the result with centralized training.
- **Why it matters:** Federated learning and privacy are active research areas with direct impact on healthcare.
- **Stack:** Flower (`flwr`), PyTorch, a public dataset (e.g., MedMNIST).
- **Can become:** a workshop paper.

### 15. Distributed Key-Value Store / Mini Database
- **What:** Implement a key-value store with Raft consensus, or a tiny SQL database with a B-tree storage engine.
- **Why it matters:** The classic systems project. It shows deep understanding of the fundamentals.
- **Reference:** the MIT 6.5840 (Distributed Systems) labs, and "Build Your Own X" style tutorials.

---

## Choosing the right one

| You want… | Pick |
|-----------|------|
| To become a maintainer of a community | #1 |
| Your first shipped product | #2, #3, #4 |
| ML portfolio for internships | #7, #8, #11 |
| Research / grad school | #12, #14 (+ see [research-projects.md](research-projects.md)) |
| Systems / backend roles | #3, #10, #15 |
| Health + tech impact | #1, #2, #6, #9, #14 |

Plan your chosen project with [project-template.md](project-template.md).
