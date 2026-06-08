# Day 15 - RNN and LSTM for Next Word Prediction

## Overview

In today's task, I studied and implemented **Recurrent Neural Networks (RNNs)** and **Long Short-Term Memory (LSTM)** models for a simple **next-word prediction task**.

The goal was to understand how sequential models process text data and how LSTM improves memory handling compared to standard RNNs.

---

## Objectives

- Understand sequential data processing in NLP  
- Learn how RNN works for text prediction  
- Understand vanishing gradient problem  
- Implement LSTM to improve long-term memory learning  
- Compare RNN vs LSTM performance  

---

## Dataset

A small custom dataset was used:

```text
i love nlp
nlp is amazing
deep learning is powerful
machine learning uses data
artificial intelligence is fascinating
```

---

## Workflow

### 1. Text Preprocessing
- Converted sentences into lowercase text
- Tokenized words using Keras Tokenizer
- Converted words into numerical sequences

---

### 2. Sequence Generation
Created input-output pairs for training:

Example:
```text
Input  → i love
Output → nlp
```

---

### 3. Padding
All sequences were padded to equal length using:

```python
pad_sequences()
```

---

### 4. One-Hot Encoding
Output words were converted into categorical format for classification.

---

## RNN Model

### Architecture

- Embedding Layer
- SimpleRNN Layer
- Dense Output Layer

```python
Embedding(vocab_size, 10)
SimpleRNN(32)
Dense(vocab_size, activation='softmax')
```

---

### Training

- Optimizer: Adam  
- Loss: Categorical Crossentropy  
- Epochs: 100  

---

### Observation

- RNN learns short-term dependencies well  
- Struggles with long context understanding  

---

## Vanishing Gradient Problem

RNN suffers from vanishing gradients:

- Gradients become very small during backpropagation  
- Model forgets earlier information in long sequences  
- This limits learning of long-term dependencies  

---

## LSTM Model

### Architecture

- Embedding Layer  
- LSTM Layer  
- Dense Output Layer  

```python
Embedding(vocab_size, 10)
LSTM(32)
Dense(vocab_size, activation='softmax')
```

---

### Why LSTM?

LSTM solves vanishing gradient using:

- Forget Gate  
- Input Gate  
- Output Gate  

This helps it remember important information for longer sequences.

---

## Comparison: RNN vs LSTM

| Feature | RNN | LSTM |
|--------|-----|------|
| Memory | Short-term | Long-term |
| Performance | Basic | Better in general |
| Complexity | Simple | Complex |
| Vanishing Gradient | Yes | No (mostly solved) |

---

## Results

| Model | Accuracy |
|------|----------|
| RNN | 0.615 |
| LSTM | 0.308 |

### Insight:
- RNN performed better on small dataset  
- LSTM requires larger datasets to perform well  
- LSTM is more powerful but data-hungry  

---

## Key Learnings

- How sequential models process text  
- How tokenization converts text to numbers  
- How RNN learns word sequences  
- Why vanishing gradient is a problem  
- How LSTM solves memory limitations  
- Importance of dataset size in deep learning  

---

## Tools Used

- Python  
- TensorFlow / Keras  
- NumPy  
- NLP preprocessing techniques  

---

## Conclusion

RNN and LSTM are foundational models in NLP.  
RNN is simple and works for short patterns, while LSTM is designed for long-term dependencies.

However, model performance strongly depends on dataset size and training quality.

---

## Future Improvements

- Train on larger datasets  
- Use GRU instead of LSTM  
- Experiment with different embedding sizes  
- Add real-world text corpus  
- Try Transformer-based models  

---