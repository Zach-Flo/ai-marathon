# AI Marathon

One hour a day, learning how AI actually works, from the math up.

Everything here is written by hand, without AI autocomplete. The goal is understanding, not a finished product. Progress is logged in [LOG.md](LOG.md).

## The plan

| Phase | Focus | Capstone |
|---|---|---|
| 0 | Python and NumPy fluency | Comfortable writing NumPy code and plots |
| 1 | Linear algebra and calculus refresher | Gradient descent from scratch |
| 2 | Neural networks from scratch | My own autograd engine (micrograd) |
| 3 | Transformers | A tiny GPT, plus vector search by hand |
| 4 | Applied AI engineering | A deployed AI app (RAG, evals) |
| 5 | Quantum and photonics | Circuits on real IBM hardware; photonic quantum ML |

Work is split into **sections**, not days. A section takes as long as it takes, and I move on when its "move on when" check is met.

## Unit 1: Python by writing

- [x] **1. Setup:** uv, Python 3.12, JupyterLab, this repo. *Move on when* the repo has its first log entry.
- [x] **2. Five functions from memory.** *Move on when* I can write them without looking anything up.
- [ ] **3. `Vector` class by hand:** `+`, `*`, `dot`, `norm`. *Move on when* every assert passes and I can explain each method.
- [ ] **4. NumPy:** arrays, shapes, broadcasting; redo `Vector` in NumPy. *Move on when* I can predict an array's shape before I run it.
- [ ] **5. matplotlib:** plot vectors as arrows. *Move on when* I can plot any vector I want.
- [ ] **Unit review**

## Unit 2: Vectors and matrices

Resource: 3Blue1Brown, *Essence of Linear Algebra*

- [ ] **6. Span** (Ch 1–2). *Move on when* I can plot a span and explain why two vectors fill the plane.
- [ ] **7. Linear transformations** (Ch 3). *Move on when* I can predict what a matrix does to a grid before plotting it.
- [ ] **8. Matrix multiplication** (Ch 4), written with loops. *Move on when* my version matches `A @ B`.
- [ ] **9. Dot product and cosine similarity** (Ch 9). *Move on when* I can explain why "king" sits close to "queen."
- [ ] **10. Explain Sections 6–9 in my own words.** *Move on when* I can write it without notes.
- [ ] **Unit review**

## Unit 3: Determinants, eigenvectors, calculus

Resources: 3Blue1Brown, *Essence of Linear Algebra* and *Essence of Calculus*; Khan Academy multivariable calculus

- [ ] **11. Determinants** (Ch 5–7). *Move on when* I can say what a determinant of 0 means visually.
- [ ] **12. Eigenvectors** (Ch 13–14). *Move on when* I can find them on a plot and check with `np.linalg.eig`.
- [ ] **13. Derivatives and the chain rule.** *Move on when* my numerical derivative matches the one I work out by hand.
- [ ] **14. Partial derivatives and gradients.** *Move on when* I can compute and explain the gradient of `f(x, y)`.
- [ ] **15. Teach the chain rule** in LOG.md. *Move on when* a coworker could follow my explanation.
- [ ] **Unit review**

**Phase 1 capstone:** gradient descent from scratch, fitting a line to noisy data with no ML libraries.

Later units will be planned as I get to them.

## Rules

1. Write the code myself. AI is a tutor, not an autocomplete.
2. Every session ends with a commit and a line in LOG.md.
3. Spend about 15 minutes reading or watching, then 45 minutes building.

## Running it

```bash
uv sync
uv run jupyter lab
```
