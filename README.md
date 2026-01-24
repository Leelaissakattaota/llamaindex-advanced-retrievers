# 🔍 Advanced Retrieval Strategies with LlamaIndex & watsonx.ai

[![LlamaIndex](https://img.shields.io/badge/Powered%20by-LlamaIndex-blue)](https://www.llamaindex.ai/)
[![IBM Watsonx](https://img.shields.io/badge/Model-IBM%20watsonx.ai-purple)](https://www.ibm.com/watsonx)
[![Python](https://img.shields.io/badge/Language-Python-yellow)](https://www.python.org/)

This project explores **Advanced Information Retrieval** techniques using the LlamaIndex framework and IBM watsonx.ai foundation models. It covers sophisticated search strategies designed to enhance **Retrieval-Augmented Generation (RAG)** applications.

---

## 🌟 Key Features & Retrievers
We implement and compare several advanced retrieval methods to improve accuracy and context preservation:

| Retriever Type | Core Functionality | Best Use Case |
| :--- | :--- | :--- |
| **Vector Index** | Semantic search based on vector embeddings. |General Q&A and RAG. |
| **BM25** | Keyword-based search using exact term matching. | Technical documents. |
| **Document Summary** | Filters documents based on generated summaries before retrieval. | Large, diverse document sets. |
| **Auto Merging** | Consolidates child nodes into parent nodes to preserve context. | Long, complex documents. |
| **Recursive** | Follows references (like citations) across document layers. | Research papers. |
| **Query Fusion** | Combines results from multiple retrievers using fusion strategies. | Ambiguous or complex queries. |

---

## 🛠️ Advanced Fusion Strategies
We explore sophisticated merging techniques supported by LlamaIndex:
* **Reciprocal Rank Fusion (RRF):** Robust ranking without relying on score magnitudes.
* **Relative Score Fusion:** Normalizes scores to preserve retriever confidence.
* **Distribution-Based Fusion:** Uses statistical normalization (z-scores) for score variability.

---

## ⚙️ Setup & Requirements
To run the notebook locally, install the following:
```bash
pip install llama-index llama-index-llms-ibm llama-index-embeddings-huggingface rank-bm25 PyStemmer ibm-watsonx-ai
