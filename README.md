# NLU-Assignment-2
[This is the git repository of Assignment 2 done for the course NLU]

# Natural Language Understanding Assignment 2

This repository contains my implementation for two problems:

* **Problem 1:** Learning word embeddings using CBOW and Skip-gram
* **Problem 2:** Character-level name generation using RNN variants

Both problems were implemented from scratch without using high-level libraries like gensim.

---

##  Repository Structure

```
├── Prob1.ipynb          # Word2Vec (CBOW + Skip-gram)
├── Prob2.ipynb          # Name generation models (RNN, BLSTM, Attention)
├── report.pdf           # Detailed report with analysis and results
├── TrainingNames.txt    # Training names used for problem 2
├── corpus.txt           # Final cleaned corpus for problem 1
├── README.md
```

---

## Requirements

The code was written in Python. You’ll need the following libraries:

* numpy
* torch
* matplotlib
* sklearn
* wordninja

The .ipynb notebooks contain the commands to install these libraries. If you are using jupyter notebook just run the code cells squentially.
Alternatively,
You can install them using:

```bash
pip install numpy torch matplotlib scikit-learn wordninja
```

---

## How to Run

### Problem 1 (Word Embeddings)

1. Open `Prob1.ipynb`
2. Make sure all dataset files are in the correct path (as used in the notebook)
3. Run all cells sequentially

This notebook:

* preprocesses text data
* trains CBOW and Skip-gram models
* evaluates using cosine similarity and analogies
* visualizes embeddings using PCA

---

### Problem 2 (Name Generation)

1. Open `Prob2.ipynb`
2. Ensure the dataset file containing names is available
3. Run all cells in order

This notebook:

* preprocesses names into character sequences
* trains:

  * Vanilla RNN
  * Bidirectional LSTM
  * RNN with Attention
* generates new names from trained models

---
📂 Dataset
Problem 1 (Word Embeddings)

The dataset was created by collecting text from the IIT Jodhpur website, including:

department pages
research sections
academic regulations
course and syllabus documents
details of which are provided in the report.

The text was converted into .txt format and combined into a single corpus after preprocessing.

Due to size and redundancy, the raw dataset files are not included in this repository, only the final corpus is uploaded.

---
## 📊 Notes

* Training may take some time depending on your system
* Some outputs (especially in Problem 2) may vary due to randomness
* Models were trained for a limited number of epochs for experimentation purposes

---

## 📄 Report

A detailed explanation of:

* dataset collection and
preparation
* model architectures
* experiments and observations
* qualitative and quantitative analysis

is available in `report.pdf`.

---

## 💡 Final Thoughts

This assignment was mainly focused on understanding how these models behave internally rather than just getting perfect outputs. Some m

