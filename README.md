# 📖 Next Word Prediction with RNN vs LSTM

This project demonstrates the difference between a **Recurrent Neural Network (RNN)** and a **Long Short-Term Memory Network (LSTM)** by training both models on Shakespeare’s _Hamlet_ text to perform **next word prediction**.

---

## 🗂 Dataset

- Source: [NLTK Gutenberg Corpus](https://www.nltk.org/)
- Text used: _Shakespeare - Hamlet_
- Preprocessing steps:
  - Lowercasing the text
  - Tokenization into words
  - Creating **n-gram sequences**
  - Padding sequences to equal length
  - Splitting into **training (80%)** and **testing (20%)**

---

## 🧠 Model Architecture

Both models start with:

- **Embedding layer**: Converts words into dense vector representations.
- **Dropout layers**: Prevent overfitting.
- **Dense softmax layer**: Outputs probability distribution over the vocabulary.

The neural network is created with some number of layers for both the models.

---

## 🚀 Training

- Both models trained for **100 epochs** and it is found that RNN overfits andd gives better accuracy fot training data.
- Optimizer: Adam
- Loss: Categorical Crossentropy
- Metric: Accuracy

---

## Example Input

### "You are a"

- LSTM Prediction: 'gentleman'
- RNN Prediction: 'poyson'
