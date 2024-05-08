# Supervised Fine-Tuning (SFT) of an LLM

In this notebook, we illustrate step 2 of creating a ChatGPT at home, which involves supervised fine-tuning (SFT) or instruction tuning. 

SFT takes a pre-trained base model, obtained from step 1 (pre-training a large language model on internet-scale data), and fine-tunes it on human instruction data using cross-entropy loss. This process aims to turn the base model into a chatbot or assistant that can generate useful completions given instructions.

## Overview

1. **Introduction**: Brief overview of supervised fine-tuning.
2. **Hardware Requirements**: Hardware specifications required for running the notebook efficiently.
3. **Environment Setup**: Installation of necessary libraries and tools.
4. **Data Preparation**: Loading and preprocessing the SFT dataset from the 🤗 hub.
5. **Model Fine-Tuning**: Fine-tuning the Mistral-7B base model using the prepared dataset.
6. **Evaluation**: Evaluating the fine-tuned model's performance.
7. **Conclusion**: Summary and closing remarks.

## Hardware Requirements

This notebook is designed to be run on any NVIDIA GPU with the Ampere architecture or later and at least 24GB of RAM. This includes GPUs such as NVIDIA RTX 3090, 4090, A100, H100, and H200. 

The requirement for Ampere architecture is due to the use of bfloat16 (bf16) format, which is not supported on older architectures like Turing. However, tweaks are provided to train the model in float16 (fp16), which is supported by older GPUs like NVIDIA RTX 2080, Tesla T4, and V100.

## Environment Setup

We install necessary libraries and tools including:
- Transformers for the LLM
- Datasets for loading and preprocessing SFT dataset
- BitsandBytes and PEFT for fine-tuning the model on consumer hardware
- TRL library for useful Trainer classes for LLM fine-tuning.
