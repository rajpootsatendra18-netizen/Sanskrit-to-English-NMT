# Sanskrit to English Neural Machine Translation
Sanskrit to English Neural Machine Translation using MarianMT
## Overview
A seq2seq Neural Machine Translation system that translates Sanskrit text into English,
built by fine-tuning the Helsinki-NLP/opus-mt-mul-en (MarianMT) Transformer on a
parallel Sanskrit–English corpus.
## Architecture
- **Model**: MarianMT (6-layer Transformer encoder-decoder)
- **Pre-trained on**: OPUS multilingual corpus (includes Devanagari-script languages)
- **Decoding**: Custom Beam Search (width=4, length penalty, no-repeat-ngram)
- **Parameters**: ~74M
## Results
BLEU (NLTK) - 53.80
BERTScore F1 (rescaled)  - 0.9310
Inference Time - 213.70s (for 1000 sentences) 
