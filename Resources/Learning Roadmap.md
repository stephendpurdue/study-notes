# Learning Roadmap — MSc AI Preparation
*Linear Algebra onwards · Paired with Obsidian + Pomodoro*

---

## Where You Are Now

**3Blue1Brown Linear Algebra** — in progress

Finish the playlist before moving to Stage 1. Then follow the stages below in order. Each stage assumes the previous one's concept notes exist and are linked in Obsidian.

---

## How Each Session Works

Every topic is structured as two Pomodoros:

- **Pomodoro 1** — active engagement with the material (watch, read, sketch)
- **Pomodoro 2** — build or write from memory (implement, push, write concept note)

Never both passive. Never both active. Boot.dev runs as your second block each day alongside every stage — maths and ML first when your brain is fresh, Boot.dev second.

---

## Stage 1 — Finish Linear Algebra
**Now · 3Blue1Brown remaining chapters**

### Eigenvalues, dot products, cross products, change of basis

**Resource:** 3Blue1Brown: Essence of Linear Algebra playlist (free, YouTube) — finish all remaining chapters

**Pomodoro 1:** Watch one chapter. Pause when you see a transformation. Sketch it on paper before continuing.

**Pomodoro 2:** Close the video. Open Obsidian. Write the concept note from memory — what it does geometrically, why it matters.

**Obsidian:**
> Concept note: `[[eigenvalues]]` → link to `[[matrix-multiplication]]` and `[[PCA]]`
> Feynman field: *"Eigenvectors are directions a transformation doesn't rotate, only stretches — the eigenvalue tells you by how much"*

**Anki card:**
> Q: What does an eigenvalue tell you about a transformation?
> A: How much it stretches along that eigenvector's direction — a value of 2 means that direction is doubled.

---

## Stage 2 — Calculus + Gradient Descent
**~1 week · The algorithm behind all ML training**

### 3Blue1Brown: Essence of Calculus

**Resource:** All chapters — derivatives, chain rule, integrals. Free on YouTube.

**Pomodoro 1:** Watch Ch 1–3. Focus on: what does a derivative actually mean at a point? Sketch the tangent line on paper.

**Pomodoro 2:** Implement derivative approximation in Python: `(f(x+h) - f(x)) / h`. Push to GitHub.

**Obsidian:**
> Concept note: `[[derivatives]]` → link to `[[gradient-descent]]` and `[[chain-rule]]`
> Feynman field: *"A derivative is the instantaneous rate of change — the slope of the tangent at a single point"*

**Anki card:**
> Q: What is the chain rule for and why does it matter for neural networks?
> A: It lets you compute how a change in early layers affects the final loss — the foundation of backpropagation.

---

### Build gradient descent from scratch

**Resource:** Python + NumPy only. Minimise f(x) = x². No tutorial open.

**Pomodoro 1:** Attempt from memory. Write the update rule: `x = x - lr * gradient`. Run it. Watch it converge.

**Pomodoro 2:** Add matplotlib to animate the steps descending. Push to repo: `gradient_descent.py`

**Obsidian:**
> Concept note: `[[gradient-descent]]` → link to `[[derivatives]]`, `[[loss-function]]`, `[[learning-rate]]`
> Feynman field: *"Gradient descent moves parameters downhill on the loss surface in small steps until it reaches the lowest point"*
> Link the GitHub repo in this note.

**Anki card:**
> Q: Write the gradient descent update rule.
> A: θ = θ − α∇L(θ) — parameter minus learning rate times gradient of loss.

**GitHub commit:** `add: gradient descent from scratch with matplotlib animation`

---

## Stage 3 — Probability + Bayes
**~1 week · Appears in week 1 of every MSc AI module**

### 3Blue1Brown: Bayes theorem + StatQuest probability

**Resource:** 3Blue1Brown Bayes video + StatQuest probability playlist (free, YouTube)

**Pomodoro 1:** Watch the Bayes video. Write the formula on paper. Work through the medical diagnosis example manually — do not skip this step.

**Pomodoro 2:** Open Obsidian. Write 3 Bayes examples from memory. Only then check your notes.

**Obsidian:**
> Concept note: `[[bayes-theorem]]` → link to `[[conditional-probability]]` and `[[naive-bayes]]`
> Feynman field: *"Bayes theorem updates your belief about something given new evidence — prior belief × likelihood of evidence = posterior belief"*

**Anki card:**
> Q: State Bayes theorem and give one real-world use.
> A: P(A|B) = P(B|A)·P(A)/P(B). Used in spam filters: compute P(spam|word) given known spam rates.

---

### Probability notebook

