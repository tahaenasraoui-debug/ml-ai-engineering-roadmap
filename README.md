# ML & AI Engineering Roadmap

![Python](https://img.shields.io/badge/python-3.11+-blue.svg)
![Type Checked](https://img.shields.io/badge/types-mypy%20strict-informational.svg)
![Tests](https://img.shields.io/badge/tests-pytest-success.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

A personal, build-first path from calculus and Python basics to deep learning and applied AI. Concise primers sit next to core textbooks. No semester-long lecture playlists.

---

## Table of Contents

1. [Workflow Overview](#workflow-overview)
2. [Progress Dashboard](#progress-dashboard)
3. [Stage 0: Fast Math Foundations](#stage-0-fast-math-foundations--intuition)
4. [Stage 1: Python Foundations & System Scripting](#stage-1-python-foundations--system-scripting)
5. [Stage 2: Modern OOP & Software Engineering](#stage-2-modern-oop--software-engineering)
6. [Stage 3: The Mathematical Engine for ML](#stage-3-the-mathematical-engine-for-ml)
7. [Stage 4: Numerical Stack & Classical ML](#stage-4-numerical-stack--classical-machine-learning)
8. [Stage 5: Deep Learning & Modern Applied AI](#stage-5-deep-learning--modern-applied-ai)
9. [Parallel Track: Data Structures & Algorithms](#parallel-track-data-structures--algorithms)
10. [Cracked Tier: Beyond the Core Path](#cracked-tier-beyond-the-core-path)
11. [Repository Layout](#repository-layout)
12. [Engineering Rules](#engineering-rules)

---

## Workflow Overview

```
  STAGE 0            STAGE 1               STAGE 2
 Math primers  -->  Python + scripting --> OOP + engineering
 (intuition)        (automation)           (clean design)
                                              |
                                              v
  STAGE 5            STAGE 4               STAGE 3
 DL + Applied  <--  NumPy/Pandas +    <--  Linear algebra,
 AI (PyTorch,       classical ML           calculus,
 HF, RAG)           (scikit-learn)         probability
```

DSA runs in parallel the whole way (45 to 60 min/day):

```
  D1 Fundamentals --> D2 Trees + Graphs --> D3 DP + Advanced --> D4 Depth + Contests
  (Stages 1-2)        (Stages 2-3)          (Stages 3-4)         (Stages 4-5)
```

Per-session loop:

```
  [ Theory 25% ] --> [ Build 75% ] --> [ Test + type check ] --> [ Commit to branch ] --> [ PR + merge ]
```

---

## Progress Dashboard

| Stage | Focus | Primary Deliverable | Status |
|-------|-------|---------------------|--------|
| 0 | Math intuition | Worked-problem notebook | - [ ] |
| 1 | Python + scripting | 3 CLI automation tools | - [ ] |
| 2 | OOP + engineering | Typed, tested package | - [ ] |
| 3 | Math for ML | Derivations + NumPy verifications | - [ ] |
| 4 | Classical ML | End-to-end sklearn project | - [ ] |
| 5 | Deep learning + applied AI | micrograd, GPT, fine-tune, RAG app | - [ ] |
| D | DSA (parallel track) | NeetCode 150 + 100 extra mediums, typed solutions repo | - [ ] |

---

## Stage 0: Fast Math Foundations & Intuition

Goal: build geometric intuition before formalism. Finish in days, not weeks.

### Fast Calculus Intuition

| Resource | Type | Why |
|----------|------|-----|
| [3Blue1Brown: Essence of Calculus](https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr) | Video playlist | Concise visual intuition for derivatives, integrals, limits |
| [Paul's Online Math Notes: Calculus I](https://tutorial.math.lamar.edu/Classes/CalcI/CalcI.aspx) | Notes | Compact cheat sheets and worked problems |

- [ ] Watch all of Essence of Calculus
- [ ] Work Paul's Notes problems on derivatives and the chain rule
- [ ] Work Paul's Notes problems on integrals and the fundamental theorem
- [ ] Deliverable: `notebooks/00_math/calculus_review.ipynb`

### Fast Linear Algebra Intuition

| Resource | Type | Why |
|----------|------|-----|
| [3Blue1Brown: Essence of Linear Algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) | Video playlist | Vectors, matrices, transformations as geometry |
| [Immersive Linear Algebra](http://immersivemath.com/ila/index.html) | Interactive book | In-browser 3D diagrams |

- [ ] Watch all of Essence of Linear Algebra
- [ ] Complete Immersive Linear Algebra chapters on vectors, matrices, and determinants
- [ ] Complete Immersive Linear Algebra chapters on eigenvalues and decompositions
- [ ] Deliverable: `notebooks/00_math/linear_algebra_review.ipynb`

**Exit criteria**
- [ ] Explain a derivative, a gradient, and an eigenvector without notation
- [ ] Visualize a 2D linear transformation in NumPy/Matplotlib

---

## Stage 1: Python Foundations & System Scripting

| Resource | Type | Scope |
|----------|------|-------|
| [4-Hour Python Crash Course with OOP](https://www.youtube.com/watch?v=rfscVS0vtbw) | Video | End-to-end tutorial |
| [Automate the Boring Stuff with Python, 3rd Ed (Al Sweigart)](https://automatetheboringstuff.com/) | Free online book | Emphasis on Part II |

- [ ] Finish the crash course with code-along
- [ ] Automate the Boring Stuff, Part I: core language
- [ ] Part II: regular expressions
- [ ] Part II: `pathlib` and `shutil` file handling
- [ ] Part II: `requests` and `bs4` scraping
- [ ] Part II: JSON and web APIs

**Deliverables**
- [ ] `src/scripts/file_organizer.py` (pathlib + shutil)
- [ ] `src/scripts/web_scraper.py` (requests + bs4, JSON output)
- [ ] `src/scripts/api_client.py` (requests, typed responses)
- [ ] Tests for each script in `tests/scripts/`

---

## Stage 2: Modern OOP & Software Engineering

| Resource | Type | Scope |
|----------|------|-------|
| [ArjanCodes (YouTube)](https://www.youtube.com/@ArjanCodes) | Video channel | Clean design, dataclasses, composition. Pick specific videos, do not binge. |
| [Python 3 Object-Oriented Programming (Phillips & Lott)](https://www.packtpub.com/product/python-3-object-oriented-programming-fourth-edition/9781801077262) | Book | OOP mechanics and patterns |
| [Effective Python (Brett Slatkin)](https://effectivepython.com/) | Book | Concrete engineering items |
| [Fluent Python, 2nd Ed (Luciano Ramalho)](https://www.fluentpython.com/) | Book | Python data model reference |

- [ ] Phillips & Lott: classes, inheritance, special methods
- [ ] Phillips & Lott: design patterns and testing OOP code
- [ ] Effective Python: items on functions, comprehensions, and generators
- [ ] Effective Python: items on classes, concurrency, and robustness
- [ ] Fluent Python: data model and special methods
- [ ] Fluent Python: sequences, mappings, and dataclasses
- [ ] ArjanCodes: dataclasses, composition over inheritance, dependency injection

**Deliverables**
- [ ] `src/engine/` package with dataclasses and composition (no deep inheritance)
- [ ] `mypy --strict` passes on the package
- [ ] `pytest` coverage of at least 80% on the package
- [ ] `docs/design_notes.md` documenting three design trade-offs

---

## Stage 3: The Mathematical Engine for ML

| Resource | Type | Domain |
|----------|------|--------|
| [Linear Algebra and Learning from Data (Strang)](https://math.mit.edu/~gs/learningfromdata/) | Textbook site | Linear algebra for ML |
| [Mathematics for Machine Learning (Deisenroth, Faisal, Ong)](https://mml-book.com/) | Free textbook | Multivariate calculus and optimization |
| [Introduction to Probability (Blitzstein & Hwang)](http://probabilitybook.net/) | Free book site (Harvard Stat 110) | Probability and statistics |

- [ ] Strang: matrix factorizations, SVD, and low-rank structure
- [ ] Strang: least squares and the link to learning from data
- [ ] MML: analytic geometry, matrix decompositions
- [ ] MML: vector calculus and backpropagation
- [ ] MML: continuous optimization (gradient descent, constrained optimization)
- [ ] Blitzstein & Hwang: conditional probability, random variables, expectation
- [ ] Blitzstein & Hwang: common distributions, joint distributions, limit theorems

**Deliverables**
- [ ] `notebooks/03_math/svd_from_scratch.ipynb`
- [ ] `notebooks/03_math/gradient_descent_from_scratch.ipynb`
- [ ] `notebooks/03_math/probability_simulations.ipynb`
- [ ] `src/mathlib/` with typed, tested implementations of the above

---

## Stage 4: Numerical Stack & Classical Machine Learning

| Resource | Type | Role |
|----------|------|------|
| [Python for Data Analysis (Wes McKinney)](https://wesmckinney.com/book/) | Free online book | NumPy and Pandas |
| [100 NumPy Exercises](https://github.com/rougier/numpy-100) | GitHub repo | Vectorization drills |
| [Hands-On Machine Learning, 3rd Ed (Géron)](https://github.com/ageron/handson-ml3) | Book + notebooks | Applied classical ML |
| [Pattern Recognition and Machine Learning (Bishop)](https://www.microsoft.com/en-us/research/publication/pattern-recognition-and-machine-learning/) | Free PDF | Mathematical rigor |

- [ ] McKinney: NumPy basics and arrays
- [ ] McKinney: Pandas data loading, cleaning, wrangling
- [ ] McKinney: groupby, time series, and aggregation
- [ ] Complete all 100 NumPy exercises
- [ ] Géron: end-to-end project, classification, training models
- [ ] Géron: SVMs, decision trees, ensembles, dimensionality reduction
- [ ] Bishop: linear models for regression and classification
- [ ] Bishop: kernel methods, graphical models, mixture models and EM

**Deliverables**
- [ ] `notebooks/04_ml/end_to_end_project.ipynb` (data to deployed pipeline)
- [ ] `src/ml/pipeline.py` with typed sklearn pipeline and tests
- [ ] Implement linear regression, logistic regression, and k-means from scratch in `src/ml/scratch/`
- [ ] `docs/ml_report.md` comparing scratch vs scikit-learn results

---

## Stage 5: Deep Learning & Modern Applied AI

| Resource | Type | Role |
|----------|------|------|
| [PyTorch Official Tutorials](https://pytorch.org/tutorials/) | Docs | Framework fluency |
| [Deep Learning (Goodfellow, Bengio, Courville)](https://www.deeplearningbook.org/) | Free online text | Theory |
| [Neural Networks: Zero to Hero (Karpathy)](https://github.com/karpathy/nn-zero-to-hero) | Repo + videos | Build micrograd and GPT from scratch |
| [Hugging Face Course](https://huggingface.co/learn/nlp-course) | Course | Transformers in practice |
| [PEFT / LoRA Docs](https://huggingface.co/docs/peft/) | Docs | Parameter-efficient fine-tuning |
| [ChromaDB Documentation](https://docs.trychroma.com/) | Docs | Vector store for retrieval |

- [ ] PyTorch tutorials: tensors, autograd, `nn.Module`, training loop
- [ ] Zero to Hero: micrograd
- [ ] Zero to Hero: makemore series
- [ ] Zero to Hero: build GPT from scratch
- [ ] Deep Learning book: Part II (deep networks, regularization, optimization)
- [ ] Hugging Face Course: transformers, tokenizers, fine-tuning
- [ ] PEFT docs: apply LoRA to a small model
- [ ] ChromaDB docs: collections, embeddings, querying

**Deliverables**
- [ ] `src/dl/micrograd/` with tests against PyTorch gradients
- [ ] `src/dl/gpt/` character-level GPT trained on a small corpus
- [ ] `notebooks/05_dl/lora_finetune.ipynb`
- [ ] `src/apps/rag_app/` retrieval app using ChromaDB, typed and tested
- [ ] `docs/capstone.md` writing up the RAG app: architecture, evaluation, failure modes

---

## Parallel Track: Data Structures & Algorithms

Runs alongside Stages 1 to 5 as a daily habit of 45 to 60 minutes, not as a separate stage. Volume and spaced repetition matter more than finishing any single book. DSA practice counts toward the "building" share of the 1:3 ratio.

### Resources

| Resource | Type | Role |
|----------|------|------|
| [Problem Solving with Algorithms and Data Structures using Python](https://runestone.academy/ns/books/published/pythonds3/index.html) | Free online book | Python-first fundamentals (D1) |
| [Grokking Algorithms, 2nd Ed (Bhargava)](https://www.manning.com/books/grokking-algorithms-second-edition) | Book | Fast visual first pass |
| [VisuAlgo](https://visualgo.net/) | Interactive visualizations | Watch structures and algorithms execute |
| [Python TimeComplexity wiki](https://wiki.python.org/moin/TimeComplexity) | Reference | Cost of `list`, `dict`, `set`, `deque` operations |
| [NeetCode Roadmap](https://neetcode.io/roadmap) and [NeetCode 150](https://neetcode.io/practice) | Curated problem list | Pattern-based practice order |
| [LeetCode](https://leetcode.com/) | Problem platform | Volume and weekly contests |
| [Algorithms (Jeff Erickson)](https://jeffe.cs.illinois.edu/teaching/algorithms/) | Free book | Rigor: recursion, DP, graphs, proofs |
| [Introduction to Algorithms, CLRS](https://mitpress.mit.edu/9780262046305/introduction-to-algorithms/) | Reference textbook | Selective depth, not cover to cover |
| [Competitive Programmer's Handbook (Laaksonen)](https://cses.fi/book/book.pdf) | Free PDF | Compact advanced techniques |
| [CSES Problem Set](https://cses.fi/problemset/) | Problem set | Classic algorithm problems with hidden tests |
| [Cracking the Coding Interview (McDowell)](https://www.crackingthecodinginterview.com/) | Book | Interview process and communication |
| [TheAlgorithms/Python](https://github.com/TheAlgorithms/Python) | GitHub repo | Reference implementations to compare against, not copy |
| [Codeforces](https://codeforces.com/) | Contest platform | Timed pressure (D4) |

### Phases

**D1: Fundamentals (alongside Stages 1 and 2)**
- [ ] Runestone: complexity analysis, recursion, sorting, searching
- [ ] Grokking Algorithms: first pass, all chapters
- [ ] Learn the cost of every built-in container operation (TimeComplexity wiki)
- [ ] NeetCode: arrays and hashing, two pointers, sliding window, stack, binary search, linked lists
- [ ] Solve 50 problems with a written complexity note on each

**D2: Trees and graphs (alongside Stages 2 and 3)**
- [ ] NeetCode: trees, tries, heap/priority queue, backtracking
- [ ] NeetCode: graphs (BFS, DFS, topological sort)
- [ ] Erickson: recursion and backtracking chapters
- [ ] Implement BST, heap, trie, and union-find from scratch with tests
- [ ] Reach 100 solved problems in total

**D3: Dynamic programming and advanced techniques (alongside Stages 3 and 4)**
- [ ] NeetCode: 1-D DP, 2-D DP, greedy, intervals
- [ ] NeetCode: advanced graphs (Dijkstra, MST), bit manipulation, math
- [ ] Erickson: dynamic programming and shortest path chapters
- [ ] Complete NeetCode 150
- [ ] Re-solve every problem you failed or needed hints for, on days 3, 7, and 21

**D4: Depth and speed (alongside Stages 4 and 5)**
- [ ] Competitive Programmer's Handbook: sorting and searching, DP, graph algorithms, range queries
- [ ] CSES: complete the Introductory, Sorting and Searching, and Dynamic Programming sections
- [ ] CLRS: read chapters on amortized analysis, graph algorithms, and NP-completeness
- [ ] Cracking the Coding Interview: behavioral and communication chapters
- [ ] 10 timed contests (LeetCode weekly or Codeforces)
- [ ] 5 mock interviews with a peer, recorded or reviewed

**Track targets**
- [ ] NeetCode 150 complete
- [ ] 100 additional medium problems
- [ ] 20 hard problems
- [ ] Solve a new medium in under 25 minutes without hints

### DSA for AI/ML Engineers

These tie the algorithm track directly to the ML stages.

| Resource | Role |
|----------|------|
| [Mining of Massive Datasets (Leskovec, Rajaraman, Ullman)](https://www.mmds.org/) | Hashing, LSH, Bloom filters, PageRank, streaming algorithms |
| [HNSW paper (Malkov & Yashunin)](https://arxiv.org/abs/1603.09320) | The graph-based nearest-neighbor index behind most vector databases |

- [ ] Implement top-k selection with a heap and use it in a beam search decoder
- [ ] Implement a trie and a BPE tokenizer (pairs with Zero to Hero in Stage 5)
- [ ] Implement k-NN with brute force and with a KD-tree, then benchmark both
- [ ] Implement a minimal HNSW-style graph search and compare recall and latency against brute force on your ChromaDB data
- [ ] Implement a Bloom filter and MinHash/LSH for near-duplicate detection
- [ ] Implement PageRank with power iteration on a sparse matrix

---

## Cracked Tier: Beyond the Core Path

Finish the core stages first. These items separate a course-completer from someone who ships and competes.

| Resource | Role |
|----------|------|
| [Dive into Deep Learning](https://d2l.ai/) | Executable DL textbook, second pass on Stage 5 with different framing |
| [Attention Is All You Need](https://arxiv.org/abs/1706.03762) | The paper behind everything in the GPT build |
| [Designing Machine Learning Systems (Chip Huyen)](https://huyenchip.com/books/) | Production ML: data, deployment, monitoring |
| [Kaggle Learn](https://www.kaggle.com/learn) and [Kaggle Competitions](https://www.kaggle.com/competitions) | Applied practice against real leaderboards |

- [ ] Reproduce one paper's headline result from scratch and document the gaps
- [ ] Finish one Kaggle competition in the top 25%
- [ ] Deploy the Stage 5 RAG app with CI, monitoring, and an evaluation set
- [ ] Write one technical post explaining something you built

**What "cracked" means here**
- [ ] Derive backpropagation by hand and match PyTorch gradients
- [ ] Build and train a small GPT without looking at reference code
- [ ] Solve most unseen LeetCode mediums inside 25 minutes
- [ ] Explain the time and space cost of every component in your own RAG pipeline

---

## Repository Layout

```
ml-roadmap/
├── README.md
├── pyproject.toml            # deps, mypy and pytest config
├── .github/workflows/ci.yml  # mypy + pytest on every PR
├── src/
│   ├── scripts/              # Stage 1 automation tools
│   ├── engine/               # Stage 2 OOP package
│   ├── mathlib/              # Stage 3 from-scratch math
│   ├── dsa/                  # DSA track solutions, one folder per topic
│   ├── ml/                   # Stage 4 pipelines
│   │   └── scratch/          # from-scratch algorithms
│   ├── dl/
│   │   ├── micrograd/        # Stage 5 autograd engine
│   │   └── gpt/              # Stage 5 GPT
│   └── apps/
│       └── rag_app/          # Stage 5 capstone
├── notebooks/
│   ├── 00_math/
│   ├── 03_math/
│   ├── 04_ml/
│   └── 05_dl/
├── tests/                    # mirrors src/ structure
└── docs/
    ├── dsa_log.md            # problem log with complexity notes and retry dates
    ├── design_notes.md
    ├── ml_report.md
    └── capstone.md
```

---

## Engineering Rules

These are strict. A stage is not complete until its deliverables follow all of them.

### 1. Daily 1:3 Theory-to-Building Ratio

For every 1 hour of reading or watching, spend 3 hours building.

- [ ] Log hours in `docs/log.md` at the end of each session
- [ ] If the ratio drifts below 1:3 for a week, cut theory scope, not building time
- [ ] No new chapter until the previous chapter has code that runs

### 2. Git Branch Hygiene

- [ ] `main` is always green and never receives direct commits
- [ ] One branch per deliverable: `stage-N/short-description`
- [ ] Commits are small and use imperative messages (`Add SVD from scratch`)
- [ ] Merge via PR after CI passes, squash on merge
- [ ] Delete branches after merge

### 3. Typing with mypy

- [ ] All code in `src/` is fully annotated
- [ ] `mypy --strict src/` passes before every PR
- [ ] No unscoped `# type: ignore`; each one needs a comment explaining why

### 4. Testing with pytest

- [ ] Every module in `src/` has a matching file in `tests/`
- [ ] `pytest` passes locally before every PR
- [ ] From-scratch implementations are tested against a reference library (NumPy, scikit-learn, PyTorch)
- [ ] Minimum 80% coverage on `src/` (`pytest --cov=src`)

### 5. DSA Practice Discipline

- [ ] Every solved problem lives in `src/dsa/<topic>/` with type hints, a complexity note in the docstring, and a pytest case covering edge cases
- [ ] Attempt each problem for 20 to 30 minutes before reading a solution
- [ ] Log failures in `docs/dsa_log.md` and re-solve on days 3, 7, and 21
- [ ] Never paste a solution you cannot rewrite from memory the next day

### Pre-PR Checklist

```bash
mypy --strict src/
pytest --cov=src --cov-fail-under=80
git status   # clean, correct branch
```

- [ ] Both commands pass
- [ ] Notebook outputs cleared or intentionally kept
- [ ] README progress dashboard updated

---

## License

MIT
