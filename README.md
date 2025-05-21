# NLP_NM_Hackathon

# Multilingual Translation with MBart-50

This project enables seamless machine translation between English and multiple Indian languages (Hindi, Telugu, Tamil, etc.) using the multilingual capabilities of the **mBART-50** model. It uses over 1 million bilingual sentence pairs and supports domain-specific adaptation for high-quality contextual translations.

## Model Overview

- **Model**: mBART-50 (Multilingual Bidirectional and Auto-Regressive Transformers)
- **Base Framework**: Hugging Face Transformers
- **Supported Languages**: English (`en_XX`) ↔ Hindi (`hi_IN`), Telugu (`te_IN`), Tamil (`ta_IN`)
- **Approach**: Preprocessing with language-specific tokens, fine-tuning on bilingual corpora

## 📂 Dataset

> **Note:** The dataset used includes over 1 million bilingual sentence pairs from publicly available corpora:

- [AI4Bharat IndicNLP Corpus](https://indicnlp.ai4bharat.org/parallel-corpora/)
- [IIT Bombay English-Hindi Parallel Corpus](http://www.cfilt.iitb.ac.in/iitb_parallel/)
- [OPUS (Tanzil, KDE, GNOME, etc.)](http://opus.nlpl.eu/)
- [Hugging face samantar dataset](https://huggingface.co/datasets/ai4bharat/samanantar)

All data is preprocessed and tokenized using `SentencePiece`, including language-specific tokens like `[en_XX]`, `[hi_IN]`, etc.

## Installation

```bash
git clone https://github.com/your-username/mbart50-indian-translation.git
cd mbart50-indian-translation
python -m venv env
source env/bin/activate  # or use env\Scripts\activate on Windows
pip install -r requirements.txt
```
