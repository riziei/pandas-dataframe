# Stemming, Lemmatization, Stopwords and Regex in NLP using NLTK

## Overview

This project introduces important Natural Language Processing (NLP) preprocessing techniques using Python and NLTK. The notebook focuses on cleaning, normalizing, and preparing raw text data before applying machine learning or NLP models.

The project covers:

- Stopwords Removal
- Stemming
- Lemmatization
- Regular Expressions (Regex)

These preprocessing techniques are essential in almost every NLP pipeline because real-world text data is often noisy, inconsistent, and unstructured.


---

# Topics Covered

## 1. Introduction to NLP Preprocessing
- What is NLP preprocessing?
- Why preprocessing is important
- Role of preprocessing in NLP pipelines

---

## 2. Tokenization
- Word tokenization
- Breaking text into individual words
- Preparing text for preprocessing

---

## 3. What are Stopwords?
Stopwords are commonly used words that usually do not add significant meaning to text.

Examples:
- is
- the
- and
- in
- are

### Stopwords Removal
- Removing unnecessary words
- Reducing noise in text data
- Improving NLP model efficiency

---

## 4. What is Stemming?
Stemming reduces words to their root or stem form.

Examples:
- running → run
- studies → studi
- playing → play

### Porter Stemmer
- Most commonly used stemming algorithm in NLTK
- Fast and simple preprocessing method

### Advantages of Stemming
- Reduces vocabulary size
- Improves text normalization
- Faster preprocessing

### Limitations of Stemming
- May produce non-meaningful words
- Less accurate than lemmatization

---

## 5. What is Lemmatization?
Lemmatization converts words into meaningful base forms using vocabulary and grammar rules.

Examples:
- studies → study
- better → good
- flies → fly

### WordNet Lemmatizer
- Uses dictionary-based word normalization
- Produces meaningful words

### Advantages of Lemmatization
- More accurate preprocessing
- Produces readable base words
- Better for advanced NLP tasks

### Limitations of Lemmatization
- Slower than stemming
- Requires more linguistic processing

---

# Stemming vs Lemmatization

| Feature | Stemming | Lemmatization |
|--------|-----------|---------------|
| Output | Root form | Meaningful base word |
| Accuracy | Lower | Higher |
| Speed | Faster | Slower |
| Method | Rule-based | Dictionary + grammar |
| Example | studies → studi | studies → study |

---

## 6. Introduction to Regex in NLP

### What is Regex?
Regular Expressions (Regex) are patterns used to search, match, clean, and manipulate text data.

Regex is widely used in NLP preprocessing for handling noisy text.

---

## 7. Why Regex is Important in NLP

Regex helps:
- clean raw text
- remove punctuation
- remove numbers
- remove extra spaces
- extract useful patterns
- preprocess noisy text data

---

## 8. Common Regex Patterns

| Pattern | Meaning |
|--------|---------|
| `\d+` | Matches numbers |
| `\s+` | Matches multiple spaces |
| `[^\w\s]` | Removes punctuation |
| `[A-Za-z]+` | Extracts words |
| `\S+@\S+` | Extracts emails |
| `https?://\S+` | Extracts URLs |

---

## 9. Regex Applications in NLP

### Text Cleaning
- Removing punctuation
- Removing unwanted symbols
- Normalizing whitespace

### Information Extraction
- Email extraction
- Phone number extraction
- URL extraction

### Data Preparation
- Preparing clean text for tokenization
- Improving model input quality

---

# Libraries Used

- Python
- NLTK
- re (Regular Expressions)

---

# Installation

Install required library:

```bash
pip install nltk
```

---

# Download Required NLTK Data

```python
import nltk

nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
```

---

# Project Structure

```text
📂 NLP-Preprocessing
│── preprocessing_nltk.ipynb
│── regex_examples.ipynb
│── README.md
```

---

# NLP Preprocessing Pipeline

A basic NLP preprocessing pipeline includes:

1. Lowercasing text  
2. Removing punctuation using Regex  
3. Tokenization  
4. Stopwords removal  
5. Stemming  
6. Lemmatization  

---

# Example NLP Preprocessing Workflow

## Input Text

```text
"NLTK is AMAZING!!! It helps students learn NLP preprocessing techniques in 2025."
```

---

## After Cleaning and Preprocessing

```text
["nltk", "amazing", "helps", "students", "learn", "nlp", "preprocessing", "techniques"]
```

---

# Real-World Applications

These preprocessing techniques are used in:

- Chatbots
- Search engines
- Spam detection systems
- Sentiment analysis
- Resume parsing
- Recommendation systems
- Text classification
- Social media analysis

---

# Key Learnings

- Understanding NLP preprocessing fundamentals
- Cleaning raw text data
- Reducing noise using stopwords removal
- Normalizing text using stemming and lemmatization
- Using Regex for text cleaning and information extraction
- Building preprocessing pipelines for NLP projects

---

# Conclusion

NLP preprocessing is one of the most important stages in Natural Language Processing. Raw text data often contains noise, unnecessary words, punctuation, and inconsistencies that can reduce the performance of NLP models.

This project demonstrates how:
- stopwords removal improves text quality
- stemming reduces words to root forms
- lemmatization produces meaningful base words
- regex helps clean and extract patterns from text

These techniques form the foundation for advanced NLP applications such as sentiment analysis, machine learning models, chatbots, and information extraction systems.

---

