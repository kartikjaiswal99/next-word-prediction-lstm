# Next Word Prediction with LSTM

This project implements a deep learning model that predicts the next word in a given input sequence using Long Short-Term Memory (LSTM) networks. The goal is to showcase how sequence modeling can be applied to natural language tasks like text completion or autocomplete.

---

## Project Highlights

- **Dataset:** Uses the complete text of Shakespeare’s *Hamlet* to train the model.
- **Architecture:** Embedding layer → Stacked LSTM layers → Dense softmax output.
- **Preprocessing:** Tokenization, sequence generation, and padding for uniform input.
- **Training:** Trained with categorical cross-entropy loss and early stopping to prevent overfitting.
---

## How It Works

1️⃣ **Prepare the data:**  
- Load Shakespeare’s *Hamlet*
- Clean and tokenize the text
- Generate input sequences and corresponding target words
- Pad sequences to a fixed length

2️⃣ **Build the model:**  
- Add an embedding layer to learn word representations
- Stack two LSTM layers to capture context
- Use a dense layer with softmax to output probabilities for the next word

3️⃣ **Train the model:**  
- Use categorical cross-entropy loss and Adam optimizer
- Monitor validation loss.
