# Sentence Embedding & Cosine Similarity

## Overview

This repository demonstrates a fundamental Natural Language Processing (NLP) technique for measuring semantic similarity between two text sentences using **Sentence Transformers** and **Cosine Similarity**.

The implementation utilizes the pretrained `all-MiniLM-L6-v2` model to convert textual inputs into dense vector embeddings and calculates their similarity using cosine similarity.

## Objectives

- Understand sentence embeddings in NLP.
- Generate semantic vector representations using a pretrained Transformer model.
- Implement cosine similarity for comparing sentence embeddings.
- Explore how sentence meaning can be represented and compared numerically.

## Technologies & Libraries

- **Python** – Implementation language.
- **Sentence Transformers** – Generating sentence embeddings.
- **PyTorch** – Tensor-based embedding operations.
- **all-MiniLM-L6-v2** – Pretrained sentence embedding model.

## Implementation Workflow

1. Import `SentenceTransformer` and `util` from the Sentence Transformers library.
2. Load the pretrained `all-MiniLM-L6-v2` model.
3. Define two sample text sentences.
4. Generate vector embeddings using `model.encode()`.
5. Calculate cosine similarity using `util.cos_sim()`.
6. Extract and display the similarity score.

## Core Concepts

### 1. Sentence Embeddings

Sentence embeddings are numerical vector representations of textual sentences. They capture semantic information, allowing text to be compared mathematically.

### 2. Cosine Similarity

Cosine similarity measures the angular similarity between two vectors.

The mathematical formula is:

\[
\text{Cosine Similarity}(A,B)=
\frac{A\cdot B}{\|A\|\|B\|}
\]

Where:
- A and B represent sentence embedding vectors.
- A · B represents their dot product.
- ||A|| and ||B|| represent their vector magnitudes.

A higher positive score generally indicates greater semantic similarity in this embedding space.

## Project Structure

```text
Sentence-Embedding-Cosine-Similarity/
│
├── 14_LLM_Cosine_Similarity.py
├── requirements.txt
└── README.md
```

## Installation & Execution

### 1. Clone the repository

```bash
git clone https://github.com/USERNAME/Sentence-Embedding-Cosine-Similarity.git
```

### 2. Navigate to the project directory

```bash
cd Sentence-Embedding-Cosine-Similarity
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the implementation

```bash
python 14_LLM_Cosine_Similarity.py
```

**Note:** The pretrained model may be downloaded automatically when executed for the first time.

## Expected Output

The program displays the two input sentences followed by their calculated cosine similarity score.

The example compares:

- Sentence 1: "I Don't love to play cricket"
- Sentence 2: "I love to play cricket"

The resulting score represents the semantic similarity between their generated embeddings. The score should not be interpreted as a direct measure of logical agreement or contradiction.

## Applications

Cosine similarity and sentence embeddings are useful in several NLP applications:

- Semantic Search
- Document Similarity
- Text Matching
- Information Retrieval
- Question Answering Systems
- Retrieval-Augmented Generation (RAG)

## Learning Outcome

This implementation provides practical exposure to pretrained sentence embedding models, vector representations, and similarity measurement techniques used in modern NLP and LLM-based applications.

## Author

**Aarti Wamane**

GitHub: [aartiwamane](https://github.com/aartiwamane)

LinkedIn: [Aarti Wamane](https://linkedin.com/in/aarti-wamane-5276562a6)

---

*An educational implementation exploring semantic representations and similarity measurement in Natural Language Processing.*
