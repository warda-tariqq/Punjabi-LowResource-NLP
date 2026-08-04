# Developing and Analyzing Punjabi Corpora in Gurmukhi and Shahmukhi Scripts: A Comparative Analysis of Word Embeddings for Low-Resource NLP

Official implementation accompanying the research paper:

> **Developing and Analyzing Punjabi Corpora in Gurmukhi and Shahmukhi Scripts: A Comparative Analysis of Word Embeddings for Low-Resource NLP**

This repository contains the complete implementation, training pipeline, evaluation scripts, and experimental notebooks used for constructing and evaluating Word2Vec embeddings for Punjabi in both the **Gurmukhi** and **Shahmukhi** writing systems.

---

## Project Overview

This study presents a comparative analysis of distributed word representations for Punjabi using two writing systems:

- Gurmukhi (India)
- Shahmukhi (Pakistan)

Four Word2Vec models were trained under identical hyperparameter settings:

- Gurmukhi CBOW
- Gurmukhi Skip-gram
- Shahmukhi CBOW
- Shahmukhi Skip-gram

The models were evaluated using multiple intrinsic evaluation methods including:

- Vocabulary Coverage
- Cosine Similarity
- Nearest Neighbor Analysis
- Principal Component Analysis (PCA)
- t-distributed Stochastic Neighbor Embedding (t-SNE)

---

## Repository Structure

```
Punjabi-LowResource-NLP/
│
├── notebooks/
│   ├── 01_corpus_statistics.ipynb
│   ├── 02_train_word2vec.ipynb
│   ├── 03_embedding_analysis.ipynb
│   └── 04_intrinsic_embedding_evaluation.ipynb
│
├── figures/
│   ├── workflow.png
│   ├── pca_visualization.png
│   ├── tsne_visualization.png
│   └── tables/
│
├── results/
│   ├── evaluation_tables.csv
│   ├── cosine_similarity.csv
│   └── nearest_neighbors.csv
│
├── requirements.txt
├── LICENSE
├── CITATION.cff
└── README.md
```

---

## Experimental Configuration

| Parameter | Value |
|-----------|------:|
| Embedding Algorithm | Word2Vec |
| Architectures | CBOW, Skip-gram |
| Vector Dimension | 200 |
| Context Window | 5 |
| Minimum Frequency | 5 |
| Epochs | 15 |
| Implementation | Gensim |
| Programming Language | Python |

---

## Trained Models

The trained Word2Vec models are publicly available on Hugging Face.

**Hugging Face**

https://huggingface.co/Wardatariqwt/Punjabi-Word2Vec-Embeddings

---

## Data Availability

The Punjabi corpora used in this study were compiled from multiple publicly available textual resources.

Because these source materials may be subject to different copyright and licensing conditions, the raw corpora are **not** redistributed through this repository.

This repository provides the complete implementation, preprocessing pipeline, experimental notebooks, evaluation scripts, and trained Word2Vec models required to reproduce the reported experiments.

---

## Requirements

Install the required packages using:

```bash
pip install -r requirements.txt
```

Main libraries:

- Python
- Gensim
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## Citation

If you use this repository in your research, please cite our paper.

```bibtex
@article{tariq2026punjabi,
  title={Developing and Analyzing Punjabi Corpora in Gurmukhi and Shahmukhi Scripts: A Comparative Analysis of Word Embeddings for Low-Resource NLP},
  author={Tariq, Warda},
  year={2026}
}
```

(The citation will be updated after publication.)

---

## Contact

**Warda Tariq**

PhD Researcher

Faculty of Computer Science

HSE University, Moscow

GitHub: https://github.com/warda-tariqq

Hugging Face: https://huggingface.co/Wardatariqwt

---

## License

This project is released under the MIT License. See the LICENSE file for details.
