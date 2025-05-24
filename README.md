# Neural and Generative Information Retrieval Methods

## Overview
This project implements various information retrieval (IR) methods with the goal of documenting, evaluating and comparing the effectiveness of different IR techniques, especially focussing on methods based on neural networks. The methods implemented in this project include:
- **BM25** (traditional non-neural IR method used as a baseline)
- **DPR**: Dense Passage Retrieval
- **TILDEv2**: Term-Independent Latent Document Expansion
- **RAG**: Retrieval Augmented Generation

Additionally, reranking pipelines for reordering the order of relevant documents retrieved by the above methods were also implemented. Specifically, pointwise reranking (scoring documents independently to determine order) and pairwise reranking (scoring pairs of documents to determine order) are used in this project.

To evaluate the performance of the IR techniques implemented, multiple metrics are considered:
- **nDCG**: Normalised Discounted Cumulative Gain
- **BLEU**: Bilingual Evaluation Understudy
- **ROGUE**: Recall-Oriented Understudy for Gisting Evaluation
- **Embedding Similarity**
- **LLM-based Evaluation**

## Project Files
```
neural-ir/
    README.md
    main.ipynb
    collection.zip
        sampled_collection.jsonl
        sampled_qrels.txt
        sampled_queries.tsv
    images/
```
- `README.md`: This README file.
- `main.ipynb`: Python notebook containing source code of the project.
- `collection.zip`: Zip file with corpus dataset and queries used in the project.
- `images/`: Supporting images used for documentation.