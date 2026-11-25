# 03 — Side Projects: Join One or Start Your Own

## Join a group vs. start your own

| Join an existing group | Start your own |
|------------------------|----------------|
| Learn from more experienced people | You own the vision and decisions |
| Faster to get going | Teaches product thinking, scoping, leadership |
| Lower risk of abandonment | Higher risk — needs discipline |
| Good first step | Great second step, or do both |

Ideally: contribute to someone else's project **and** have one project of your own.

## Where to find people to build with

- University clubs: ACM/IEEE chapters, AI/robotics clubs, Google Developer Student Clubs, entrepreneurship clubs
- Hackathons (MLH events, university hackathons, Kaggle/Devpost challenges) — the best place to find teammates fast
- Discord/Slack communities of tools you use
- Classmates from courses with good projects — propose continuing a course project after the semester
- Twitter/X, LinkedIn, Bluesky, Reddit (r/learnprogramming, r/MachineLearning, r/SideProject)
- Kaggle competitions — team up with people on the forums

## Starting from scratch: a process

### 1. Find a real problem
The best projects solve a problem **you** have. Ask:
- What do I do repeatedly that's annoying?
- What tool do I wish existed?
- What data do I find interesting that nobody has analyzed well?

### 2. Scope it down (the MVP)
Write one sentence: *"A [tool] that lets [who] do [what] in [constraint]."*
Then cut features until you could build v0.1 in **2–4 weekends**.

### 3. Plan in public
- Create the GitHub repo on day 1 with a README describing the goal.
- Use GitHub Issues / Projects as your to-do list.
- Write a short `ROADMAP.md`.

### 4. Build, ship, iterate
- Ship v0.1 even if it's ugly. Get one real user (a friend counts).
- Deploy it: Vercel/Netlify (web), Hugging Face Spaces / Streamlit / Gradio (ML demos), PyPI (libraries), GitHub Releases (CLIs).
- Collect feedback → next version.

### 5. Document and share
See [05-document-and-blog.md](05-document-and-blog.md). A project that isn't documented and shared barely exists.

## Idea bank

Pick one, remix it, or let it spark your own. Each has a beginner → advanced range.

### AI / ML
- **Paper reproduction series:** reproduce one classic paper per month; publish code + blog post.
- **Domain-specific RAG assistant:** chatbot over your university's course catalog / policies, with citations and an evaluation set.
- **Small-model fine-tuning:** fine-tune a small open LLM for a low-resource language or niche task; publish to Hugging Face with a proper model card.
- **Evaluation benchmark:** build a dataset + benchmark for something models are bad at; contribute it to an evaluation harness.
- **On-device ML app:** run a vision/speech model fully offline on a phone or Raspberry Pi.
- **Interpretability toy:** visualize what neurons/attention heads do in a small transformer.

### Health & wellbeing *(matches this folder's "healthy tips" theme)*
- **Healthy-habit tracker** with streaks, reminders and a privacy-first local data store.
- **Food-label scanner** using open data (e.g., Open Food Facts API) to explain nutrition in plain language.
- **Posture / screen-time break reminder** desktop app using the webcam (on-device only).
- **Sleep or step data analysis** — export your own wearable data and build an insightful dashboard + blog post.
- **Evidence-based health tips site** where every tip links to a source (static site, community-contributed via PRs — doubles as an open-source project others can contribute to!).

### Developer tools
- A CLI that automates something tedious in your workflow
- A VS Code / browser extension
- A GitHub Action that others can reuse
- A Python library wrapping a useful public API

### Social impact / campus
- Lost-and-found / ride-share / book-exchange app for your campus
- Accessibility tools (screen-reader-friendly versions of course materials, captioning)
- Open datasets for your local language, city, or region

## Team project survival tips

- Agree on **scope, roles, and weekly meeting time** on day one.
- Use issues and PRs even in a team of two — it builds good habits and a visible history.
- Write decisions down (a `docs/decisions.md` file).
- Have a deadline (hackathon, demo day, semester end). Projects without deadlines drift.
- It's okay to archive a project — but write a final post about what you learned.

## What makes a project impressive to others

1. **It works** and someone can try it in < 2 minutes (live demo link or `pip install`).
2. **It's documented** — README with screenshots/GIF, architecture explanation.
3. **It has users or results** — stars, downloads, a benchmark number, feedback.
4. **You can explain the trade-offs** you made and what you'd do differently.
