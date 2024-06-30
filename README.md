# Fine-tuning Gemma using qLora and Supervised Fine-tuning

This repository contains a comprehensive notebook and tutorial on how to fine-tune the `gemma-7b-it` model using qLora and Supervised Fine-tuning.

## Overview

This project demonstrates the steps required to fine-tune the Gemma model for tasks like code generation. We use qLora quantization to reduce memory usage and the `SFTTrainer` from the `trl` library for supervised fine-tuning.

## Notebook

The notebook is available on my GitHub:
[gemma-Instruct-2b-Finetuning-on-alpaca.ipynb](https://github.com/MadhanMohanReddy2301/gemma-Instruct-2b-Finetuning-on-alpaca/blob/main/gemma-Instruct-Finetuning-on-alpaca.ipynb)

## Prerequisites

Before running the notebook, ensure you have the following:

1. **GPU**: 
   - [gemma-2b](https://huggingface.co/google/gemma-2b) can be fine-tuned on a T4 GPU (free on Google Colab).
   - [gemma-7b](https://huggingface.co/google/gemma-7b) requires an A100 GPU.
2. **Python Packages**: Install the necessary packages using the following commands:

   ```sh
   !pip3 install -q -U bitsandbytes==0.42.0 peft==0.8.2 trl==0.7.10 accelerate==0.27.1 datasets==2.17.0 transformers==4.38.0
   ```
