# Applied Artificial Intelligence: 9-Month University Study Guide & Progress Tracker

> **Target Audience:** Undergraduate students studying Applied AI, Data Science, or Machine Learning Engineering.  
> **Duration:** 9 Months (36 Weeks — 3 Academic Terms).  
> **Interactive Local Library:** Books cross-referenced with your local **Calibre-Web** instance (Port `8083`).  
> **Calibre-Web Direct Search:** Every book title below includes its exact **Calibre `#ID`** (e.g. `[#1025] Hands-On Machine Learning...`) so you can search directly by number or full name in Calibre-Web (`http://<server-ip>:8083` or direct URL `http://<server-ip>:8083/book/<id>`).  
> **GitHub Native:** Uses GitHub-flavoured markdown task lists (`- [ ]`). Tick off tasks as you learn, commit, and push your progress directly to GitHub.

---

## 1. The 3-Step Daily Git Loop (After One-Time Clone)

You don't need to be a Git expert to track your studies. There is a **one-time setup**, followed by a simple **3-step daily habit**:

### Day 1: One-Time Clone
Run this **only once** when you first set up your local study environment:
```bash
git clone <your-github-repo-url>
cd applied-ai-study
```

### The 3-Step Daily Study Habit
At the end of each study session (after taking notes, completing exercises, or ticking checkboxes in this guide):

```
+-----------------------------------------------------------------------------------------+
|                                  THE 3-STEP DAILY LOOP                                  |
+----------------------+------------------------------------------------------------------+
| 1. Stage Changes     | git add .                                                        |
| 2. Commit Progress   | git commit -m "<type>: <what you did>"                           |
| 3. Push to GitHub    | git push                                                         |
+----------------------+------------------------------------------------------------------+
```
> [!NOTE]
> *Multi-device tip:* If you switch between a laptop and desktop, run `git pull` at the start of your session to download your latest progress before making new changes.

### Conventional Commits (Keep It Clean & Simple)

When committing, use standard prefixes so your GitHub history is professional and organized:

* `docs:` — Ticking off items in `Study-Guide.md` or writing notes.
  ```bash
  git commit -m "docs: tick off Week 3 Pandas exercises"
  ```
* `feat:` — Adding new code or completing a milestone project.
  ```bash
  git commit -m "feat: implement gradient descent from scratch"
  ```
* `fix:` — Correcting a bug in an exercise or formula.
  ```bash
  git commit -m "fix: resolve matrix multiplication dimension error"
  ```

### Suggested Folder Layout

```text
applied-ai-study/
├── .gitignore                      # Prevents uploading large data and junk
├── README.md                       # Your personal bio and target goals
├── Study-Guide.md                  # This study guide with your ticked checkboxes
├── notes/                          # Short notes & markdown summaries per topic
│   ├── 01-math/
│   ├── 02-classical-ml/
│   ├── 03-deep-learning/
│   └── 04-llms-and-agents/
└── milestones/                     # Your 9 monthly project deliverables
    ├── m01-numpy-eda/
    ├── m02-gradient-descent-scratch/
    ├── m03-scikit-pipeline/
    ├── m04-pytorch-mlp/
    ├── m05-vision-transfer-learning/
    ├── m06-transformer-embeddings/
    ├── m07-rag-vector-search/
    ├── m08-autonomous-agent/
    └── m09-production-capstone/
```

### Essential `.gitignore`

```gitignore
.venv/
__pycache__/
*.csv
*.parquet
*.pt
*.pth
*.onnx
*.bin
.env
```

---

## 2. Master Book Index (Calibre `#ID` & Exact Titles)

All internal books are hosted in Calibre-Web at `http://<server-ip>:8083`. You can find any book instantly by typing its **#ID number** into the Calibre-Web search bar or navigating directly to `http://<server-ip>:8083/book/<id>`.

