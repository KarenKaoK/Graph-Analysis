# Graph Analysis 

This repository is a notebook-based graph analysis project focused on social-network data, shortest-path exploration, and centrality analysis. It combines Python experiments in Jupyter notebooks with browser-based visualization examples built from exported HTML files.

## Overview

The project currently includes three main study areas:

- `graph_algorithm.ipynb`: general graph analysis experiments using the `ogbn-products` dataset and `networkx`.
- `shortest_path/short_path.ipynb`: shortest path exploration and "six degrees of separation" style analysis using Facebook network data.
- `centrality/degree centrality.ipynb`: degree centrality analysis on a small social graph.

This is not structured as a Python package or application. The main deliverables are notebooks, local datasets, generated images, and interactive HTML demos.

## Packages

- `networkx`
- `matplotlib`
- `pandas`
- `ogb`
- `torch`
- `scikit-learn`
- `pyvis`
- `vis-network` and `tom-select` for static HTML visualization

## Repository Structure

```text
.
|-- graph_algorithm.ipynb
|-- centrality/
|   `-- degree centrality.ipynb
|-- dataset/
|   |-- twitter/
|   `-- ogbn_products/
`-- shortest_path/
    |-- short_path.ipynb
    |-- example.html
    |-- example2.html
    |-- example_shortest_path.html
    |-- example_shortest_path_2.html
    |-- networ.html
    |-- data/
    `-- lib/
```

## Included Datasets

### Facebook network dataset

Located under [`shortest_path/data/facebook_combined.txt`](/Users/ren/Desktop/karen/git_karen/graph/shortest_path/data/facebook_combined.txt).

- 4,039 nodes
- 88,234 edges
- Used for shortest path, graph sampling, and separation analysis

The `shortest_path/data/facebook/` folder also contains ego-network files from the Facebook dataset.

### Twitter toy dataset

Located under [`dataset/twitter/social-nodes.csv`](/Users/ren/Desktop/karen/git_karen/graph/dataset/twitter/social-nodes.csv) and [`dataset/twitter/social-relationships.csv`](/Users/ren/Desktop/karen/git_karen/graph/dataset/twitter/social-relationships.csv).

- Small CSV-based example graph
- Useful for introductory graph modeling and centrality experiments

### OGBN-Products dataset

Located under [`dataset/ogbn_products`](/Users/ren/Desktop/karen/git_karen/graph/dataset/ogbn_products).

- `edge.csv.gz`: about 61.9 million rows
- `node-label.csv.gz`: about 2.45 million rows
- Includes mapping files for product identifiers and category labels
- Used in `graph_algorithm.ipynb`

## What You Can Explore

- Build and inspect graphs from real datasets
- Compute graph statistics and node degree information
- Visualize subgraphs with `matplotlib`
- Experiment with shortest path queries
- Demonstrate small-world / six-degrees concepts
- Open interactive HTML network visualizations in a browser

## Getting Started

### 1. Create and activate a Python environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 2. Install dependencies

```bash
pip install --upgrade pip
pip install jupyter networkx matplotlib pandas ogb torch scikit-learn pyvis tqdm
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

Then open:

- [`graph_algorithm.ipynb`](/Users/ren/Desktop/karen/git_karen/graph/graph_algorithm.ipynb)
- [`shortest_path/short_path.ipynb`](/Users/ren/Desktop/karen/git_karen/graph/shortest_path/short_path.ipynb)
- [`centrality/degree centrality.ipynb`](/Users/ren/Desktop/karen/git_karen/graph/centrality/degree%20centrality.ipynb)

## Interactive HTML Examples

You can open these files directly in a browser:

- [`shortest_path/example.html`](/Users/ren/Desktop/karen/git_karen/graph/shortest_path/example.html)
- [`shortest_path/example2.html`](/Users/ren/Desktop/karen/git_karen/graph/shortest_path/example2.html)
- [`shortest_path/example_shortest_path.html`](/Users/ren/Desktop/karen/git_karen/graph/shortest_path/example_shortest_path.html)
- [`shortest_path/example_shortest_path_2.html`](/Users/ren/Desktop/karen/git_karen/graph/shortest_path/example_shortest_path_2.html)
- [`shortest_path/networ.html`](/Users/ren/Desktop/karen/git_karen/graph/shortest_path/networ.html)

These examples use local frontend assets stored in [`shortest_path/lib`](/Users/ren/Desktop/karen/git_karen/graph/shortest_path/lib).


