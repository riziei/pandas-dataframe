# Document Similarity using TF-IDF and Cosine Similarity

## Overview

This project demonstrates how to measure similarity between text documents using Natural Language Processing (NLP) techniques.

The notebook uses **TF-IDF (Term Frequency-Inverse Document Frequency)** and **Cosine Similarity** to convert text into numerical vectors and determine how similar documents are to one another.

---

## Topics Covered

* Introduction to Document Similarity
* TF-IDF Representation
* Cosine Similarity
* Document-to-Document Comparison
* Similarity Matrix Analysis
* Building a Simple Document Similarity Tool
* Applications of Document Similarity

---

## Libraries Used

* Python
* Scikit-learn
* Pandas
* NumPy
* Regular Expressions (re)

---

## Installation

Install the required libraries:

```bash
pip install scikit-learn pandas numpy
```

---

## Project Structure

```text
Document-Similarity/
│
├── document_similarity.ipynb
└── README.md
```

---

## Workflow

1. Load text documents
2. Preprocess text data
3. Convert documents into TF-IDF vectors
4. Calculate cosine similarity scores
5. Analyze similarity between documents
6. Build a simple document similarity tool

---

## Key Concepts

### TF-IDF (Term Frequency-Inverse Document Frequency)

TF-IDF converts text into numerical vectors by assigning weights to words based on their importance within a document and across a collection of documents.

### Cosine Similarity

Cosine Similarity measures the similarity between two document vectors. The score ranges from:

* **1.0** → Identical documents
* **0.0** → Completely different documents

---

## Features

* TF-IDF Vectorization
* Cosine Similarity Calculation
* Similarity Matrix Generation
* Document Comparison
* Reusable Similarity Function

---

## Applications

* Search Engines
* Recommendation Systems
* Chatbots
* Plagiarism Detection
* Resume Matching
* Information Retrieval Systems

---

## Key Learnings

* Converting text into numerical representations
* Understanding TF-IDF weighting
* Measuring document similarity using cosine similarity
* Building a basic NLP retrieval system
* Applying NLP techniques to real-world problems

---



## Conclusion

Document similarity is a fundamental NLP task used in search engines, recommendation systems, chatbots, and information retrieval applications. By combining TF-IDF and Cosine Similarity, we can efficiently compare documents and identify related content.

This project provides a practical introduction to document similarity and serves as a foundation for more advanced NLP techniques.

---