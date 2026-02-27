## Phase 1 — DataFrame Fundamentals 

**Goal:** Stop feeling lost when you see a dataset.

### Learn

* Series vs DataFrame
* Reading data

  * `read_csv()`
  * `read_excel()`
  * Handling JSON files
* Inspecting data

  * `head()`
  * `info()`
  * `describe()`
  * `shape`
  * `columns`
* Selecting data

  * `loc`
  * `iloc`
  * Column selection
* Filtering rows (conditions)

---

## Phase 2 — Cleaning Data 

Real datasets are messy. This is 70% of real work.

### Learn

* Missing values

  * `isna()`
  * `fillna()`
  * `dropna()`
* Duplicate handling
* Renaming columns
* Type conversion

  * `astype()`

**ML reason:**
Garbage data → garbage model. Clean data → usable signal.

---

## Phase 3 — Feature Engineering Basics

This is where pandas becomes powerful.

### Learn

* Creating new columns
* `apply()` (avoid overuse)
* `map()` / `replace()`
* One-hot encoding

  * `get_dummies()`
* Binning

  * `cut()`
  * `qcut()`

**ML reason:**
Better features = better models.

---

## Phase 4 — Advanced Data Manipulation & Analytical Workflows

**Goal:** Move from “using pandas” to handling real ML-ready datasets confidently.

---

### Category Analysis & Frequency Handling

* `value_counts()`

  * Normalized counts (`normalize=True`)
  * Handling NaN (`dropna=False`)
  * Binning numerical data (`bins=`)
* `unique()`
* `nunique()`

---

### Sorting & Ordering

* `sort_values()`

  * Single column
  * Multiple columns
  * Ascending / Descending control
* `sort_index()`

---

### Concatenation

* `pd.concat()`

  * Row-wise concatenation
  * Column-wise (`axis=1`)
  * `ignore_index=True`
  * `keys=` for hierarchical indexing
  * Handling mismatched columns

Difference between:

* `concat()` vs `merge()`

---

### GroupBy Operations (Core Analytical Skill)

* `groupby()`

  * Single column grouping
  * Multi-column grouping

### Aggregations

* `mean()`, `sum()`, `min()`, `max()`
* `agg()`
* Multiple aggregations
* Named aggregation

### Advanced Grouping

* `transform()`
* `filter()`
* `size()` vs `count()`

Understanding:

* Shape difference between `agg()` and `transform()`

---

### Pivoting & Reshaping

* `pivot()`
* `pivot_table()`

  * Handling duplicates
  * Multiple aggregation functions
  * Multiple index/columns
  * `fill_value=`
  * `margins=True`

---

### Crosstabulation

* `pd.crosstab()`

  * Multiple categorical variables
  * `normalize=`
  * Adding margins

---

### Merging & Joining DataFrames

* `pd.merge()`

  * `how="inner"`
  * `how="left"`
  * `how="right"`
  * `how="outer"`

### Merge on:

* Single key
* Multiple keys
* Different column names (`left_on`, `right_on`)
* Index-based merging

Understanding:

* Join behavior
* Null handling after joins

---

### MultiIndex (Hierarchical Indexing — Practical Level Only)

* `set_index()`
* `reset_index()`
* Selecting & slicing hierarchical index
* MultiIndex from `concat(keys=...)`

---

## Final Outcome After This Roadmap

After completing this:

* You can clean messy datasets
* You can engineer meaningful features
* You can reshape and aggregate data
* You can combine multiple datasets safely
* You can prepare ML-ready structured data

At this point, pandas is DONE for ML.

Then you move to:

👉 Matplotlib
👉 Then Machine Learning

