# Graph Analysis Notebook Collection

This repository is a notebook-based graph analysis project focused on social-network data, shortest-path exploration, and centrality analysis. It combines Python experiments in Jupyter notebooks with browser-based visualization examples built from exported HTML files.

## Overview

The project currently includes three main study areas:

- `graph_algorithm.ipynb`: general graph analysis experiments using the `ogbn-products` dataset and `networkx`.
- `shortes_path/short_path.ipynb`: shortest path exploration and "six degrees of separation" style analysis using Facebook network data.
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
`-- shortes_path/
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

Located under [`shortes_path/data/facebook_combined.txt`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/data/facebook_combined.txt).

- 4,039 nodes
- 88,234 edges
- Used for shortest path, graph sampling, and separation analysis

The `shortes_path/data/facebook/` folder also contains ego-network files from the Facebook dataset.

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
- [`shortes_path/short_path.ipynb`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/short_path.ipynb)
- [`centrality/degree centrality.ipynb`](/Users/ren/Desktop/karen/git_karen/graph/centrality/degree%20centrality.ipynb)

## Interactive HTML Examples

You can open these files directly in a browser:

- [`shortes_path/example.html`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/example.html)
- [`shortes_path/example2.html`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/example2.html)
- [`shortes_path/example_shortest_path.html`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/example_shortest_path.html)
- [`shortes_path/example_shortest_path_2.html`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/example_shortest_path_2.html)
- [`shortes_path/networ.html`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/networ.html)

These examples use local frontend assets stored in [`shortes_path/lib`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/lib).

# 中文說明
Graph 圖分析 Notebook 專案

這個專案是一個以 Jupyter Notebook 為主的圖分析練習與展示集合，內容涵蓋社群網路資料分析、最短路徑探索，以及中心性分析。專案同時包含 Python notebook、產出的圖片，以及可直接在瀏覽器開啟的互動式 HTML 視覺化範例。

## 專案內容

目前主要分成三個主題：

- `graph_algorithm.ipynb`：使用 `networkx` 與 `ogbn-products` 資料集進行一般圖演算法與子圖分析。
- `shortes_path/short_path.ipynb`：以 Facebook 社群網路資料做最短路徑與六度分隔理論相關實驗。
- `centrality/degree centrality.ipynb`：以小型社群圖進行 degree centrality 分析。

## packages

- `networkx`
- `matplotlib`
- `pandas`
- `ogb`
- `torch`
- `scikit-learn`
- `pyvis`
- `vis-network`、`tom-select`（用於靜態 HTML 互動視覺化）

## 目錄結構

```text
.
|-- graph_algorithm.ipynb
|-- centrality/
|   `-- degree centrality.ipynb
|-- dataset/
|   |-- twitter/
|   `-- ogbn_products/
`-- shortes_path/
    |-- short_path.ipynb
    |-- example.html
    |-- example2.html
    |-- example_shortest_path.html
    |-- example_shortest_path_2.html
    |-- networ.html
    |-- data/
    `-- lib/
```

## 內含資料集

### Facebook 社群網路資料

位置：[`shortes_path/data/facebook_combined.txt`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/data/facebook_combined.txt)

- 4,039 個節點
- 88,234 條邊
- 用於最短路徑、圖抽樣與六度分隔分析

此外，`shortes_path/data/facebook/` 目錄中也包含 Facebook ego network 相關檔案。

### Twitter 小型示例資料

位置：[`dataset/twitter/social-nodes.csv`](/Users/ren/Desktop/karen/git_karen/graph/dataset/twitter/social-nodes.csv) 與 [`dataset/twitter/social-relationships.csv`](/Users/ren/Desktop/karen/git_karen/graph/dataset/twitter/social-relationships.csv)

- 小型 CSV 社群圖資料
- 適合做入門圖建模與中心性分析示例

### OGBN-Products 資料集

位置：[`dataset/ogbn_products`](/Users/ren/Desktop/karen/git_karen/graph/dataset/ogbn_products)

- `edge.csv.gz`：約 6,185 萬列
- `node-label.csv.gz`：約 245 萬列
- 包含商品編號與分類標籤對照檔
- 主要用於 `graph_algorithm.ipynb`

## 可以做什麼

- 從真實資料建立圖結構
- 計算節點 degree 與基本圖統計
- 使用 `matplotlib` 視覺化子圖
- 實驗最短路徑查詢
- 展示 small-world / 六度分隔概念
- 直接用瀏覽器打開互動式網路圖 HTML 範例

## 如何開始

### 1. 建立並啟用 Python 環境

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 2. 安裝相依套件

```bash
pip install --upgrade pip
pip install jupyter networkx matplotlib pandas ogb torch scikit-learn pyvis tqdm
```

### 3. 啟動 Jupyter Notebook

```bash
jupyter notebook
```

接著打開：

- [`graph_algorithm.ipynb`](/Users/ren/Desktop/karen/git_karen/graph/graph_algorithm.ipynb)
- [`shortes_path/short_path.ipynb`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/short_path.ipynb)
- [`centrality/degree centrality.ipynb`](/Users/ren/Desktop/karen/git_karen/graph/centrality/degree%20centrality.ipynb)

## HTML 互動範例

以下檔案可直接用瀏覽器開啟：

- [`shortes_path/example.html`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/example.html)
- [`shortes_path/example2.html`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/example2.html)
- [`shortes_path/example_shortest_path.html`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/example_shortest_path.html)
- [`shortes_path/example_shortest_path_2.html`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/example_shortest_path_2.html)
- [`shortes_path/networ.html`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/networ.html)

這些範例使用的前端資源位於 [`shortes_path/lib`](/Users/ren/Desktop/karen/git_karen/graph/shortes_path/lib)。


