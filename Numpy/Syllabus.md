# NumPy Roadmap for Machine Learning

##  Phase 1 — Absolute Core (Start Here)

Goal: Stop thinking in loops. Start thinking in arrays.

**What to learn**

* What NumPy actually is (ndarray vs list)
* Creating arrays
  `array()`, `zeros()`, `ones()`, `arange()`, `linspace()`, `random`
* Shape, ndim, dtype
* Indexing and slicing
* Boolean indexing
* Reshape, flatten, transpose

**Why this matters for ML**
Every dataset you touch becomes a matrix. If indexing feels slow or confusing, ML will feel painful.

---

##  Phase 2 — Vectorization & Broadcasting (MOST IMPORTANT)

This is where beginners struggle — and where performance comes from.

**What to learn**

* Element-wise operations
* Broadcasting rules
* Vectorized math (no loops)
* Axis concept

Examples:

* Normalization
* Feature scaling
* Batch operations

---

##  Phase 3 — Matrix and Multiplication (ML Core)

ML = linear algebra in disguise.

* Dot product
* Matrix multiplication
* `@` operator
* Matrix transpose

---

##  Phase 4 — Advanced Indexing & Masking 
This is what real pipelines use.

**Learn**

* Fancy indexing
* Masks
* `where`
* `argmax`, `argsort`
* Conditional selection
