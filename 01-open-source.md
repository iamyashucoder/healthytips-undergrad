# 01 — Contributing to Open Source

## Why it matters

- Real code review from experienced engineers (free mentorship).
- A public, verifiable record of your work (recruiters and admissions committees can click and see it).
- You learn how large codebases, CI, testing, and collaboration actually work.
- Leads to programs like GSoC/Outreachy (paid), internships, and maintainer roles.

## The contribution ladder

You don't start by writing a new feature. Climb step by step:

| Level | What you do | Example |
|-------|-------------|---------|
| 0. User | Use the project seriously | Use a library in your coursework |
| 1. Reporter | File clear bug reports with reproductions | "Function X crashes on empty input — minimal example attached" |
| 2. Docs contributor | Fix typos, broken links, unclear docs, add examples | Add a missing example to an API docstring |
| 3. Tester | Add tests, reproduce/triage issues others reported | Confirm a bug on your OS, write a failing test |
| 4. Code contributor | Fix `good first issue` bugs, then larger bugs | Fix an off-by-one error |
| 5. Feature contributor | Propose (in an issue first!) and implement features | Add a new option to a CLI |
| 6. Reviewer / triager | Review others' PRs, label issues, help newcomers | Answer questions in the project's forum/Discord |
| 7. Maintainer | Get commit rights, own a module, cut releases | Become a core developer |

## Step-by-step: your first PR

1. **Pick a project you use.** You'll understand the problem domain and stay motivated.
2. **Read the house rules:** `README.md`, `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, and the dev setup guide.
3. **Build it locally and run the tests.** This alone teaches you a lot — and if the setup docs are wrong, that's your first PR.
4. **Find an issue** labeled `good first issue`, `help wanted`, `documentation`, or `easy`.
5. **Comment before you start:** "Hi, I'd like to work on this. My plan is X. Does that sound right?" Wait for a response if the project asks you to.
6. **Make a small, focused change** on a new branch. One PR = one logical change.
7. **Write a good PR description:** what changed, why, how you tested it, and `Fixes #123`.
8. **Respond to review politely and quickly.** Review comments are a gift, not criticism.
9. **After merging, pick the next issue in the same project.** Depth compounds.

### Git workflow cheat sheet

```bash
# Fork on GitHub, then:
git clone https://github.com/<you>/<project>.git
cd <project>
git remote add upstream https://github.com/<org>/<project>.git

git checkout -b fix-issue-123
# ... make changes, run tests ...
git add -p                       # review what you stage
git commit -m "Fix crash on empty input in parse() (#123)"
git push origin fix-issue-123
# Open a PR on GitHub

# Keep your branch up to date:
git fetch upstream
git rebase upstream/main
```

## Where to find beginner-friendly issues

- **goodfirstissue.dev** — curated good-first-issues from popular repos
- **up-for-grabs.net** — projects with tasks for new contributors
- **GitHub search:** `is:issue is:open label:"good first issue" language:python`
- **GitHub Explore → Topics** for your interests (e.g., `machine-learning`, `rust`, `accessibility`)
- **The issue tracker of tools you already use** (often the best option)

## Project suggestions by area

These are generally welcoming to newcomers and have good contributor docs (always verify current status):

**AI / ML / Data**
- Hugging Face `transformers`, `datasets`, `diffusers`, `peft` (also: write model cards, docs, translations)
- PyTorch, `torchvision`, PyTorch Lightning
- scikit-learn (famous for excellent contributor docs)
- NumPy, pandas, SciPy, matplotlib, Jupyter
- LangChain / LlamaIndex style ecosystems, vLLM, llama.cpp (more advanced)
- EleutherAI `lm-evaluation-harness` (add benchmarks/tasks)

**Web / Apps**
- freeCodeCamp, MDN Web Docs content, Excalidraw, Zulip, Mattermost
- Oppia (education), OpenMRS (healthcare), Public Lab — social-impact projects with strong mentorship

**Systems / Dev tools**
- Rust ecosystem (crates with `E-easy` labels), Python CPython docs, VS Code extensions, Neovim plugins
- Kubernetes & CNCF projects (via LFX mentorship)

**Science & Health** *(fits a "healthy tips" interest!)*
- OpenMRS, Open Food Facts, MONAI (medical imaging), Biopython, nilearn

## Make / improve a library

Once you've contributed a bit, consider:

- **Fill a gap:** a missing Python wrapper for an API, a utility you copy-paste between projects, a port of a tool to another language.
- **Improve an existing small library:** add type hints, tests, docs, CI, packaging. Many useful libraries are under-maintained — ask the author if you can help co-maintain.
- **Library checklist:**
  - [ ] Clear README with install + 30-second example
  - [ ] Tests + CI (GitHub Actions)
  - [ ] Published package (PyPI / npm / crates.io)
  - [ ] Semantic versioning + CHANGELOG
  - [ ] License (MIT / Apache-2.0 are common)
  - [ ] Docs site (MkDocs, Sphinx, Docusaurus)
  - [ ] Contributing guide + `good first issue` labels for *your* newcomers

## Etiquette (do / don't)

| Do | Don't |
|----|-------|
| Search existing issues before opening one | Open "Can I work on this?" on 10 issues at once |
| Keep PRs small and focused | Submit huge PRs nobody asked for |
| Be patient — maintainers are often volunteers | Ping maintainers daily |
| Thank reviewers, accept feedback | Argue defensively |
| Disclose if you used AI tools, and understand every line you submit | Submit AI-generated PRs you can't explain (many projects now reject these) |
| Do Hacktoberfest-style events with real contributions | Spam trivial PRs for swag |
