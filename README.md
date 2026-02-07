# PCA vs t-SNE: Visualizing High-Dimensional Data

## Overview

High-dimensional datasets are often difficult to interpret, making it challenging to identify patterns, relationships, and clusters. In this project, I applied **Principal Component Analysis (PCA)** and **t-Distributed Stochastic Neighbor Embedding (t-SNE)** to transform complex datasets into lower-dimensional representations for effective visualization and analysis.

The objective was not just to reduce dimensions, but to understand **when linear methods are sufficient and when non-linear techniques reveal deeper structure**.

---

## Objectives

* Prepare and standardize high-dimensional data for fair feature contribution.
* Apply PCA to capture maximum variance using linear projections.
* Use t-SNE to uncover non-linear relationships and local cluster structure.
* Visualize embeddings in 2D/3D for intuitive interpretation.
* Compare both techniques to understand their strengths, limitations, and practical use cases.

---

## Tech Stack

* **Python**
* **Scikit-learn**
* **Pandas**
* **NumPy**
* **Matplotlib / Seaborn**

---

## Project Workflow

### 1. Data Preprocessing

* Cleaned the dataset and handled missing values.
* Standardized features using scaling to ensure equal contribution across variables.
* Verified data suitability for dimensionality reduction.

### 2. PCA Implementation

* Applied PCA to reduce dimensionality while preserving global variance.
* Analyzed explained variance to determine the optimal number of components.
* Generated 2D projections to observe large-scale structure.

### 3. t-SNE Implementation

* Applied t-SNE to capture complex, non-linear relationships.
* Tuned parameters such as perplexity for meaningful embeddings.
* Visualized local clusters that were not clearly separable using PCA.

### 4. Visualization & Analysis

* Created scatter plots to compare how each technique represents the same dataset.
* Evaluated how well clusters and separations appeared after reduction.
* Interpreted differences between global vs local structure preservation.

---

## Results

### PCA Projection
```
images/pca_plot.png
```
### t-SNE Projection
```
images/tsne_plot.png
```

---

## PCA vs t-SNE — Quick Comparison

| Technique | Type       | Strength                                               | Limitation                                       |
| --------- | ---------- | ------------------------------------------------------ | ------------------------------------------------ |
| **PCA**   | Linear     | Fast, interpretable, preserves global variance         | May miss complex non-linear relationships        |
| **t-SNE** | Non-linear | Excellent for visualizing clusters and local structure | Computationally expensive and less interpretable |

---

## Key Takeaways

* **PCA** is highly efficient for reducing dimensionality when the dataset largely follows linear structure.
* **t-SNE** excels at revealing hidden clusters but should primarily be used for visualization rather than downstream modeling.
* Feature scaling significantly impacts dimensionality reduction performance.
* There is no universally “better” method — the right choice depends on the problem, dataset size, and whether global interpretability or local structure is more important.

---

## How to Run the Project

```bash
# Clone the repository
git clone <your-repo-url>

# Navigate to the project folder
cd <project-folder>

# Install dependencies
pip install -r requirements.txt

# Run the main script / notebook
python winepca.py
python winetsne.py
```

---

## Ideal Use Cases for This Approach

* Exploratory Data Analysis (EDA)
* Feature space visualization
* Detecting hidden clusters
* Understanding dataset structure before modeling
* Communicating complex data insights visually

---

## Future Improvements

* Experiment with **UMAP** for faster non-linear dimensionality reduction.
* Evaluate performance across multiple datasets.
* Integrate interactive visualizations using Plotly.
* Benchmark runtime differences between techniques.

---

## Author

**Khushi Ozha**

If you found this project interesting or useful, feel free to connect or reach out!
