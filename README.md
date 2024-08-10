# Document Similarity Search with HNSW and Multilingual Embeddings

![HNSW](https://github.com/user-attachments/assets/c2df5539-3895-4fa9-b276-9ce8fd91d77a)



Memory updated
Here’s a section you can add to your GitHub README to explain the Hierarchical Navigable Small World (HNSW) algorithm:

# Hierarchical Navigable Small World (HNSW) Algorithm
The HNSW algorithm is a powerful method for approximate nearest neighbor search, providing a balance between search accuracy and computational efficiency. Here's an overview of how it works:

## 1. Hierarchical Structure
HNSW organizes data into a multi-layered structure, where each layer forms a navigable small world graph.

Top Layers: These layers contain fewer nodes and have more sparse connections. They provide a high-level view of the data and help in quickly narrowing down the search space.
Lower Layers: These layers have more nodes and denser connections, offering a more detailed view and finer granularity in the search.
## 2. Navigability
The algorithm leverages the small world property of these graphs to efficiently navigate through nodes:

High-Level Navigation: Starting from the top layers, HNSW quickly narrows down to a relevant region of the graph where nearest neighbors are likely to be located.
Greedy Search: The search is performed greedily, meaning that at each step, the algorithm moves to the closest neighbor, rapidly converging towards the target.
## 3. Search Process
The search process in HNSW involves:

Starting at the Top Layer: The algorithm begins at the top layer and performs a search to find the closest nodes.
Refining the Search: As it moves down to lower layers, the search is refined by exploring denser connections, ultimately finding approximate nearest neighbors efficiently.
## 4. Approximation
HNSW is an approximate nearest neighbor search algorithm, which:

Trade-Offs: Sacrifices some accuracy in exchange for significantly faster search speeds and reduced memory usage.
Efficiency: Designed to provide a good balance between search accuracy and computational efficiency, making it suitable for high-dimensional data and large datasets.


This project demonstrates how to perform document similarity search using the Hierarchical Navigable Small World (HNSW) algorithm combined with multilingual embeddings. It also includes visualizations to show document embeddings and their relationships.

## Features

- **Multilingual Embeddings**: Use `intfloat/multilingual-e5-large-instruct` for encoding English and Bengali documents.
- **Hierarchical Navigable Small World (HNSW) Index**: Efficiently search for similar documents.
- **Visualization**: Plot document embeddings and visualize the connections between a query and similar documents.

## Prerequisites

Ensure you have the following Python packages installed:

- `hnswlib`
- `numpy`
- `sentence-transformers`
- `sklearn`
- `matplotlib`
- `transformers`

You can install the required packages using pip:

```bash
pip install hnswlib numpy sentence-transformers scikit-learn matplotlib transformers
