# Data Analysis & Machine Learning Foundations

This repository documents my learning journey through the core tools required for **data analysis and machine learning workflows**.

The focus is on building strong fundamentals in:

* NumPy
* Pandas
* Matplotlib
* Seaborn

These tools form the **data processing and exploratory analysis stack** used before applying machine learning models.

---

# Learning Roadmap

The learning path is structured to move from **numerical computation → data manipulation → visualization → machine learning readiness**.

```
NumPy → Pandas → Visualization → Machine Learning
```

---

# NumPy Roadmap for Machine Learning

NumPy provides the foundation for numerical computing and matrix operations used in machine learning algorithms.

## Phase 1 — Absolute Core

Goal: Stop thinking in loops and start thinking in arrays.

Topics covered:

* Understanding `ndarray` vs Python lists
* Creating arrays

  * `array()`
  * `zeros()`
  * `ones()`
  * `arange()`
  * `linspace()`
  * random number generation
* Array attributes

  * `shape`
  * `ndim`
  * `dtype`
* Indexing and slicing
* Boolean indexing
* Reshaping arrays

  * `reshape()`
  * `flatten()`
  * `transpose()`

Why this matters:

Machine learning models operate on **vectors and matrices**, so efficient array manipulation is essential.

---

## Phase 2 — Vectorization & Broadcasting

Goal: Write fast numerical code without loops.

Topics covered:

* Element-wise operations
* Broadcasting rules
* Vectorized mathematical operations
* Understanding the `axis` concept

Applications:

* Feature normalization
* Feature scaling
* Batch operations on datasets

Vectorization is critical because it enables **high-performance numerical computation**.

---

## Phase 3 — Matrix Operations

Machine learning algorithms rely heavily on linear algebra.

Topics covered:

* Dot product
* Matrix multiplication
* `@` operator
* Matrix transpose

These operations form the backbone of algorithms such as:

* Linear regression
* Neural networks
* Principal component analysis

---

## Phase 4 — Advanced Indexing & Masking

Used frequently in real-world data pipelines.

Topics covered:

* Fancy indexing
* Boolean masks
* `np.where`
* `argmax`
* `argsort`
* Conditional selection

These techniques allow efficient filtering and transformation of large datasets.

---

# Pandas Roadmap

Pandas is used for **data manipulation, cleaning, and feature engineering**.

---

## Phase 1 — DataFrame Fundamentals

Goal: Become comfortable exploring datasets.

Topics covered:

* Series vs DataFrame
* Reading datasets

  * `read_csv()`
  * `read_excel()`
  * JSON files
* Inspecting data

  * `head()`
  * `info()`
  * `describe()`
  * `shape`
  * `columns`
* Selecting data

  * column selection
  * `loc`
  * `iloc`
* Filtering rows using conditions

---

## Phase 2 — Data Cleaning

Real-world datasets require extensive preprocessing.

Topics covered:

* Handling missing values

  * `isna()`
  * `fillna()`
  * `dropna()`
* Removing duplicates
* Renaming columns
* Type conversion

  * `astype()`

Importance:

Clean data leads to reliable machine learning models.

---

## Phase 3 — Feature Engineering

Feature engineering transforms raw data into meaningful model inputs.

Topics covered:

* Creating new columns
* `apply()` (used carefully)
* `map()` and `replace()`
* One-hot encoding

  * `get_dummies()`
* Binning numerical data

  * `cut()`
  * `qcut()`

Better features often lead to **better model performance**.

---

## Phase 4 — Advanced Data Manipulation

These operations are common in analytical workflows.

---

### Category Analysis

* `value_counts()`
* normalized frequencies
* handling missing values
* binning numerical data

Additional utilities:

* `unique()`
* `nunique()`

---

### Sorting

* `sort_values()`
* sorting by multiple columns
* ascending and descending order
* `sort_index()`

---

### Concatenation

Combining datasets using:

```
pd.concat()
```

Techniques covered:

* row-wise concatenation
* column-wise concatenation
* `ignore_index`
* hierarchical indexing using `keys`

Difference between:

```
concat vs merge
```

---

### GroupBy Operations

One of the most important analytical tools.

Topics covered:

* `groupby()` on single or multiple columns
* aggregations

```
mean
sum
min
max
```

* multiple aggregations using `agg()`
* named aggregations

Advanced grouping operations:

* `transform()`
* `filter()`
* `size()` vs `count()`

Understanding the difference between:

```
agg() vs transform()
```

---

### Pivoting & Reshaping

Data restructuring techniques.

Topics covered:

* `pivot()`
* `pivot_table()`

Handling:

* duplicate values
* multiple aggregation functions
* hierarchical rows and columns
* missing values
* margins

---

### Crosstabulation

Used for analyzing relationships between categorical variables.

```
pd.crosstab()
```

Features:

* normalization
* margins
* multiple categorical variables

---

### Merging & Joining DataFrames

Combining multiple datasets.

Topics covered:

```
pd.merge()
```

Join types:

* inner join
* left join
* right join
* outer join

Merging techniques:

* single key
* multiple keys
* different column names
* index-based joins

Understanding how joins affect missing data.

---

### MultiIndex

Practical hierarchical indexing.

Topics covered:

* `set_index()`
* `reset_index()`
* selecting hierarchical data

---

# Data Visualization

Visualization is used to understand data patterns before modeling.

Libraries used:

* Matplotlib
* Seaborn

---

## Matplotlib

Matplotlib provides foundational plotting capabilities.

Plots covered:

* Histogram
* Boxplot
* Bar chart
* Scatter plot
* Line plot

Additional concepts:

* Subplots
* Multiple lines in a plot
* Figure sizing
* Saving figures
* `tight_layout()` for clean visual structure

---

## Seaborn

Seaborn builds on top of Matplotlib and simplifies statistical visualization.

Plots covered:

* `histplot()` – distribution analysis
* `countplot()` – categorical frequency
* `boxplot()` – outlier detection and distribution comparison
* `scatterplot()` – relationships between variables
* `regplot()` – regression trend visualization
* `heatmap()` – correlation matrix visualization
* `pairplot()` – multi-variable relationship exploration

---

# Outcome

After completing this roadmap:

* Datasets can be explored and understood quickly
* Data can be cleaned and transformed efficiently
* Meaningful features can be engineered
* Relationships and distributions can be visualized
* Data can be prepared for machine learning models

At this stage, the **data analysis foundation for machine learning is complete**.

---
