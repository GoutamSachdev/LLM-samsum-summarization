# SAMSum Dialogue Summarization with Flan T5-small

## Overview
This project focuses on training a sequence-to-sequence model for dialogue summarization using the Flan T5-small model architecture on the SAMSum dataset. The goal is to generate concise summaries for dialogues, capturing the key points of the conversation.

## Installation
Before running the code, make sure to install the required packages:

```bash
!pip install bitsandbytes
!pip install accelerate
!pip install --upgrade transformers
!pip install --upgrade peft
!pip install --upgrade datasets
```

## Usage
1. **Data Preprocessing:** The dataset (`samsum-train.csv` and `samsum-validation.csv`) is preprocessed to prepare it for training. This includes converting text columns to bytes and formatting the data for input into the model.

2. **Model Training:** The Flan T5-small model is fine-tuned for dialogue summarization using the prepared dataset. The model is configured with BitsAndBytes quantization and PEFT (Parameter Efficient Fine-Tuning) techniques for optimized performance.

3. **Evaluation:** The trained model is evaluated using the `samsum-validation` dataset. ROUGE scores are computed to assess the quality of generated summaries compared to reference summaries.

## Results
The trained model achieves impressive ROUGE scores, indicating its effectiveness in generating high-quality summaries for dialogues.

## Dependencies
- Python 3.x
- PyTorch
- Transformers
- BitsAndBytes
- PEFT
- Datasets

## Acknowledgements
- Flan T5-small model: [link](https://huggingface.co/google/flan-t5-small)

## Author
Goutam Sachdev
