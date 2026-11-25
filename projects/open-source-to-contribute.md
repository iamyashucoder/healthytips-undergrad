# Important Open-Source Projects to Contribute To

These projects matter: they are widely used, actively maintained, and most of them welcome new contributors.

**How to start with any of them:**
1. Star and fork the repo, then read `CONTRIBUTING.md`.
2. Build it locally and run the tests.
3. Open the **Issues** tab and filter by the label in the "Start with" column. Label names differ slightly between repos; check the repo's label list.
4. Comment on the issue before you start working.

> Repos sometimes move to new organizations. If a link redirects, use the new location.

---

## 🧠 AI / Machine Learning

| Project | Link | Lang | Why it's important | Start with | Level |
|---------|------|------|--------------------|-----------|-------|
| Hugging Face Transformers | [huggingface/transformers](https://github.com/huggingface/transformers) | Python | The standard library for pretrained models | `Good First Issue`, docs, model cards | 🟡 |
| Hugging Face Datasets | [huggingface/datasets](https://github.com/huggingface/datasets) | Python | Dataset loading/processing used everywhere | `good first issue` | 🟢 |
| Diffusers | [huggingface/diffusers](https://github.com/huggingface/diffusers) | Python | Image/video diffusion models | `good first issue`, docs | 🟡 |
| PEFT | [huggingface/peft](https://github.com/huggingface/peft) | Python | LoRA and efficient fine-tuning | docs, examples, tests | 🟡 |
| PyTorch | [pytorch/pytorch](https://github.com/pytorch/pytorch) | Python/C++ | Core deep learning framework | `good first issue`, docs | 🔴 |
| scikit-learn | [scikit-learn/scikit-learn](https://github.com/scikit-learn/scikit-learn) | Python | Classic ML; excellent contributor guide | `good first issue`, `Easy`, docs | 🟢 |
| Keras | [keras-team/keras](https://github.com/keras-team/keras) | Python | High-level multi-backend DL API | `good first issue` | 🟡 |
| JAX | [jax-ml/jax](https://github.com/jax-ml/jax) | Python | Research-grade numerical computing | docs, `good first issue` | 🔴 |
| PyTorch Lightning | [Lightning-AI/pytorch-lightning](https://github.com/Lightning-AI/pytorch-lightning) | Python | Training framework | `good first issue` | 🟡 |
| lm-evaluation-harness | [EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) | Python | The standard LLM benchmark runner | add a new task/benchmark | 🟡 |
| vLLM | [vllm-project/vllm](https://github.com/vllm-project/vllm) | Python/CUDA | Fast LLM inference serving | `good first issue` | 🔴 |
| llama.cpp | [ggml-org/llama.cpp](https://github.com/ggml-org/llama.cpp) | C/C++ | Running LLMs locally on any hardware | `good first issue` | 🔴 |
| Ollama | [ollama/ollama](https://github.com/ollama/ollama) | Go | Local LLM runner | docs, bugs | 🟡 |
| tinygrad | [tinygrad/tinygrad](https://github.com/tinygrad/tinygrad) | Python | Small, readable DL framework — great to learn internals | read code, small fixes | 🔴 |
| spaCy | [explosion/spaCy](https://github.com/explosion/spaCy) | Python/Cython | Industrial NLP | docs, language support | 🟡 |
| OpenCV | [opencv/opencv](https://github.com/opencv/opencv) | C++/Python | Computer vision standard | `good first issue` | 🟡 |
| Gradio | [gradio-app/gradio](https://github.com/gradio-app/gradio) | Python/TS | ML demo UIs | `good first issue` | 🟢 |
| Streamlit | [streamlit/streamlit](https://github.com/streamlit/streamlit) | Python/TS | Data apps | `good first issue` | 🟢 |
| MLflow | [mlflow/mlflow](https://github.com/mlflow/mlflow) | Python | Experiment tracking / MLOps | `good first issue` | 🟡 |
| LangChain | [langchain-ai/langchain](https://github.com/langchain-ai/langchain) | Python | LLM app framework | docs, integrations | 🟡 |
| LlamaIndex | [run-llama/llama_index](https://github.com/run-llama/llama_index) | Python | RAG/data framework for LLMs | integrations, docs | 🟡 |

## 📊 Data Science & Scientific Python

| Project | Link | Lang | Why it's important | Start with | Level |
|---------|------|------|--------------------|-----------|-------|
| NumPy | [numpy/numpy](https://github.com/numpy/numpy) | Python/C | Foundation of scientific Python | `good first issue`, docs | 🟡 |
| pandas | [pandas-dev/pandas](https://github.com/pandas-dev/pandas) | Python | Data analysis standard | `good first issue`, `Docs` | 🟢 |
| Polars | [pola-rs/polars](https://github.com/pola-rs/polars) | Rust/Python | Fast DataFrames | `good first issue` | 🟡 |
| matplotlib | [matplotlib/matplotlib](https://github.com/matplotlib/matplotlib) | Python | Plotting standard | `Good first issue` | 🟢 |
| SciPy | [scipy/scipy](https://github.com/scipy/scipy) | Python/C | Scientific algorithms | `good first issue` | 🟡 |
| SymPy | [sympy/sympy](https://github.com/sympy/sympy) | Python | Symbolic math; very newcomer-friendly | `Easy to Fix` | 🟢 |
| NetworkX | [networkx/networkx](https://github.com/networkx/networkx) | Python | Graph algorithms | `good first issue` | 🟢 |
| PyMC | [pymc-devs/pymc](https://github.com/pymc-devs/pymc) | Python | Bayesian modeling | `beginner friendly` | 🟡 |
| JupyterLab | [jupyterlab/jupyterlab](https://github.com/jupyterlab/jupyterlab) | TS/Python | Notebook interface used by millions | `good first issue` | 🟡 |

## 🩺 Health, Biology & Science

| Project | Link | Lang | Why it's important | Start with | Level |
|---------|------|------|--------------------|-----------|-------|
| MONAI | [Project-MONAI/MONAI](https://github.com/Project-MONAI/MONAI) | Python | Deep learning for medical imaging | `good first issue`, tutorials | 🟡 |
| OpenMRS | [openmrs/openmrs-core](https://github.com/openmrs/openmrs-core) | Java | Medical records for low-resource clinics | their "intro" tickets on OpenMRS Talk/Jira | 🟡 |
| Open Food Facts | [openfoodfacts/openfoodfacts-server](https://github.com/openfoodfacts/openfoodfacts-server) | Perl/JS | Open food & nutrition database | `good first issue` | 🟢 |
| Open Food Facts (mobile app) | [openfoodfacts/smooth-app](https://github.com/openfoodfacts/smooth-app) | Dart/Flutter | The scanner app | `good first issue` | 🟢 |
| Biopython | [biopython/biopython](https://github.com/biopython/biopython) | Python | Computational biology | docs, tests | 🟡 |
| scanpy | [scverse/scanpy](https://github.com/scverse/scanpy) | Python | Single-cell genomics | `good first issue` | 🟡 |
| nilearn | [nilearn/nilearn](https://github.com/nilearn/nilearn) | Python | Machine learning for neuroimaging | `Good first issue` | 🟡 |

## 🌍 Social Impact & Education

| Project | Link | Lang | Why it's important | Start with | Level |
|---------|------|------|--------------------|-----------|-------|
| Oppia | [oppia/oppia](https://github.com/oppia/oppia) | Python/TS | Free interactive education; strong mentoring | `good first issue` + their onboarding | 🟢 |
| freeCodeCamp | [freeCodeCamp/freeCodeCamp](https://github.com/freeCodeCamp/freeCodeCamp) | JS/TS | Free coding education | `first timers only`, `help wanted` | 🟢 |
| MDN Web Docs | [mdn/content](https://github.com/mdn/content) | Markdown | The web's documentation | `good first issue` | 🟢 |
| Zulip | [zulip/zulip](https://github.com/zulip/zulip) | Python/JS | Open-source team chat; excellent newcomer docs | `good first issue` | 🟢 |
| Wikipedia / MediaWiki | [wikimedia/mediawiki](https://github.com/wikimedia/mediawiki) | PHP | Powers Wikipedia | "good first task" on Phabricator | 🟡 |

## 🛠 Developer Tools

| Project | Link | Lang | Why it's important | Start with | Level |
|---------|------|------|--------------------|-----------|-------|
| VS Code | [microsoft/vscode](https://github.com/microsoft/vscode) | TS | Most-used editor | `good first issue` | 🟡 |
| Neovim | [neovim/neovim](https://github.com/neovim/neovim) | C/Lua | Modern Vim | `good first issue` | 🟡 |
| Ruff | [astral-sh/ruff](https://github.com/astral-sh/ruff) | Rust | Very fast Python linter | `good first issue` (new lint rules) | 🟡 |
| uv | [astral-sh/uv](https://github.com/astral-sh/uv) | Rust | Fast Python package manager | `good first issue` | 🟡 |
| FastAPI | [fastapi/fastapi](https://github.com/fastapi/fastapi) | Python | Modern web APIs; docs translations welcome | docs, translations | 🟢 |
| Excalidraw | [excalidraw/excalidraw](https://github.com/excalidraw/excalidraw) | TS/React | Whiteboard drawing | `good first issue` | 🟢 |
| Home Assistant | [home-assistant/core](https://github.com/home-assistant/core) | Python | Smart-home platform; add integrations | integrations, docs | 🟡 |
| Godot Engine | [godotengine/godot](https://github.com/godotengine/godot) | C++ | Open-source game engine | `good first issue`, docs | 🟡 |

## ⚙️ Systems, Languages & Infrastructure

| Project | Link | Lang | Why it's important | Start with | Level |
|---------|------|------|--------------------|-----------|-------|
| CPython | [python/cpython](https://github.com/python/cpython) | C/Python | The Python language itself | `easy`, docs (read the devguide) | 🔴 |
| Rust | [rust-lang/rust](https://github.com/rust-lang/rust) | Rust | Systems language | `E-easy`, `E-mentor` | 🔴 |
| Kubernetes | [kubernetes/kubernetes](https://github.com/kubernetes/kubernetes) | Go | Container orchestration standard | `good first issue` (via LFX mentorship) | 🔴 |
| Apache Airflow | [apache/airflow](https://github.com/apache/airflow) | Python | Data pipeline orchestration | `good first issue` | 🟡 |

## 🐣 Practice Repos (for your very first PR)

| Project | Link | Purpose |
|---------|------|---------|
| First Contributions | [firstcontributions/first-contributions](https://github.com/firstcontributions/first-contributions) | Practice the fork → PR workflow in 10 minutes |
| The Algorithms (Python) | [TheAlgorithms/Python](https://github.com/TheAlgorithms/Python) | Add or improve algorithm implementations with tests |

## 🔍 Places to discover more

- [goodfirstissue.dev](https://goodfirstissue.dev) — curated beginner issues
- [up-for-grabs.net](https://up-for-grabs.net) — projects with tasks for new contributors
- GitHub search: `label:"good first issue" is:open language:python`
- [GSoC organizations list](https://summerofcode.withgoogle.com/) — every org listed there is set up to mentor students

---

## Suggested focus paths

Pick one path and stay with it for at least a semester.

| If you like… | Start here | Then go deeper |
|--------------|-----------|----------------|
| Classic ML / data | scikit-learn, pandas docs | NumPy, SciPy, Polars |
| LLMs / NLP | HF datasets, lm-evaluation-harness | Transformers, vLLM, llama.cpp |
| Healthcare + AI | Open Food Facts, MONAI tutorials | MONAI core, OpenMRS |
| Web dev | freeCodeCamp, MDN, Excalidraw | Zulip, VS Code |
| Systems | TheAlgorithms, Ruff lint rules | uv, Rust, CPython |
