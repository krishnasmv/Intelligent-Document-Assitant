# Intelligent-Document-Assitant
Transformer-Based Abstractive Summarization using BART

Intelligent Document Assistant

Transformer-Based Abstractive Summarization using BART

# Overview

This project implements an intelligent document summarization system by fine-tuning a pretrained BART transformer model for abstractive text generation. The system generates concise summaries from long-form documents and evaluates performance using ROUGE metrics.

The model is trained and validated on the XSum and CNN/DailyMail datasets and benchmarked against a T5-small baseline for comparative performance analysis.

# Key Features

Fine-tuning of pretrained facebook/bart-base sequence-to-sequence transformer

Mixed-precision training with gradient accumulation

Combined training on XSum and CNN/DailyMail datasets

ROUGE-1, ROUGE-2, and ROUGE-L evaluation

Baseline comparison with T5-small

Real-time summary generation pipeline

Named Entity Recognition (NER) visualization using spaCy

# Tech Stack

PyTorch

Hugging Face Transformers

Datasets Library

ROUGE Score

spaCy

Matplotlib

# Model Architecture

The system uses BART (Bidirectional and Auto-Regressive Transformer), an encoder-decoder transformer architecture designed for sequence-to-sequence tasks such as summarization.

The encoder processes the input document, and the decoder generates a context-aware abstractive summary.

# Training Strategy

Tokenization with max input length of 1024 tokens

Gradient accumulation to stabilize training

Mixed precision (AMP) for computational efficiency

20 training epochs

AdamW optimizer

Beam search decoding during inference

# Evaluation

Model performance is evaluated using:

ROUGE-1

ROUGE-2

ROUGE-L

The fine-tuned BART model is compared against a pretrained T5-small model to assess summarization quality.

# Example Workflow

Input raw document

Preprocess and tokenize

Generate summary using trained BART model

Compute ROUGE score (optional)

Visualize named entities

# Future Improvements

PDF document upload support

Web-based interface (Streamlit/FastAPI)

Larger pretrained models (BART-large, T5-base)

Retrieval-Augmented Generation integration

This project demonstrates applied transformer fine-tuning, sequence-to-sequence modeling, model benchmarking, and real-world NLP pipeline development.
