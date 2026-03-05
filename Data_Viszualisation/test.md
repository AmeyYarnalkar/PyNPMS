Good. Now let’s move to the **modern approach** used in almost all real projects.

The old `plt.subplot()` works, but it becomes messy when plots increase.
The better way is **`plt.subplots()`**.

---

# 2️⃣ Modern Method — `plt.subplots()`

## Syntax

```python
fig, ax = plt.subplots(rows, columns)
```

Meaning:

* **fig** → the whole figure (canvas)
* **ax** → the axes (individual plots)

Think of it like this:

```
Figure
 ├── Axes (Plot 1)
 ├── Axes (Plot 2)
 └── Axes (Plot 3)
```

---

# Example — Two Plots Side by Side

```python
import matplotlib.pyplot as plt

fig, ax = plt.subplots(1, 2)

ax[0].hist(df["NA_Sales"])
ax[0].set_title("NA Sales")

ax[1].hist(df["EU_Sales"])
ax[1].set_title("EU Sales")

plt.show()
```

---

# Understanding the Syntax

### This line

```python
fig, ax = plt.subplots(1, 2)
```

creates:

```
[ ax[0] ] [ ax[1] ]
```

So you access plots using:

```
ax[0]
ax[1]
```

---

# Adding Labels

With `subplots()` we don't use `plt.title()`.

Instead we use:

```python
ax[i].set_title()
ax[i].set_xlabel()
ax[i].set_ylabel()
```

Example:

```python
fig, ax = plt.subplots(1,2)

ax[0].hist(df["NA_Sales"])
ax[0].set_title("NA Sales")
ax[0].set_xlabel("Sales")
ax[0].set_ylabel("Frequency")

ax[1].hist(df["EU_Sales"])
ax[1].set_title("EU Sales")

plt.show()
```

---

# Adding Figure Size

```python
fig, ax = plt.subplots(1,2, figsize=(12,5))
```

This makes plots readable.

---

# 2 × 2 Grid Example

```python
fig, ax = plt.subplots(2,2, figsize=(10,8))
```

Layout becomes:

```
ax[0,0]   ax[0,1]

ax[1,0]   ax[1,1]
```

Example:

```python
fig, ax = plt.subplots(2,2)

ax[0,0].hist(df["NA_Sales"])
ax[0,1].hist(df["EU_Sales"])
ax[1,0].hist(df["JP_Sales"])
ax[1,1].hist(df["Global_Sales"])

plt.show()
```

---

# Why `plt.subplots()` is Better

Old method:

```
plt.subplot(2,2,1)
plt.subplot(2,2,2)
plt.subplot(2,2,3)
```

Hard to manage.

Modern method:

```
fig, ax = plt.subplots()
```

Clean and scalable.

Almost every professional codebase uses this.

---

# Quick Practice

Create **two boxplots side by side** using `subplots()`:

```
NA_Sales
Global_Sales
```

Expected layout:

```
[ NA Boxplot ] [ Global Boxplot ]
```

---

Next concept we’ll cover (also very useful):

**Multiple lines in one plot** — this is extremely common in data analysis.
