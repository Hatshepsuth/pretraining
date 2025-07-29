# pretraining

# AI Assistant for Translation — Pretrained Model Weights

This repository contains the pretrained weights and model card for the multilingual neural machine translation model developed as part of the "AI Assistant for Translation" project.

---

## Overview

- **Model type:** Multilingual seq2seq transformer (e.g., based on facebook/m2m100_1.2B)
- **Supported languages:** English, French, German, Spanish, Italian, Russian (bidirectional)
- **Trained on:** Public parallel corpora (see below)
- **Intended use:** General-purpose and professional translation tasks, research, further fine-tuning and integration in downstream applications.

---

## License

The model weights and configuration files are distributed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).

You are free to use, modify, redistribute, and fine-tune the model, including for commercial purposes, subject to the terms of the Apache License 2.0.

---

## Training Data

- Publicly available datasets including OPUS, WMT, TED, Multi30k, ParaCrawl, Tatoeba (see documentation for full details)
- No private, proprietary, or confidential data was used for training.

---

## Intended Use & Limitations

- This model is intended for research, professional translation, and educational purposes.
- Not suitable for processing sensitive personal data without additional review and compliance.
- The model may contain biases present in the training data.

---

## How to Use

See example loading code with HuggingFace Transformers:

```python
from transformers import AutoModelForSeq2SeqLM, AutoTokenizer

tokenizer = AutoTokenizer.from_pretrained("your-org/your-model-name")
model = AutoModelForSeq2SeqLM.from_pretrained("your-org/your-model-name")
