# 📚 Google Gemma 3.4B-IT - Image-Text-to-Text Pipeline

This project demonstrates how to use Google's **Gemma-3-4B-IT** model for **image-text-to-text generation** using Hugging Face's `transformers` library.

## 🚀 Project Overview

- **Model Used:** `google/gemma-3-4b-it`
- **Task:** Image + Text → Text generation
- **Platform:** Google Colab
- **Framework:** Hugging Face Transformers (`v4.49.0-Gemma-3`)

## 🛠️ Setup

Install the specific version of `transformers` with Gemma-3 support:

```bash
pip install -q git+https://github.com/huggingface/transformers@v4.49.0-Gemma-3
```

## 🧩 Usage

Import necessary libraries and initialize the pipeline:

```python
import torch
from transformers import pipeline

pipe = pipeline(
    "image-text-to-text",
    model="google/gemma-3-4b-it",
    device="cuda",
    torch_dtype=torch.bfloat16
)
```

You can now use this pipeline to generate text from images and prompts!

## 📖 References

- [Gemma 3 Official Blog on Hugging Face](https://huggingface.co/blog/gemma3)
