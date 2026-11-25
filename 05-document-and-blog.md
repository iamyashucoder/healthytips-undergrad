# 05 — Document It Well. Blog About It.

> If you built something great but no one can understand or find it, it might as well not exist.

## Part A: Documenting your projects

### The README is your project's front door

Template you can copy:

```markdown
# Project Name
One-sentence description of what it does and who it's for.

![demo](docs/demo.gif)   <!-- a GIF or screenshot is worth 1000 words -->

[Live demo](https://...) · [Blog post](https://...) · [Docs](https://...)

## Why
The problem this solves, in 2–3 sentences.

## Features
- Feature 1
- Feature 2

## Quick start
​```bash
pip install your-package
your-command --example
​```

## How it works
Short explanation + architecture diagram.

## Results / Benchmarks   (for ML/research projects)
| Model | Accuracy | Notes |

## Roadmap
- [x] Done thing
- [ ] Next thing

## Contributing
See CONTRIBUTING.md. Good first issues are labeled `good first issue`.

## License
MIT

## Acknowledgements
People, papers, datasets you built on.
```

### Documentation checklist

- [ ] README (above)
- [ ] `LICENSE` file
- [ ] `CONTRIBUTING.md` (how to set up, run tests, submit PRs)
- [ ] `CHANGELOG.md` for releases
- [ ] Docstrings / code comments explaining **why**, not just **what**
- [ ] Architecture diagram (draw.io, Excalidraw, Mermaid)
- [ ] For ML: model card / dataset card (data sources, limitations, ethics)
- [ ] For research: exact commands to reproduce each result in the paper/blog
- [ ] Docs site for bigger projects (MkDocs Material, Sphinx, Docusaurus)

### The Diátaxis idea (how good docs are organized)
Good documentation has four kinds of content:
1. **Tutorials** — learning-oriented ("build your first X")
2. **How-to guides** — task-oriented ("how to deploy to Y")
3. **Reference** — information-oriented (API docs)
4. **Explanation** — understanding-oriented ("why we designed it this way")

## Part B: Blogging

### Why blog?
- Writing forces you to truly understand something.
- Posts are searchable forever — people find you through them (recruiters, professors, collaborators).
- It's a record of your growth.

### Where to host

| Option | Effort | Notes |
|--------|--------|-------|
| **dev.to / Hashnode / Medium** | Lowest | Built-in audience; less control |
| **GitHub Pages + Jekyll / Hugo / Astro** | Medium | Free, you own it, markdown-based — recommended |
| **Quarto / Jupyter Book / fastpages-style** | Medium | Great for ML posts with code and plots |
| **Personal domain** | Medium | ~$10–15/year; looks professional |

Tip: publish on your own site, then cross-post to dev.to/Hashnode/LinkedIn with a link back (canonical URL).

### What to write about (you have more ideas than you think)

- **"I built X"** — project write-ups: problem → approach → challenges → results → what's next
- **"TIL / How I fixed Y"** — a bug that took you 3 hours to solve will save someone else 3 hours
- **Paper explainers** — summarize a paper in plain language with diagrams
- **Reproduction reports** — "I tried to reproduce paper Z; here's what matched and what didn't"
- **My first open-source contribution** — newcomers love these
- **Learning logs** — "What I learned in 30 days of learning Rust"
- **Tutorials** — the guide you wish existed when you started
- **Event recaps** — hackathons, conferences, research internships
- **Health/tech crossover** — e.g., "I analyzed a year of my sleep data"

### A simple post structure

1. **Hook** — the problem or question (1 paragraph)
2. **Context** — why it matters, what you tried
3. **The meat** — code, diagrams, results, screenshots
4. **Lessons / pitfalls**
5. **Links** — repo, demo, references
6. **Call to action** — "Feedback welcome", "Contributions welcome"

### Writing habits
- Aim for **1 post per month**. Consistency beats perfection.
- Keep a `drafts/` list of ideas; add to it whenever you learn something.
- Short is fine. 500 useful words > 3000 words never published.
- Ask a friend to read it before you publish.

## Part C: Your public portfolio

- **GitHub profile README** — who you are, what you're working on, pinned best 4–6 repos.
- **Personal website** — About, Projects, Blog, Publications, CV.
- **LinkedIn** — post when you ship something or publish a post (short + link).
- **Google Scholar / ORCID** — once you have publications.
- **Hugging Face profile** — for models, datasets, Spaces.
- **Talks** — present at a club meeting, local meetup, or lightning talk. Upload slides.

> One well-documented project + one well-written blog post about it is often what gets you the interview.