| Calibre Search ID | Exact Book Title in Calibre-Web | Author(s) | Primary Domain | Direct Local Link |
| :---: | :--- | :--- | :--- | :---: |
| **#1397** | *Python Data Science Handbook* | Jake VanderPlas | NumPy, Pandas, Matplotlib | [Open #1397](http://localhost:8083/book/1397) |
| **#1524** | *Pandas Workout* | Reuven Lerner | Data Wrangling Drills | [Open #1524](http://localhost:8083/book/1524) |
| **#827** | *A Common-Sense Guide to Data Structures and Algorithms in Python, Volume 1* | Jay Wengrow | Computational Big-O | [Open #827](http://localhost:8083/book/827) |
| **#720** | *Essential Math for AI* | Hala Nelson | Linear Algebra & Calculus | [Open #720](http://localhost:8083/book/720) |
| **#377** | *Mathematics of Machine Learning: Master Linear Algebra, Calculus, and Probability* | Tivadar Danka | ML Math & Optimization | [Open #377](http://localhost:8083/book/377) |
| **#1025** | *Hands-On Machine Learning with Scikit-Learn and PyTorch* | Aurélien Géron | Classical ML & Pipelines | [Open #1025](http://localhost:8083/book/1025) |
| **#1053** | *Deep Learning With Python, Third Edition* | Watson & Chollet | Deep Learning & Keras 3 | [Open #1053](http://localhost:8083/book/1053) |
| **#1434** | *AI and ML for Coders in Pytorch* | Laurence Moroney | PyTorch Vision & NLP | [Open #1434](http://localhost:8083/book/1434) |
| **#980** | *AI Engineering: Building Applications With Foundation Models* | Chip Huyen | Modern GenAI & RAG | [Open #980](http://localhost:8083/book/980) |
| **#1787** | *An Illustrated Guide to AI Agents* | Grootendorst & Alammar | Agents & Planning | [Open #1787](http://localhost:8083/book/1787) |
| **#1784** | *Build a Reasoning Model (From Scratch)* | Sebastian Raschka | Reasoning Models & LLMs | [Open #1784](http://localhost:8083/book/1784) |
| **#1579** | *Streamlit for Data Science* | Tyler Richards | Rapid UI Prototyping | [Open #1579](http://localhost:8083/book/1579) |
| **External** | *Mathematics for Machine Learning* | Deisenroth et al. | Cambridge University Press | [mml-book.com](https://mml-book.com) |
| **External** | *An Intro to Statistical Learning (ISLP)* | James, Witten et al. | Springer (Free Online) | [statlearning.com](https://www.statlearning.com) |
| **External** | *Build a Large Language Model (From Scratch)* | Sebastian Raschka | Manning (2024) | [manning.com](https://www.manning.com) |

---

## 3. 9-Month (36-Week) Study Roadmap & Checklist

```
+----------------------------------------------------------------------------------------------------+
|                                    9-MONTH ACCELERATED TIMELINE                                    |
+------------------------------------+----------------------------------+----------------------------+
| TERM 1 (Weeks 1–12)                | TERM 2 (Weeks 13–24)             | TERM 3 (Weeks 25–36)       |
| Foundations & Classical ML         | Deep Learning & Neural Nets      | Modern AI, Agents & Capstone|
+------------------------------------+----------------------------------+----------------------------+
| • Python & NumPy Vectorization     | • PyTorch Tensors & Autograd     | • Vector Search & RAG      |
| • Vectors, Calculus & Gradients    | • Computer Vision (CNNs/ResNets) | • Agentic ReAct Loops      |
| • Scikit-Learn Pipelines & Tuning  | • NLP, Embeddings & Transformers | • MLOps, Docker & Capstone |
+------------------------------------+----------------------------------+----------------------------+
```

---

### 🚀 Master 36-Week Progress Tracker (By Month)
> **Quick View:** Tick off each week as you progress, and tick off the month when its milestone deliverable is shipped. Track your complete journey at a glance without scrolling through the full document!

- [ ] **Month 1: Python Data Stack & Data Wrangling** &rarr; [`milestones/m01-numpy-eda/`](#month-1-python-data-science-stack--data-wrangling-weeks-1-4)
  - [ ] **Week 1:** Environment Setup & The Git Loop (~18 pages)
  - [ ] **Week 2:** Vectorized Computing with NumPy (~42 pages)
  - [ ] **Week 3:** Data Wrangling with Pandas (~36 pages + 5 targeted drills)
  - [ ] **Week 4:** Computational Efficiency & **Milestone 1 Deliverable** (~31 pages)
- [ ] **Month 2: Applied Mathematics, Calculus & Optimization** &rarr; [`milestones/m02-gradient-descent-scratch/`](#month-2-applied-mathematics-calculus--optimization-weeks-5-8)
  - [ ] **Week 5:** Linear Algebra & Vector Geometry (~26 pages)
  - [ ] **Week 6:** Matrix Decompositions & Eigenvalues (PCA) (~28 pages)
  - [ ] **Week 7:** Multivariable Calculus & Gradient Vectors (~30 pages)
  - [ ] **Week 8:** Optimization from Scratch & **Milestone 2 Deliverable** (~24 pages)
- [ ] **Month 3: Classical Machine Learning & Validation Rigor** &rarr; [`milestones/m03-scikit-pipeline/`](#month-3-classical-machine-learning--validation-rigor-weeks-9-12)
  - [ ] **Week 9:** Linear Models & Regularization (Ridge/Lasso) (~32 pages)
  - [ ] **Week 10:** Decision Trees, Random Forests & Ensembles (XGBoost) (~30 pages)
  - [ ] **Week 11:** Validation Discipline & Leak-Free Pipelines (~35 pages)
  - [ ] **Week 12:** Term 1 Capstone & **Milestone 3 Deliverable** (Streamlit GUI) (~28 pages)
- [ ] **Month 4: Neural Networks from Scratch & PyTorch Foundations** &rarr; [`milestones/m04-pytorch-mlp/`](#month-4-neural-networks-from-scratch--pytorch-foundations-weeks-13-16)
  - [ ] **Week 13:** Perceptrons & Backpropagation Theory (~30 pages)
  - [ ] **Week 14:** PyTorch Tensors, CUDA & Autograd (~26 pages)
  - [ ] **Week 15:** Training Loops, Losses & Optimizers (~28 pages)
  - [ ] **Week 16:** Custom PyTorch Architecture & **Milestone 4 Deliverable** (~18 pages)
- [ ] **Month 5: Computer Vision, Convolutions & Transfer Learning** &rarr; [`milestones/m05-vision-transfer-learning/`](#month-5-computer-vision-convolutions--transfer-learning-weeks-17-20)
  - [ ] **Week 17:** Convolutions & Spatial Feature Hierarchies (~26 pages)
  - [ ] **Week 18:** Modern CNN Backbones & Residual Connections (ResNet) (~24 pages)
  - [ ] **Week 19:** Transfer Learning & Data Augmentation (~28 pages)
  - [ ] **Week 20:** Vision Capstone & **Milestone 5 Deliverable** (Grad-CAM) (~16 pages)
- [ ] **Month 6: Sequence Modeling, Attention & Transformers** &rarr; [`milestones/m06-transformer-embeddings/`](#month-6-sequence-modeling-attention--transformers-weeks-21-24)
  - [ ] **Week 21:** Text Preprocessing & Subword Tokenization (BPE) (~25 pages)
  - [ ] **Week 22:** Word & Sentence Embeddings (Cosine Similarity) (~28 pages)
  - [ ] **Week 23:** The Transformer Architecture & Self-Attention Equations (~32 pages)
  - [ ] **Week 24:** Term 2 Capstone & **Milestone 6 Deliverable** (Attention Module) (~15 pages)
- [ ] **Month 7: Vector Databases, RAG & Semantic Retrieval** &rarr; [`milestones/m07-rag-vector-search/`](#month-7-vector-databases-rag--semantic-retrieval-weeks-25-28)
  - [ ] **Week 25:** The Modern AI Engineering Stack (~26 pages)
  - [ ] **Week 26:** Vector Databases & Chunking Strategies (ChromaDB) (~32 pages)
  - [ ] **Week 27:** Advanced RAG Patterns & Hybrid Search (Dense + BM25) (~30 pages)
  - [ ] **Week 28:** RAG Evaluation & **Milestone 7 Deliverable** (Faithfulness Evals) (~28 pages)
- [ ] **Month 8: Autonomous Agents & Reasoning Loops** &rarr; [`milestones/m08-autonomous-agent/`](#month-8-autonomous-agents--reasoning-loops-weeks-29-32)
  - [ ] **Week 29:** Agentic Foundations & The ReAct Loop (~30 pages)
  - [ ] **Week 30:** Function Calling & Tool Integration (JSON Schemas / MCP) (~28 pages)
  - [ ] **Week 31:** Reasoning Tokens & Advanced Prompting (Inference Scaling) (~32 pages)
  - [ ] **Week 32:** Autonomous Research Agent & **Milestone 8 Deliverable** (~22 pages)
- [ ] **Month 9: Production MLOps, Containerization & Shipped Capstone** &rarr; [`milestones/m09-production-capstone/`](#month-9-production-mlops-containerization--shipped-capstone-weeks-33-36)
  - [ ] **Week 33:** Microservices & API Design (Async FastAPI & SSE Streaming) (~24 pages)
  - [ ] **Week 34:** Containerization with Docker & Compose Orchestration (~20 pages)
  - [ ] **Week 35:** Portfolio Polish, Technical Writing & Mermaid Architecture (~15 pages)
  - [ ] **Week 36:** Final Capstone Cloud Deployment & **Milestone 9 Shipped 🚀**

---

### TERM 1: Foundations, Math & Classical Machine Learning (Months 1–3)

#### Month 1: Python Data Science Stack & Data Wrangling (Weeks 1–4)
- [ ] **Month 1 Complete: All 4 Weeks Finished & Milestone 1 Delivered**
*Goal: Set up your environment, master the 3-step Git loop, and eliminate slow Python for-loops using NumPy and Pandas.*

> [!TIP]
> **Curated Reading Strategy:** Do **not** attempt to read all 3 books cover-to-cover! 
> - **[#1397] *Python Data Science Handbook*** is your **core conceptual textbook**.
> - **[#1524] *Pandas Workout*** is an **exercise gym** — do only the 5 targeted drills listed below.
> - **[#827] *Common-Sense Guide to DSA*** is your **mental model for efficiency** — read only Chapters 1 and 3 to understand Big-O.
> Total reading is streamlined to ~30 pages per week (~20 minutes/day).

- [ ] **Week 1: Environment Setup & The Git Loop (~18 pages)**
  - [ ] Set up Python virtual environment (`.venv`), VS Code, and Jupyter extension
  - [ ] Initialize GitHub repository with `.gitignore` and `Study-Guide.md`
  - [ ] Practice the basic loop: `git add .`, `git commit -m "docs: setup repo"`, `git push`
  - [ ] Read: **[#1397] *Python Data Science Handbook***:
    - [ ] **Ch 1:** *Getting Started in IPython and Jupyter* (Focus: Tab completion, `?` docstrings, keyboard shortcuts)
    - [ ] **Ch 2:** *Enhanced Interactive Features* (Focus: `%timeit` magic, shell commands `!ls`/`!pwd`)
    - *(Skip Ch 3 for now: Memory profiling is premature for Week 1)*
- [ ] **Week 2: Vectorized Computing with NumPy (~42 pages)**
  - [ ] Read: **[#1397] *Python Data Science Handbook***:
    - [ ] **Ch 4:** *Understanding Data Types in Python* (Why fixed-type NumPy arrays eliminate Python list overhead)
    - [ ] **Ch 5:** *The Basics of NumPy Arrays* (Indexing, multidimensional slicing, `.reshape()`, views vs copies)
    - [ ] **Ch 6:** *Computation on NumPy Arrays: Universal Functions* (Why loops are slow, vector arithmetic)
    - [ ] **Ch 8:** *Computation on Arrays: Broadcasting* (Broadcasting rules — vital for machine learning tensors!)
    - *(Skip Ch 7, 9–12 for now: Aggregations and indexing are handled in Ch 5/6 and Pandas)*
  - [ ] Practice: Write matrix multiplication and normalisation using vectorized NumPy without a single `for` loop
  - [ ] Commit: `git commit -m "feat: complete numpy vectorization exercises"`
- [ ] **Week 3: Data Wrangling with Pandas (~36 pages + 5 targeted drills)**
  - [ ] Read: **[#1397] *Python Data Science Handbook***:
    - [ ] **Ch 13:** *Introducing Pandas Objects* (Series, DataFrames, Index objects)
    - [ ] **Ch 14:** *Data Indexing and Selection* (`.loc`, `.iloc`, boolean masking)
    - [ ] **Ch 18:** *Aggregation and Grouping* (`.groupby()`, `.agg()`, `.transform()`)
  - [ ] Solve **5 Targeted Drills** in **[#1524] *Pandas Workout*** (Do NOT do all 50 exercises!):
    - [ ] **Exercise 1** (p. 96): *Test scores* (Series filtering)
    - [ ] **Exercise 2** (p. 137): *Scaling test scores* (Vector operations on Series)
    - [ ] **Exercise 8** (p. 232): *Net revenue* (Creating calculated DataFrame columns)
    - [ ] **Exercise 15** (p. 410): *Weird taxi rides* (Handling missing/malformed CSV data)
    - [ ] **Exercise 29** (p. 759): *Longest taxi rides* (`groupby` aggregations and sorting)
  - [ ] Commit: `git commit -m "docs: complete 5 pandas workout drills"`
- [ ] **Week 4: Computational Efficiency & Milestone 1 (~31 pages)**
  - [ ] Read: **[#827] *A Common-Sense Guide to Data Structures and Algorithms in Python, Vol 1***:
    - [ ] **Ch 1:** *Why Data Structures Matter* (How arrays store data in memory: Read, Search, Insert, Delete)
    - [ ] **Ch 3:** *O Yes! Big O Notation* (Understanding $O(1)$ constant time vs $O(N)$ linear time vs $O(N^2)$ quadratic time)
    - *(Skip Ch 2, 4–20: Sorting algorithms and tree/graph implementations belong in CS theory, not Month 1 AI)*
  - [ ] **Deliverable: Milestone 1** — Clean, transform, and visualize an untidy multi-table Kaggle dataset in `milestones/m01-numpy-eda/`.
  - [ ] Commit & Push: `git add . && git commit -m "feat(m01): ship exploratory data analysis project" && git push`

---

#### Month 2: Applied Mathematics, Calculus & Optimization (Weeks 5–8)
- [ ] **Month 2 Complete: All 4 Weeks Finished & Milestone 2 Delivered**
*Goal: Understand the geometry of linear transformations and code gradient descent from first principles.*

> [!TIP]
> **Curated Reading Strategy:** Do **not** attempt to read all 700+ pages of math proofs!
> - **[#720] *Essential Math for AI*** is your **core intuitive textbook** — read the visual, geometric explanations applied directly to code.
> - **[#377] *Mathematics of Machine Learning*** is your **deep-dive reference** — consult *only* targeted sections on practical vector algebra and gradient descent. Skip abstract lemmas, topology proofs, and vector space axioms.
> Total reading is streamlined to ~25–30 pages per week (~20 minutes/day).

- [ ] **Week 5: Linear Algebra & Vector Geometry (~26 pages)**
  - [ ] Read: **[#720] *Essential Math for AI***:
    - [ ] **Ch 2:** *Data, Data, Data* — Focus on sections: *Random Variables*, *Joint Distributions*, *Covariance and Correlation*, and vector data representations.
  - [ ] Read: **[#377] *Mathematics of Machine Learning***:
    - [ ] **Ch 1:** *Vectors and Vector Spaces* — Section: *Vectors in practice* (p. 55–65: Dot products, angles, vector projections).
    - *(Skip [#377] formal vector space axioms p. 33–54: Abstract algebra theory is not needed to build AI models)*
  - [ ] Commit: `git commit -m "docs: notes on vector projections and dot products"`
- [ ] **Week 6: Matrix Decompositions & Eigenvalues (~28 pages)**
  - [ ] Read: **[#720] *Essential Math for AI***:
    - [ ] **Ch 6:** *Singular Value Decomposition* — First 20 pages (Geometric intuition of SVD and Principal Component Analysis (PCA) as an orthogonal basis transformation).
  - [ ] Read: **[#377] *Mathematics of Machine Learning***:
    - [ ] **Ch 6:** *Eigenvalues and Eigenvectors* — Section: *Eigenvalues of matrices* (p. 219–226: How transformations stretch coordinate space).
    - *(Skip [#377] Ch 7–8: QR algorithms and graph Frobenius normal forms are out of scope)*
  - [ ] Practice: Implement 2D/3D PCA dimensionality reduction using NumPy matrix multiplication.
  - [ ] Commit: `git commit -m "feat: implement PCA dimensionality reduction in numpy"`
- [ ] **Week 7: Multivariable Calculus & Gradient Vectors (~30 pages)**
  - [ ] Read: **[#720] *Essential Math for AI***:
    - [ ] **Ch 3:** *Fitting Functions to Data* (Loss functions, MSE, analytical vs numerical solutions).
    - [ ] **Ch 4:** *Optimization for Neural Networks* (Gradients, slope tangents, and the multivariable chain rule).
  - [ ] Read: **[#377] *Mathematics of Machine Learning***:
    - [ ] **Ch 16:** *Derivatives and Gradients* (p. 477–492: Partial derivatives, gradient vectors, and tangent hyperplanes).
    - *(Skip [#377] Ch 9–11 real analysis topology and limits)*
  - [ ] Commit: `git commit -m "docs: calculus derivatives and gradient derivations"`
- [ ] **Week 8: Optimization from Scratch & Milestone 2 (~24 pages)**
  - [ ] Read: **[#377] *Mathematics of Machine Learning***:
    - [ ] **Ch 17:** *Optimization in Multiple Variables* (p. 503–516: Gradient descent algorithm, step sizes/learning rates, local minima vs saddle points).
  - [ ] Read: **[#720] *Essential Math for AI***:
    - [ ] **Ch 4:** Optimization algorithms — Stochastic Gradient Descent (SGD) intuition and learning rate schedules.
  - [ ] **Deliverable: Milestone 2** — Code a Batch and Stochastic Gradient Descent (SGD) optimizer from scratch in NumPy in `milestones/m02-gradient-descent-scratch/`. Plot the 3D trajectory across a loss surface.
  - [ ] Commit & Push: `git add . && git commit -m "feat(m02): pure numpy gradient descent and 3d loss plot" && git push`

---

#### Month 3: Classical Machine Learning & Validation Rigor (Weeks 9–12)
- [ ] **Month 3 Complete: All 4 Weeks Finished & Milestone 3 Delivered**
*Goal: Master supervised algorithms, cross-validation discipline, and leak-free Scikit-Learn pipelines.*

> [!TIP]
> **Curated Reading Strategy:** Do **not** attempt to read all 1,400+ pages of Géron!
> - **[#1025] *Hands-On Machine Learning*** is your **core ML handbook** — read targeted sections on supervised algorithms, validation metrics, and data pipelines (~30 pages/week).
> - **[#1579] *Streamlit for Data Science*** is your **UI prototyping guide** — read only Chapters 1 and 4 to wire your model into an interactive frontend.
> Total reading is streamlined to ~28–32 pages per week (~20 minutes/day).

- [ ] **Week 9: Linear Models & Regularization (~32 pages)**
  - [ ] Read: **[#1025] *Hands-On Machine Learning with Scikit-Learn and PyTorch***:
    - [ ] **Ch 1:** *The Machine Learning Landscape* (p. 26–50: Supervised vs unsupervised, batch vs online learning, overfitting, underfitting, no-free-lunch theorem).
    - [ ] **Ch 4:** *Training Models* — Sections on Linear Regression, Normal Equation, Ridge ($L_2$) and Lasso ($L_1$) regularization intuition (p. 246–265).
    - *(Skip Ch 4's polynomial derivations and softmax math for now)*
  - [ ] Commit: `git commit -m "feat: linear and logistic regression experiments"`
- [ ] **Week 10: Decision Trees, Random Forests & Ensembles (~30 pages)**
  - [ ] Read: **[#1025] *Hands-On Machine Learning with Scikit-Learn and PyTorch***:
    - [ ] **Ch 5:** *Support Vector Machines* — Linear SVM classification and soft-margin intuition (p. 308–320).
    - [ ] **Ch 6:** *Decision Trees* — Gini impurity vs Entropy, tree pruning, regression trees (p. 329–342).
    - [ ] **Ch 7:** *Ensemble Learning and Random Forests* — Voting classifiers, Bagging, Random Forests, and Gradient Boosting (XGBoost) overview (p. 362–378).
  - [ ] Commit: `git commit -m "feat: ensemble models and feature importance comparison"`
- [ ] **Week 11: Validation Discipline & Leak-Free Pipelines (~35 pages)**
  - [ ] Read: **[#1025] *Hands-On Machine Learning with Scikit-Learn and PyTorch***:
    - [ ] **Ch 2:** *End-to-End Machine Learning Project* — Specific section: *Prepare the Data for Machine Learning Algorithms* (p. 130–155: Scikit-Learn `Pipeline`, `ColumnTransformer`, imputers, scalers, avoiding data snooping/leakage).
    - [ ] **Ch 3:** *Classification* — Precision, Recall, $F_1$ score, ROC-AUC curve, confusion matrix (p. 190–210).
    - *(Skip Ch 2's geographical clustering and exploratory plotting: already mastered in Month 1)*
  - [ ] Commit: `git commit -m "feat: leak-free scikit-learn preprocessing pipeline"`
- [ ] **Week 12: Term 1 Capstone & Milestone 3 (~28 pages)**
  - [ ] Read: **[#1579] *Streamlit for Data Science***:
    - [ ] **Ch 1:** *An Introduction to Streamlit* (p. 21–38: Core widgets, sliders, forms, reactive data flow).
    - [ ] **Ch 4:** *Machine Learning and AI with Streamlit* (p. 95–115: Loading pickled Scikit-Learn pipelines, making real-time user predictions).
    - *(Skip Ch 2–3, 5–12: Database connections, custom JS components, and enterprise hosting are out of scope)*
  - [ ] **Deliverable: Milestone 3** — End-to-end classifier with full pipeline, cross-validation, and an interactive Streamlit frontend in `milestones/m03-scikit-pipeline/`.
  - [ ] Commit & Push: `git add . && git commit -m "feat(m03): complete term 1 scikit-learn streamlit app" && git push`

---

### TERM 2: Deep Learning & Neural Frameworks (Months 4–6)

#### Month 4: Neural Networks from Scratch & PyTorch Foundations (Weeks 13–16)
- [ ] **Month 4 Complete: All 4 Weeks Finished & Milestone 4 Delivered**
*Goal: Move from linear models to computational graphs, backpropagation, and PyTorch `nn.Module`.*

> [!TIP]
> **Curated Reading Strategy:** Do **not** get bogged down in framework confusion!
> - **[#1434] *AI and ML for Coders in PyTorch*** is your **practical PyTorch code manual** — learn syntax, tensor manipulations, `nn.Module`, and the standard training loop.
> - **[#1053] *Deep Learning With Python*** is your **conceptual mental model** — read Chollet's world-class visual explanations of computational graphs and loss surfaces.
> Total reading is streamlined to ~25–30 pages per week (~20 minutes/day).

- [ ] **Week 13: Perceptrons & Backpropagation Theory (~30 pages)**
  - [ ] Read: **[#1053] *Deep Learning With Python, Third Edition***:
    - [ ] **Ch 2:** *The mathematical building blocks of neural networks* (p. 16–45: Tensors, tensor operations, geometric interpretation of deep learning, gradient-based optimization).
    - *(Skip Ch 1: General historical AI overview)*
  - [ ] Practice: Work through the forward pass, loss calculation, and backward chain-rule propagation for a 2-layer perceptron by hand.
  - [ ] Commit: `git commit -m "docs: backpropagation mathematical derivation"`
- [ ] **Week 14: PyTorch Tensors, CUDA & Autograd (~26 pages)**
  - [ ] Read: **[#1434] *AI and ML for Coders in PyTorch***:
    - [ ] **Ch 1:** *Introduction to PyTorch* (Tensors, dimensions, slicing, device placement with `to(device)`, and computational graphs via `autograd`).
    - [ ] **Ch 4:** *Using Data with PyTorch* (Dataset loaders, batching, and shuffling with `torch.utils.data.DataLoader`).
  - [ ] Commit: `git commit -m "feat: pytorch autograd and computational graph basics"`
- [ ] **Week 15: Training Loops, Losses & Optimizers (~28 pages)**
  - [ ] Read: **[#1053] *Deep Learning With Python, Third Edition***:
    - [ ] **Ch 5:** *Fundamentals of machine learning* (p. 136–160: Generalization, underfitting vs overfitting, validation splits, weight regularization ($L_1$/$L_2$), and dropout).
  - [ ] Read: **[#1434] *AI and ML for Coders in PyTorch***:
    - [ ] **Ch 2:** Building neural architectures with `torch.nn.Module`, writing the standard PyTorch training loop (`optimizer.zero_grad()`, `loss.backward()`, `optimizer.step()`).
  - [ ] Commit: `git commit -m "feat: reusable pytorch training and evaluation loop"`
- [ ] **Week 16: Custom PyTorch Architecture & Milestone 4 (~18 pages + Milestone 4)**
  - [ ] Read: **[#1053] *Deep Learning With Python, Third Edition***:
    - [ ] **Ch 5.3–5.4:** Hyperparameter tuning, learning rate schedules, early stopping, and saving model checkpoints (`torch.save()`).
  - [ ] **Deliverable: Milestone 4** — Build a multi-layer deep neural network in `milestones/m04-pytorch-mlp/` with modular dataset loaders (`torch.utils.data.DataLoader`), training/validation loss curves, and early stopping.
  - [ ] Commit & Push: `git add . && git commit -m "feat(m04): custom pytorch mlp with training loop" && git push`

---

#### Month 5: Computer Vision, Convolutions & Transfer Learning (Weeks 17–20)
- [ ] **Month 5 Complete: All 4 Weeks Finished & Milestone 5 Delivered**
*Goal: Master spatial feature extraction, convolutional backbones, and transfer learning.*

> [!TIP]
> **Curated Reading Strategy:** Do **not** read all 650 pages of vision architectures!
> - **[#1053] *Deep Learning With Python*** provides the clearest visual explanations of convolutional filters, spatial pooling, and ResNet skip connections.
> - **[#1434] *AI and ML for Coders in PyTorch*** provides the practical code for `torchvision.models` and data augmentation.
> Total reading is streamlined to ~26–30 pages per week (~20 minutes/day).

- [ ] **Week 17: Convolutions & Spatial Feature Hierarchies (~26 pages)**
  - [ ] Read: **[#1053] *Deep Learning With Python, Third Edition***:
    - [ ] **Ch 8:** *Image classification* (p. 231–255: Why ConvNets beat MLPs for images, convolution operations, kernels/filters, strides, and pooling layers).
  - [ ] Read: **[#1434] *AI and ML for Coders in PyTorch***:
    - [ ] **Ch 3:** *Going Beyond the Basics: Detecting Features in Images* (Implementing `nn.Conv2d` and `nn.MaxPool2d` in PyTorch).
  - [ ] Commit: `git commit -m "feat: conv2d layer experiments and feature maps"`
- [ ] **Week 18: Modern CNN Backbones & Residual Connections (~24 pages)**
  - [ ] Read: **[#1053] *Deep Learning With Python, Third Edition***:
    - [ ] **Ch 9:** *ConvNet architecture patterns* (p. 268–283: Modularity, residual skip connections, batch normalization, why ResNet solves the vanishing gradient problem).
    - *(Skip Ch 11–12: Segmentation and YOLO object detection are specialized vision tasks, not needed for classification transfer learning)*
  - [ ] Commit: `git commit -m "docs: notes on resnet skip connections"`
- [ ] **Week 19: Transfer Learning & Data Augmentation (~28 pages)**
  - [ ] Read: **[#1053] *Deep Learning With Python, Third Edition***:
    - [ ] **Ch 8.3:** *Using a pretrained model* (p. 256–267: Feature extraction vs fine-tuning, freezing convolutional weights).
  - [ ] Read: **[#1434] *AI and ML for Coders in PyTorch***:
    - [ ] **Ch 4:** Image data pipelines with `torchvision.transforms` (resize, crop, horizontal flip, normalization).
  - [ ] Practice: Freeze pretrained `torchvision.models.resnet18` backbone, replace final FC classification head, and train on custom dataset.
  - [ ] Commit: `git commit -m "feat: fine-tuning pretrained vision backbone"`
- [ ] **Week 20: Vision Capstone & Milestone 5 (~16 pages + Milestone 5)**
  - [ ] Read: **[#1053] *Deep Learning With Python, Third Edition***:
    - [ ] **Ch 10:** *Interpreting what ConvNets learn* (p. 299–305: Visualizing class activation maps / Grad-CAM heatmaps).
  - [ ] **Deliverable: Milestone 5** — Fine-tune a pretrained ResNet or EfficientNet on a specialized image dataset in `milestones/m05-vision-transfer-learning/`. Include validation metrics, confusion matrix, and Grad-CAM interpretability heatmaps.
  - [ ] Commit & Push: `git add . && git commit -m "feat(m05): vision transfer learning classifier" && git push`

---

#### Month 6: Sequence Modeling, Attention & Transformers (Weeks 21–24)
- [ ] **Month 6 Complete: All 4 Weeks Finished & Milestone 6 Delivered**
*Goal: Demystify word tokenization, vector embeddings, and the self-attention mechanism.*

> [!TIP]
> **Curated Reading Strategy:** Do **not** waste time on legacy NLP models!
> - Skip obsolete Recurrent Neural Networks (RNNs) and LSTMs — modern AI has completely transitioned to Transformer attention mechanisms.
> - **[#1053] *Deep Learning With Python*** Ch 14–15 is your core textbook for modern tokenization and Transformer blocks.
> - **[#1787] *An Illustrated Guide to AI Agents*** Ch 2 gives the visual step-by-step breakdown of self-attention dot products ($Q, K, V$).
> Total reading is streamlined to ~28–30 pages per week (~20 minutes/day).

- [ ] **Week 21: Text Preprocessing & Subword Tokenization (~25 pages)**
  - [ ] Read: **[#1053] *Deep Learning With Python, Third Edition***:
    - [ ] **Ch 14:** *Text classification* (p. 381–405: Text vectorization, vocabulary indexing, subword tokenization, WordPiece/Byte-Pair Encoding (BPE) vs word-level tokenization).
    - *(Skip traditional RNN/LSTM sections: Focus purely on tokenization and embeddings)*
  - [ ] Commit: `git commit -m "feat: bpe subword tokenizer experiment"`
- [ ] **Week 22: Word & Sentence Embeddings (~28 pages)**
  - [ ] Read: **[#1025] *Hands-On Machine Learning with Scikit-Learn and PyTorch***:
    - [ ] **Ch 14:** *Natural Language Processing with Attention* (p. 885–905: Vector embeddings, semantic distance, cosine similarity, high-dimensional representation).
  - [ ] Practice: Generate sentence embeddings with Hugging Face `sentence-transformers` and compute cosine similarity rankings.
  - [ ] Commit: `git commit -m "feat: sentence embeddings and cosine similarity search"`
- [ ] **Week 23: The Transformer Architecture & Self-Attention (~32 pages)**
  - [ ] Read: **[#1053] *Deep Learning With Python, Third Edition***:
    - [ ] **Ch 15:** *Language models and the Transformer* (p. 421–445: Self-attention mechanism, multi-head attention, positional encoding, residual connections).
  - [ ] Read: **[#1787] *An Illustrated Guide to AI Agents***:
    - [ ] **Ch 2:** *Large Language Models* — Section: *How Self-Attention Works* (Visual step-by-step breakdown of Query, Key, and Value dot-product matrices).
  - [ ] Derive Scaled Dot-Product Attention:
    $$\text{Attention}(Q, K, V) = \text{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right)V$$
  - [ ] Commit: `git commit -m "docs: self-attention mathematical breakdown"`
- [ ] **Week 24: Term 2 Capstone & Milestone 6 (~15 pages + Milestone 6)**
  - [ ] Read: **[#1053] *Deep Learning With Python, Third Edition***:
    - [ ] **Ch 15.4:** Classification with a pretrained Transformer encoder (p. 454–465).
  - [ ] **Deliverable: Milestone 6** — Implement multi-head self-attention from scratch in PyTorch in `milestones/m06-transformer-embeddings/`, and build a semantic document search pipeline using dense vector embeddings.
  - [ ] Commit & Push: `git add . && git commit -m "feat(m06): multi-head attention module in pytorch" && git push`

---

### TERM 3: Modern AI Engineering, Agents & Shipped Capstone (Months 7–9)

#### Month 7: Vector Databases, RAG & Semantic Retrieval (Weeks 25–28)
- [ ] **Month 7 Complete: All 4 Weeks Finished & Milestone 7 Delivered**
*Goal: Architect scalable Retrieval-Augmented Generation (RAG) systems over private knowledge bases.*

> [!TIP]
> **Curated Reading Strategy:** Do **not** read all 1,096 pages of Chip Huyen's book!
> - **[#980] *AI Engineering*** is the gold standard for foundation model systems, but we read **only targeted chapters on RAG, Vector Search, and Evaluation** (Ch 1, 4, and 6).
> - **[#1787] *An Illustrated Guide to AI Agents*** Ch 4 provides the visual architecture of chunking, indexing, and Agentic RAG.
> Total reading is streamlined to ~28–32 pages per week (~20 minutes/day).

- [ ] **Week 25: The Modern AI Engineering Stack (~26 pages)**
  - [ ] Read: **[#980] *AI Engineering: Building Applications With Foundation Models***:
    - [ ] **Ch 1:** *Introduction to Building AI Applications with Foundation Models* (p. 33–55: Foundation model lifecycle, prompting vs fine-tuning vs RAG trade-offs, token economics, latency considerations).
    - *(Skip Ch 2 pre-training infrastructure clusters: out of scope for application engineers)*
  - [ ] Commit: `git commit -m "docs: foundation model engineering stack overview"`
- [ ] **Week 26: Vector Databases & Chunking Strategies (~32 pages)**
  - [ ] Read: **[#980] *AI Engineering: Building Applications With Foundation Models***:
    - [ ] **Ch 6:** *RAG and Agents* — Part 1: Retrieval Systems (p. 540–575: Chunking strategies — recursive character vs sentence-based, embedding generation, vector databases like ChromaDB/FAISS, cosine vs dot product indexing).
  - [ ] Read: **[#1787] *An Illustrated Guide to AI Agents***:
    - [ ] **Ch 4:** *Memory* — Section: *Long-Term Memory and Retrieval-Augmented Generation*.
  - [ ] Commit: `git commit -m "feat: document chunking and chromadb vector indexing"`
- [ ] **Week 27: Advanced RAG Patterns & Hybrid Search (~30 pages)**
  - [ ] Read: **[#980] *AI Engineering: Building Applications With Foundation Models***:
    - [ ] **Ch 6:** *RAG and Agents* — Part 2: Advanced Retrieval (p. 576–605: Hybrid search combining dense embeddings + BM25 keyword matching, cross-encoder rerankers, contextual compression).
  - [ ] Commit: `git commit -m "feat: hybrid dense-sparse search pipeline"`
- [ ] **Week 28: RAG Evaluation & Milestone 7 (~28 pages + Milestone 7)**
  - [ ] Read: **[#980] *AI Engineering: Building Applications With Foundation Models***:
    - [ ] **Ch 4:** *Evaluate AI Systems* (p. 339–365: Automated RAG metrics — Faithfulness, Answer Relevancy, Context Recall, LLM-as-a-judge).
  - [ ] Read: **[#1787] *An Illustrated Guide to AI Agents***:
    - [ ] **Ch 7:** *Evaluating Agents* — Section: *Building a simple evaluator* (Exact match, programmatic checks, rubric evaluation).
  - [ ] **Deliverable: Milestone 7** — End-to-end RAG question-answering assistant over custom documentation in `milestones/m07-rag-vector-search/` with hybrid search, rerankers, and an automated evaluation test suite.
  - [ ] Commit & Push: `git add . && git commit -m "feat(m07): complete rag system with evaluation suite" && git push`

---

#### Month 8: Autonomous Agents & Reasoning Loops (Weeks 29–32)
- [ ] **Month 8 Complete: All 4 Weeks Finished & Milestone 8 Delivered**
*Goal: Build agentic systems capable of reasoning, calling external tools, and executing multi-step plans.*

> [!TIP]
> **Curated Reading Strategy:** Do **not** attempt to train reasoning models from scratch!
> - **[#1787] *An Illustrated Guide to AI Agents*** is your **core visual textbook** for tool calling, memory architectures, and multi-step reasoning loops.
> - **[#1784] *Build a Reasoning Model (From Scratch)***: Read **only Chapter 1 and Chapter 4** to understand inference-time scaling and self-refinement. Do NOT attempt the 400-page reinforcement learning / GRPO pretraining!
> Total reading is streamlined to ~28–32 pages per week (~20 minutes/day).

- [ ] **Week 29: Agentic Foundations & The ReAct Loop (~30 pages)**
  - [ ] Read: **[#1787] *An Illustrated Guide to AI Agents***:
    - [ ] **Ch 1:** *Introduction* (The Anatomy of an AI Agent: Brain, Tools, Memory, Planning).
    - [ ] **Ch 6:** *Planning and Reflection* (The ReAct pattern: Reason $\rightarrow$ Act $\rightarrow$ Observe, task decomposition, action sequencing).
  - [ ] Practice: Implement a minimal ReAct loop in raw Python with structured string parsing.
  - [ ] Commit: `git commit -m "feat: basic react prompt loop implementation"`
- [ ] **Week 30: Function Calling & Tool Integration (~28 pages)**
  - [ ] Read: **[#1787] *An Illustrated Guide to AI Agents***:
    - [ ] **Ch 5:** *Tool Usage, Learning, and Protocols* (Structured function calling, JSON schema generation, safe execution sandbox, error handling, Model Context Protocol (MCP) overview).
  - [ ] Practice: Implement custom tools (e.g. calculator, python runner, API fetcher) with Pydantic schema validation.
  - [ ] Commit: `git commit -m "feat: json schema tool calling integration"`
- [ ] **Week 31: Reasoning Tokens & Advanced Prompting (~32 pages)**
  - [ ] Read: **[#1784] *Build a Reasoning Model (From Scratch)***:
    - [ ] **Ch 1:** *Understanding reasoning models* (p. 25–41: Why reasoning models output thought chains before answering, test-time compute vs training-time compute).
    - [ ] **Ch 4:** *Improving reasoning with inference-time scaling* (p. 118–145: Best-of-N sampling, self-consistency, verification).
    - *(Skip [#1784] Ch 6–8: Pre-training reasoning models with RL/GRPO is research-level engineering, not needed for applied agent orchestration)*
  - [ ] Read: **[#1787] *An Illustrated Guide to AI Agents***:
    - [ ] **Ch 3:** *Reasoning Large Language Models* (Inference scaling and reflection loops).
  - [ ] Commit: `git commit -m "docs: notes on test-time compute and reasoning tokens"`
- [ ] **Week 32: Autonomous Research Agent & Milestone 8 (~22 pages + Milestone 8)**
  - [ ] Read: **[#1787] *An Illustrated Guide to AI Agents***:
    - [ ] **Ch 6:** *Agents That Continuously Improve* (Self-Refine, Reflexion, trajectory evaluation).
  - [ ] **Deliverable: Milestone 8** — Build a multi-tool autonomous researcher agent in `milestones/m08-autonomous-agent/` that queries external APIs, validates intermediate steps, handles tool errors, and synthesizes structured markdown reports.
  - [ ] Commit & Push: `git add . && git commit -m "feat(m08): autonomous research agent with api tool use" && git push`

---

#### Month 9: Production MLOps, Containerization & Shipped Capstone (Weeks 33–36)
- [ ] **Month 9 Complete: All 4 Weeks Finished & Milestone 9 Delivered**
*Goal: Package, containerize, and deploy a full-stack applied AI product with live documentation.*

> [!TIP]
> **Curated Reading Strategy:** Focus on shipping code and infrastructure!
> - Reading is strictly minimized to ~15–20 pages per week (~15 minutes/day) so you can spend 80% of your time packaging, containerizing, and polishing your final capstone codebase.
> - **[#980] *AI Engineering***: Read **only Chapter 9** (Inference optimization, streaming SSE) and **Chapter 10** (Architecture & logging).
> Total reading is streamlined to ~18–22 pages per week.

- [ ] **Week 33: Microservices & API Design (~24 pages)**
  - [ ] Read: **[#980] *AI Engineering: Building Applications With Foundation Models***:
    - [ ] **Ch 9:** *Inference Optimization* (p. 851–875: Server-Sent Events (SSE) streaming responses, async generation, latency vs throughput trade-offs).
  - [ ] Expose models and agents through asynchronous FastAPI (`async def`) endpoints with Pydantic validation schemas and streaming responses.
  - [ ] Commit: `git commit -m "feat: fastapi inference endpoints with pydantic validation"`
- [ ] **Week 34: Containerization with Docker (~20 pages)**
  - [ ] Read: **[#980] *AI Engineering: Building Applications With Foundation Models***:
    - [ ] **Ch 10:** *AI Engineering Architecture and User Feedback* (p. 940–965: Architecture blueprints, logging, fallback handling).
  - [ ] Write optimized multi-stage `Dockerfile` and `compose.yaml` to run your AI service with persistent volumes, environment secrets, and health checks.
  - [ ] Commit: `git commit -m "feat: add dockerfile and compose configuration"`
- [ ] **Week 35: Portfolio Polish & Technical Writing (~15 pages)**
  - [ ] Document project architecture with Mermaid diagrams (`flowchart LR`, `sequenceDiagram`) in your repository `README.md`.
  - [ ] Include reproducible setup instructions: `docker compose up -d` with automated health checks.
  - [ ] Commit: `git commit -m "docs: comprehensive architectural documentation and readme"`
- [ ] **Week 36: Final Capstone Deployment & Milestone 9**
  - [ ] **Deliverable: Milestone 9** — Deploy the complete, containerized Applied AI service live to the cloud or Hugging Face Spaces in `milestones/m09-production-capstone/`.
  - [ ] Final Commit & Push: `git add . && git commit -m "feat(m09): 9-month applied ai curriculum completed!" && git push`
  - [ ] Celebrate completing your 1st year Applied AI portfolio! 🚀

---

## 4. Milestone Projects Summary Table

| Month | Milestone Project | Repository Directory | Technologies |
| :---: | :--- | :--- | :--- |
| **M1** | Exploratory Data Analysis & Clean Data Pipeline | `milestones/m01-numpy-eda/` | NumPy, Pandas, Matplotlib, Seaborn |
| **M2** | From-Scratch Gradient Descent & Loss Visualizer | `milestones/m02-gradient-descent-scratch/` | NumPy, Matplotlib 3D, Calculus |
| **M3** | Leak-Free Predictive Pipeline & Streamlit GUI | `milestones/m03-scikit-pipeline/` | Scikit-Learn, Streamlit, XGBoost |
| **M4** | PyTorch Neural Classifier & Custom Training Loop | `milestones/m04-pytorch-mlp/` | PyTorch, Autograd, DataLoader |
| **M5** | Transfer Learning Vision Classifier | `milestones/m05-vision-transfer-learning/` | PyTorch, Torchvision, ResNet |
| **M6** | Multi-Head Self-Attention & Semantic Index | `milestones/m06-transformer-embeddings/` | PyTorch, Transformers, Embeddings |
| **M7** | Production RAG Assistant with Eval Test-Suite | `milestones/m07-rag-vector-search/` | ChromaDB, Rerankers, Eval Metrics |
| **M8** | Autonomous Multi-Tool Research Agent | `milestones/m08-autonomous-agent/` | ReAct, Tool Calling, Pydantic |
| **M9** | Containerized End-to-End AI Cloud Service | `milestones/m09-production-capstone/` | Docker, FastAPI, Streamlit |
