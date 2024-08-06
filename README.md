# Document Similarity Search with HNSW and Multilingual Embeddings

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
