# Neural-Machine-Translation-Tool-with-Hugging-Face
A modular Neural Machine Translation (NMT) tool powered by Hugging Face Transformers and MarianMT, featuring batch processing and automatic GPU/MPS acceleration for high-quality language translation.

# 🌍 Neural Machine Translation Tool with Hugging Face

This project implements a production-ready **Neural Machine Translation (NMT)** system using pretrained transformer models. By leveraging the **MarianMT** architecture via the Hugging Face ecosystem, the tool provides high-quality translations across hundreds of language pairs.

## 🚀 Features
* **Modular Design:** Encapsulated logic in a reusable `LanguageTranslator` class.
* **Hardware Acceleration:** Automatic detection and utilization of CUDA (NVIDIA), MPS (Apple Silicon), or CPU.
* **Batch Processing:** Efficiently translates multiple sentences simultaneously to maximize throughput.
* **High-Quality Decoding:** Uses Beam Search (`num_beams=4`) to ensure more accurate translation sequences than standard greedy search.

## 🛠️ Technology Stack
* **Backend:** [PyTorch](https://pytorch.org/)
* **NLP Framework:** [Hugging Face Transformers](https://huggingface.co/docs/transformers/index)
* **Models:** [MarianMT (OPUS-MT)](https://huggingface.co/Helsinki-NLP)
* **Tokenization:** SentencePiece & Sacremoses

## 📋 Installation

Ensure you have Python installed, then install the required dependencies:

```bash
pip install transformers sentencepiece sacremoses torch