**Resource:** Python + matplotlib. No scipy for the Gaussian — implement the PDF from scratch.

**Pomodoro 1:** Code Gaussian PDF from scratch. Plot it. Change μ and σ and watch what happens — understand what each parameter does visually.

**Pomodoro 2:** Add Bayes worked examples to the notebook. Push to GitHub: `probability_foundations.ipynb`

**Obsidian:**
> Update `[[bayes-theorem]]` concept note with your notebook link.
> Create `[[distributions]]` note — link Gaussian, Bernoulli, Binomial. Note when each appears in ML.

**Anki card:**
> Q: What does variance measure and why does it matter in ML?
> A: Spread around the mean — high variance = overfitting (too sensitive to training data), high bias = underfitting (too simple).

**GitHub commit:** `add: probability foundations — gaussian pdf, bayes examples`

---

## Stage 4 — Python + NumPy Consolidation
**~3 days · MSc practicals use NumPy from week 1**

### NumPy quickstart + matrix operations

**Resource:** numpy.org official tutorial (free). One focused session.

**Pomodoro 1:** Work through the tutorial typing every example yourself. Pause at broadcasting — draw what it does to the arrays on paper before continuing.

**Pomodoro 2:** Build 15 exercises: reshape, slice, dot product, matrix multiply, eigenvectors with `np.linalg`. Push to GitHub: `numpy_exercises.ipynb`

**Obsidian:**
> Concept note: `[[numpy-operations]]` → link to `[[linear-algebra]]` and `[[matrix-multiplication]]`
> Note which NumPy functions map to which maths concepts — e.g. `np.dot` = dot product, `np.linalg.eig` = eigendecomposition.

**Anki card:**
> Q: What does NumPy broadcasting do?
> A: Automatically expands smaller arrays to match shapes — lets you add a (3,) vector to a (4,3) matrix without writing a loop.

**GitHub commit:** `add: numpy exercises — reshape, broadcasting, matrix operations`

---

## Stage 5 — Neural Network from Scratch
**~1 week · The most impressive thing on your GitHub before September**

### 3Blue1Brown Neural Networks + Karpathy micrograd

**Resource:** All 4 Neural Network videos + micrograd video (2.5 hrs). Free on YouTube. Watch completely before writing any code.

**Pomodoro 1:** Watch NN Ch 1–2. Sketch the architecture from memory: inputs → weights → activations → output. Label every arrow.

**Pomodoro 2:** Watch backprop chapter. Trace the chain rule through a 2-layer network on paper. Every gradient labelled. Do not open an IDE yet.

**Obsidian:**
> Concept note: `[[backpropagation]]` → link to `[[chain-rule]]`, `[[gradient-descent]]`, `[[neural-networks]]`
> Feynman field: *"Backprop applies the chain rule layer by layer, flowing gradients backwards to tell each weight how much it contributed to the error"*

**Anki card:**
> Q: Why do we need activation functions in neural networks?
> A: Without them, stacked linear layers collapse to one linear layer — activations add non-linearity so the network can learn complex patterns.

---

### Build in NumPy — then port to PyTorch

**Resource:** No tutorials open. Build from memory. Create repo: `neural-net-from-scratch`

**Pomodoro 1:** Attempt the full forward pass from memory: matrix multiply → activation → softmax → cross-entropy loss. Don't look anything up until you're stuck for more than 10 minutes.

**Pomodoro 2:** Add backpropagation. Train on XOR. Once it works, port to PyTorch. README compares both versions: what PyTorch handles that NumPy forces you to write manually.

**Obsidian:**
> Push both files. Update README with architecture diagram.
> Link this repo in your `[[backpropagation]]` concept note.
> Note: this repo is your MSc conversation starter — professors who see this will ask about it in week 1.

**Anki card:**
> Q: What does PyTorch autograd do that NumPy doesn't?
> A: Tracks operations on tensors and automatically computes gradients — you write the forward pass only, backprop is handled for you.

**GitHub commit:** `add: neural network from scratch — numpy and pytorch versions with backprop`

---

## Stage 6 — First End-to-End ML Project
**~1 week · Real data, real model, documented reasoning**

### Pandas EDA + scikit-learn classifier

**Resource:** Kaggle: Titanic or House Prices dataset. Kaggle Pandas micro-course (free).

**Pomodoro 1:** Load the data. Explore without modelling yet — distributions, null values, correlations. Write hypotheses about what predicts the target.

**Pomodoro 2:** Train logistic regression. Compute accuracy, precision, recall, F1, ROC curve. Compare 2 model types. Document which performs better and why.

