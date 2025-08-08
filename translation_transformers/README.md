# German-to-English Neural Machine Translation Using Transformers

This project implements a sequence-to-sequence Transformer model from scratch in PyTorch to perform German-to-English translation on the Multi30K dataset. The goal is to build a neural machine translation (NMT) system that learns to translate German sentences into English using the Transformer architecture introduced by Vaswani et al. (2017).

---

## Project Overview

- **Dataset:** Multi30K (English-German parallel corpus)
- **Model:** Custom implementation of the Transformer encoder-decoder architecture
- **Key Features:**
  - Token embedding and positional encoding
  - Multi-head self-attention with masking to prevent future token leakage
  - Custom greedy decoding for sequence generation
  - Training with cross-entropy loss
  - Evaluation using BLEU score to quantify translation quality

---

## Architecture Details

- **Encoder:** Processes the input German sentence to generate contextual embeddings.
- **Decoder:** Autoregressively generates English translation tokens, conditioned on encoder outputs and previously generated tokens.
- **Masking:** Implemented causal masking in the decoder to ensure the model only attends to earlier tokens during training and inference.
- **Positional Encoding:** Adds positional information to token embeddings to maintain word order awareness.

---

## Requirements

- Python 3.7+
- PyTorch
- TorchText
- NumPy
- SacreBLEU (for BLEU score evaluation)
- tqdm

Or just copy paste the 'Importing Required Libraries' section from the notebook above.

## Inference Process
<img width="1357" height="1583" alt="transformer inference process" src="https://github.com/user-attachments/assets/2c52e4bb-905b-4b8a-82e8-2643ec67d5e1" />



