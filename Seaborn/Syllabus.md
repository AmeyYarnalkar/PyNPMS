# Seaborn Roadmap (High-Level Statistical Plots)

Seaborn sits on top of Matplotlib and makes statistical visuals easier. Think **EDA accelerator**, not a new universe to master.

---

##  Phase 1 — Core Plots 

Learn only these first:

* `sns.histplot()` → distributions
* `sns.boxplot()` → outliers
* `sns.scatterplot()` → relationships
* `sns.heatmap()` → correlation matrix

These alone cover most ML exploratory analysis.

---

##  Phase 2 — Relationship Visualization

**Learn**

* `pairplot()`
* `regplot()` or `lmplot()`

ML use:

* Detect feature relationships fast
* Spot linear vs nonlinear patterns

---

##  Phase 3 — Minimal Styling

Just enough:

* themes (`set_style`)
* palettes

Don’t dive into advanced aesthetics — low ROI for the  goal.

---