**Obsidian:**
> Concept notes: `[[precision-vs-recall]]`, `[[overfitting]]`, `[[cross-validation]]`
> Link all three to your `[[neural-networks]]` and `[[gradient-descent]]` notes.
> Feynman for precision vs recall: *"Precision = when you say yes, how often are you right. Recall = of all the actual yeses, how many did you catch."*

**Anki card:**
> Q: When would you prioritise recall over precision?
> A: When false negatives are costly — e.g. cancer screening, where missing a case is worse than a false alarm.

---

### Write the project README

**Resource:** Excalidraw (excalidraw.com, free) for architecture diagram.

**Pomodoro 1:** Write: problem → your approach → results → what you'd do differently. No code in this document — reasoning only.

**Pomodoro 2:** Add the architecture diagram. Review the whole repo as if you were a professor seeing it for the first time.

**Obsidian:**
> The README is the documentation — no separate concept note needed here.
> Add the repo link to your `[[ml-projects]]` index note.

**GitHub commit:** `add: full project README with architecture diagram and results`

---

## Stage 7 — Boot.dev Track
**Ongoing · Run in parallel with all stages above**

### Sequence: Git → Linux → DSA → SQL → Docker → AWS → RAG

**Resource:** Boot.dev (paid subscription)

**How it fits into your day:**
Boot.dev goes in your second Pomodoro block — after the maths or ML main work. Never first. Your brain's freshest hours go to the conceptual material.

**Pomodoro 1 (after main session):** Work through the Boot.dev lesson, type every exercise yourself.

**Pomodoro 2:** Push the exercise output to GitHub before closing the session.

**Obsidian:**
> One concept note per Boot.dev concept that surprises you — not every lesson.
> Link where relevant: `[[sql]]` → `[[data-pipeline]]`, `[[docker]]` → `[[containerisation]]`, `[[rag]]` → `[[embeddings]]` and `[[semantic-search]]`

**Anki card per module:**
> Q: What does Docker solve that running locally doesn't?
> A: Guarantees the same environment everywhere — your model runs identically on your machine, a teammate's machine, and any cloud server.

---

## The Obsidian System — Quick Reference

### Vault structure

```
vault/
├── 00-inbox/          ← raw capture, uncleaned
├── 01-concepts/       ← one note per concept
├── 02-projects/       ← one note per GitHub repo
├── 03-courses/        ← one note per module/course
├── 04-recall/         ← weekly blank-page recall dumps
├── 05-resources/      ← papers, videos, books
└── templates/         ← reusable templates
```

### Concept note template

```markdown
# [Concept Name]

**One sentence:**

**The intuition (no jargon):**

**The maths or code:**

**Why it matters for AI/MSc:**

**Connected concepts:** [[link]] [[link]]

**I was confused by:**

**Feynman test:** (explain as if teaching a complete beginner)

**Anki card created:** [ ]

---
*Source:*
*Date first encountered:*
*Last recalled:*
```

### Rules

- Write the concept note **after** attempting from memory — never copy from source
- Fill the Feynman field or you haven't understood it yet
- Every note links to at least two others — isolated notes signal isolated understanding
- Push to GitHub every evening with a descriptive commit message
- Weekly recall: every Sunday, blank page, write everything from memory before opening any notes

### After every lecture (24-hour rule)

1. Blank page recall — write everything you remember, no notes open
2. Compare with lecture notes — mark gaps
3. Process into concept notes in `01-concepts/`
4. Create Anki cards — one per concept, question must require explanation not recognition
5. Link new concepts to existing ones with `[[wikilinks]]`

---

## Anki — Daily Habit

- 10 minutes every morning before studying
- One card per concept, not per page
- Question format that works: *"Explain X without using the word X"*
- Question format that doesn't work: *"What is X?"* — recognition, not understanding
- Use the Obsidian-to-Anki plugin to sync cards automatically from your concept notes

---

## GitHub — Commit Every Session

Every session ends with a push. Commit messages follow this pattern:

```
add: gradient descent from scratch with animation
add: bayes theorem notebook — 3 worked examples
update: neural network README with architecture diagram
fix: backprop gradient calculation in layer 2
```

Your repo list by the end of this roadmap:

| Repo | Contents |
|---|---|
| `python-foundations` | OOP, data structures, NumPy exercises |
| `maths-for-ml` | Gradient descent, Bayes notebook, probability distributions |
| `neural-net-from-scratch` | NumPy version + PyTorch version + backprop notes |
| `ml-foundations` | EDA, classification, evaluation, full project README |
| `deep-learning-notes` | Transformer architecture, attention implementation |
| `data-engineering` | Docker, AWS notes, RAG foundations |

---

*Last updated: May 2026 · Paired with Career Plan (ML Engineering Track)*
