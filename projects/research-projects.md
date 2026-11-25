# Research Projects for Undergrads

Research-style projects show professors and admissions committees that you can work on open-ended problems. Start with reproductions, then move to small original contributions.

## Level 1: Reproduce a Paper

Reimplement the key result **without copying the official code**. Then compare with the official code and write up where your result matches or differs.

| Paper | Area | Why it's a good reproduction | Compute needed |
|-------|------|------------------------------|----------------|
| *ImageNet Classification with Deep CNNs* (AlexNet, 2012) — reproduce on CIFAR-10 | Vision | Fundamentals of CNN training | 1 GPU / Colab |
| *Deep Residual Learning* (ResNet, 2015) — on CIFAR-10 | Vision | Shows why skip connections matter; easy to do ablations | 1 GPU |
| *Dropout* (Srivastava et al., 2014) | Regularization | Simple, clear experiments | CPU/Colab |
| *Batch Normalization* (Ioffe & Szegedy, 2015) | Optimization | Try to reproduce the training-speed claims | 1 GPU |
| *Adam* (Kingma & Ba, 2014) — compare optimizers | Optimization | Good plotting/analysis practice | CPU/Colab |
| *Attention Is All You Need* (2017) — small-scale translation | NLP | Core of modern AI | 1 GPU |
| *Word2Vec* (Mikolov et al., 2013) | NLP | Embeddings from scratch | CPU |
| *GANs* (Goodfellow et al., 2014) / DCGAN | Generative | Classic training-instability lessons | 1 GPU |
| *DDPM — Denoising Diffusion Probabilistic Models* (2020) on MNIST/CIFAR | Generative | Foundation of modern image generation | 1 GPU |
| *LoRA* (Hu et al., 2021) | LLMs | Compare LoRA vs full fine-tuning on a small model | 1 GPU |
| *Chain-of-Thought Prompting* (Wei et al., 2022) | LLMs | Evaluate on small open models | API or 1 GPU |
| *U-Net* (Ronneberger et al., 2015) on a public medical segmentation dataset | Medical imaging | Health + vision; widely used | 1 GPU |
| *Playing Atari with Deep RL* (DQN, 2013) — CartPole/simple Atari | RL | RL fundamentals | 1 GPU |

**Deliverable:** repo + blog post titled "Reproducing [Paper]: what matched, what didn't."
**Bonus:** submit your reproduction to a reproducibility challenge or workshop (ML conferences have run these, e.g., the ML Reproducibility Challenge).

## Level 2: Extend a Paper

Take a reproduced paper and ask a new question:
- Does the result hold on a **different dataset or domain** (e.g., medical images, your local language)?
- What happens with **less data or compute**?
- Which components actually matter? Run an **ablation study**.
- Is it **robust** to noise, distribution shift or adversarial inputs?
- Is it **fair** across subgroups?

## Level 3: Small Original Contributions

| Idea | What you produce | Who'd care |
|------|------------------|-----------|
| **New benchmark** for something LLMs are bad at (local culture, math in your language, health-misinformation detection) | Dataset + eval harness + baseline results | Workshop paper; add to lm-evaluation-harness |
| **Low-resource language dataset** (speech, text, QA) | Cleaned dataset with a dataset card on Hugging Face | Communities like Masakhane; language-tech workshops |
| **Medical AI robustness study**: does a public model fail on images from different hospitals or devices? | Analysis + code | Medical imaging workshops |
| **Interpretability** of a small model: find circuits/features for a simple behavior | Notebook + blog + writeup | Interpretability community (very open to newcomers) |
| **Efficient ML**: make a model run on a phone or microcontroller with minimal accuracy loss | Benchmarks + code | TinyML / efficiency workshops |
| **Data quality audit** of a popular dataset (label errors, duplicates, bias) | Report + cleaned version | Dataset/benchmark tracks |
| **Health misinformation detection** for social media posts | Dataset + classifier + error analysis | NLP-for-social-good workshops |

## Where to publish undergrad work

- **Workshops** at major ML conferences (NeurIPS, ICML, ICLR, ACL, CVPR, MICCAI) — shorter papers, more welcoming
- **Student research workshops** (e.g., ACL Student Research Workshop)
- **Affinity workshops** (WiML, Black in AI, LatinX in AI, Queer in AI) — they welcome undergrads
- **Undergraduate research symposiums** at your university
- **arXiv** (with your advisor's approval) and a blog post explaining the paper

## Research project workflow

1. **Question** — write it down in one sentence.
2. **Related work** — read 5–10 papers; keep notes in Zotero/Obsidian.
3. **Baseline** — reproduce the existing best simple method.
4. **Experiments** — change one thing at a time; track with W&B/MLflow; fix seeds.
5. **Analysis** — plots, tables, error analysis. What failed, and why?
6. **Write** — Overleaf + LaTeX; get feedback from a PhD student or advisor.
7. **Release** — clean code, README with exact reproduce commands, model/dataset on HF.
8. **Share** — blog post, X/LinkedIn thread, talk at your lab or club.

## Tools

| Purpose | Tools |
|---------|-------|
| Finding papers | Google Scholar, Semantic Scholar, arXiv, Papers with Code-style leaderboards, Connected Papers |
| Reading & notes | Zotero, Obsidian, Notion |
| Experiments | PyTorch, Weights & Biases, MLflow, Hydra (configs) |
| Free compute | Google Colab, Kaggle notebooks (free GPU hours), your university cluster, cloud student credits |
| Writing | Overleaf, LaTeX, draw.io / Excalidraw for figures |
