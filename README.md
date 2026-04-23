# SMS Spam Detection Using a From-Scratch LSTM

## Group Members

- Sejal Patel (SVP220003)
- Jennah Shahein (JXS220148)
- Afiya Syed (AXS220450)

---

## Project Description

This project implements a Long Short-Term Memory (LSTM) neural network from scratch using NumPy, without using PyTorch, TensorFlow, Keras, or any deep-learning library. The goal is to classify SMS messages as spam or ham using the SMS Spam Collection dataset.

All preprocessing, the LSTM forward pass, backpropagation through time (BPTT), and parameter updates were manually implemented.

---

## Dataset Source

The SMS Spam Collection dataset originally comes from UCI / Kaggle. For this project, the cleaned version is hosted publicly on GitHub (as required):
Dataset URL: https://github.com/jennah99/CS4375-spam-data/raw/refs/heads/main/spam.csv
GitHub URL: https://github.com/jennah99/CS4375-spam-data

The notebook automatically loads this dataset using the URL above, so no local files need to be uploaded.

---

## How to Run the Code (Google Colab)

1. Open Google Colab at https://colab.research.google.com
2. Upload the `CS_4375_Project_Code.ipynb` file into Colab
3. Run each cell from top to bottom, in order
4. The notebook automatically downloads the dataset from GitHub
   - No manual uploads are required
5. After the preprocessing section, the LSTM will begin training
   - Loss and accuracy prints will appear for each epoch

---

## Assumptions Made

- All sequences are padded/truncated to length 40
- Labels are binary: 0 = ham, 1 = spam
- Learning rate ∼ 0.001
- Embedding dimension = 50
- Hidden size = 64
- NumPy operations assume CPU execution
- The notebook sets np.random.seed(42).

---

## Libraries Used

- Only basic Python libraries were used:
  - NumPy: vectorized math operations
  - Pandas: loading and cleaning dataset
  - Matplotlib: loss and accuracy plots
- No deep learning frameworks were used.
- No NLP libraries (NLTK/spaCy) were used.
