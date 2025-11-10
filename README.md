<h1 align="center">🌐 Neural Machine Translation using Seq2Seq LSTM</h1>

<p align="center">
  <em>A Deep Learning project that translates text from one language to another using a <b>Sequence-to-Sequence (Seq2Seq)</b> model with <b>Encoder–Decoder LSTM</b> architecture built in TensorFlow and Keras.</em>
</p>

---

## 📘 Project Overview
This project demonstrates how to build a **Neural Machine Translation (NMT)** system — similar to how Google Translate works — using **Recurrent Neural Networks (RNN)** with **LSTM layers**.  
It is designed to translate text from a **source language (e.g., English)** to a **target language (e.g., Hindi/French)** by learning sentence-to-sentence mappings from a parallel dataset.

The model follows the **Encoder–Decoder** framework, where the **encoder** processes the input sequence and the **decoder** generates the translated output sequence, word by word.

---

## 🧠 Problem Statement
Given an input sentence in the source language, the model predicts its equivalent sentence in the target language.  
This project explores how deep learning can understand, encode, and generate human language, forming the foundation for applications like **chatbots**, **AI translators**, and **conversational systems**.

---

## 🧩 Dataset
- **Source:** Parallel corpus (English ↔ Target Language)  
- **Format:** Text files containing sentence pairs  

 - **Dataset Split:**
- 80% Training Data  
- 20% Testing Data  

Each sentence pair is preprocessed, tokenized, and aligned for training the translation model.

---

## 🧹 Data Preprocessing Workflow

1. **Text Cleaning**
 - Removed punctuation, lowercased text, and normalized special characters.
2. **Tokenization**
 - Split sentences into word-level tokens for both source and target languages.
3. **Vocabulary Creation**
 - Built `word-to-index` and `index-to-word` dictionaries.
4. **Padding**
 - Applied sequence padding to ensure uniform input lengths.
5. **Encoding**
 - Converted words into integer sequences suitable for LSTM input.
6. **Train-Test Split**
 - Split the dataset into training and testing subsets for evaluation.

---

## ⚙️ Model Building

| Step | Description |
|:----:|:-------------|
| **Architecture** | Encoder–Decoder Sequence-to-Sequence Model |
| **Encoder** | LSTM network that encodes input sentence into a context vector |
| **Decoder** | LSTM network that decodes context vector into translated output |
| **Embedding Layer** | Converts words into dense vector representations |
| **Dense Layer** | Softmax layer for word prediction |
| **Loss Function** | Categorical Crossentropy |
| **Optimizer** | Adam |
| **Evaluation Metric** | Accuracy |

### 🧱 Model Pipeline
Input Sentence → Tokenization → Padding → Encoder (LSTM)
→ Decoder (LSTM + Dense Softmax) → Translated Output


---

## 📈 Results

| Metric | Value |
|:--------|:------|
| **Training Accuracy** | ~90% |
| **Validation Accuracy** | ~88% |
| **Model Type** | Seq2Seq (Encoder–Decoder LSTM) |
| **Dataset** | Parallel Text Corpus |
| **Translation Example** | Input: *How are you?* → Output: *तुम कैसे हो?* |

---

## 🛠️ Tech Stack

| Category | Tools / Libraries |
|:----------|:------------------|
| **Language** | Python |
| **Deep Learning Framework** | TensorFlow / Keras |
| **Data Processing** | NumPy, Pandas |
| **Text Preprocessing** | re, NLTK |
| **Model Type** | Encoder–Decoder LSTM |
| **Environment** | Jupyter Notebook / Google Colab |

---

## 🚀 Future Improvements
- Integrate **Attention Mechanism** (Bahdanau or Luong) for better context understanding.  
- Implement **Bidirectional Encoder** and **Beam Search decoding**.  
- Experiment with **Transformer models** for comparison.  
- Deploy as an interactive **Web App** using Flask or Streamlit.

---

## 📦 About
This project showcases a complete workflow of **Neural Machine Translation using LSTM**, including data preprocessing, model training, and sequence decoding.  
It highlights the ability of deep learning models to learn linguistic patterns and perform **automatic text translation**.


