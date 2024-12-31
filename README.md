# Enhanced Sarcasm Detection with Attention Network

This project focuses on improving sarcasm detection in text, specifically news headlines, by leveraging advanced natural language processing techniques. By integrating CNNs, BiLSTMs, and a custom Attention Mechanism, the proposed model achieves state-of-the-art performance using sentence embeddings from Word2Vec, GloVe, and BERT.

---

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Methodology](#methodology)
- [Dataset](#dataset)
- [Results](#results)
- [Conclusion](#conclusion)
- [Acknowledgments](#acknowledgments)

---

## Introduction

Sarcasm detection is a challenging task in computational linguistics due to its reliance on subtle contextual cues, tone, and cultural references. This research addresses these challenges using a combination of neural network architectures and embeddings to identify sarcasm in textual data.

Key objectives:
- Enhance sarcasm detection accuracy by leveraging contextual and semantic information.
- Experiment with multiple word embeddings to optimize model performance.
- Provide a robust framework applicable to sarcasm detection and broader NLP tasks.

---

## Features
- **Integrated Architecture**: Combines CNNs, BiLSTMs, and a custom Attention Mechanism.
- **Advanced Sentence Embeddings**: Utilizes Word2Vec, GloVe, and BERT embeddings for semantic representation.
- **Dynamic Attention Mechanism**: Focuses on pivotal elements within sentences to identify nuanced sarcastic cues.
- **Scalable Design**: Processes datasets with varying sentence lengths using bucket-based embeddings.

---

## Methodology

1. **Sentence Embeddings**:
   - **Word2Vec**: Average embeddings for semantic representation.
   - **GloVe**: Pre-trained vectors for contextual understanding.
   - **BERT**: Concatenation of three hidden states to capture rich contextual nuances.

2. **Model Architecture**:
   - **CNNs**: Extract local features and patterns in text.
   - **BiLSTMs**: Capture sequential dependencies bidirectionally.
   - **Attention Mechanism**: Dynamically assigns weights to sentence parts for nuanced sarcasm detection.

3. **Proposed Model**:
   - Combines BiLSTM with 128 units and dropout (0.3) with a tuned attention mechanism.
   - Uses positional encodings with BERT embeddings to enhance attention focus.

---

## Dataset

- **Source**: News Headlines Dataset for Sarcasm Detection.
- **Size**: 28,620 entries (sarcastic and non-sarcastic labels).
- **Data Quality**: High-quality, professionally written headlines with minimal errors.

Data Preprocessing includes:
- Text cleaning and tokenization.
- Histogram analysis of word counts and average word lengths for sarcastic vs. non-sarcastic text.
- Wordcloud visualization for frequently occurring terms.

---

## Results

Performance metrics (accuracy) of different models with embeddings:

| Model            | Word2Vec | GloVe | BERT |
|------------------|----------|-------|------|
| CNNs             | 0.64     | 0.605 | 0.71 |
| BiLSTMs          | 0.62     | 0.73  | 0.70 |
| Attention Model  | 0.72     | 0.64  | 0.60 |
| **Proposed Model** | 0.70     | 0.69  | **0.81** |

Key observations:
- The proposed model performs best with BERT embeddings due to its ability to capture both local and global dependencies.
- Performance increases with LSTM cell units (up to 128) but decreases beyond due to overfitting.

---

## Conclusion

This research successfully enhances sarcasm detection by integrating advanced embedding techniques with a novel neural architecture. The proposed model demonstrates superior performance on high-quality datasets, paving the way for advancements in sentiment analysis and natural language understanding.

---

## Acknowledgments

We extend our gratitude to the following contributors:
- **Darshan R K**
- **A D Mahit Nandan**
- **Dr. Anand Kumar M**

