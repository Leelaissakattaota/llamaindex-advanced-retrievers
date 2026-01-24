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
| **Vector Index** | [cite_start]Semantic search based on vector embeddings[cite: 14, 51]. | [cite_start]General Q&A and RAG[cite: 15, 16]. |
| **BM25** | [cite_start]Keyword-based search using exact term matching[cite: 21, 22]. | [cite_start]Technical documents[cite: 46]. |
| **Document Summary** | [cite_start]Filters documents based on generated summaries before retrieval[cite: 26, 56]. | [cite_start]Large, diverse document sets[cite: 11, 49]. |
| **Auto Merging** | [cite_start]Consolidates child nodes into parent nodes to preserve context[cite: 30, 32]. | [cite_start]Long, complex documents[cite: 47]. |
| **Recursive** | [cite_start]Follows references (like citations) across document layers[cite: 33, 34]. | [cite_start]Research papers[cite: 48]. |
| **Query Fusion** | [cite_start]Combines results from multiple retrievers using fusion strategies[cite: 37, 60]. | Ambiguous or complex queries. |

---

## 🛠️ Advanced Fusion Strategies
[cite_start]We explore sophisticated merging techniques supported by LlamaIndex[cite: 40]:
* [cite_start]**Reciprocal Rank Fusion (RRF):** Robust ranking without relying on score magnitudes[cite: 41].
* [cite_start]**Relative Score Fusion:** Normalizes scores to preserve retriever confidence[cite: 42].
* [cite_start]**Distribution-Based Fusion:** Uses statistical normalization (z-scores) for score variability[cite: 43].

---

## ⚙️ Setup & Requirements
To run the notebook locally, install the following:
```bash
pip install llama-index llama-index-llms-ibm llama-index-embeddings-huggingface rank-bm25 PyStemmer ibm-watsonx-ai
