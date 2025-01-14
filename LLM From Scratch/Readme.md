## Building a Large Language Model From Scratch

This folder contains building a `**Large Language Model**` completely from scratch.

## Large Language Model

A **large language model** is a neural network designed to understand, generate and respond to human like text. These networks are trained on very **large amount** of text data available on the internet. The large in the large language model means the model is trained for `language modeling` task utilizing large amount of textual data.

Large Language Model is trained with the task on `next word prediction` given the prior words and simply works on generating more texts one by one hence called `autoregressive` model. The first step of training an LLM is `PreTraining Step` where the model is trained on **raw text** meaning it is not labeled and just a raw text data. Then after **pretraining** step the model is further **Fine Tuned** for downstream tasks like **Text Classification**, **Summarization**, **Assistant Chatbot**, etc. The process of further training a pretrained LLM to downstream task is called `**Supervised Fine Tuning**` where a model is trained with human labeled data. Then further training is done for `Preference Alignment` using techniques like `DPO`, `PPO` and `RLHF`. So a pretrained model which is also called `Foundational Model` or `Base Model` can be further pretrained or Fine Tuned on smaller dataset for specific purpose. This is the basic summary of how a Large Language Model like GPT is trained on to be ChatGPT.

## Working with text

Here data is prepared to train our model with our **context size**, **embedding dimension** and **batch size**.

- [Tokenizing Text](./1.%20working%20with%20text/tokenization.ipynb)

## Attention Mechanism

Understanding Attention Mechanism

- [A simple attention mechanism](./2.Attention%20Mechanism/01_simple_sa.ipynb)
- [Self Attention](./2.Attention%20Mechanism/02_self_attention.ipynb)
- [Causal Self Attention](./2.Attention%20Mechanism/03_causal_sa.ipynb)
- [MultiHead Self Attention](./2.Attention%20Mechanism/04_multihead_attention.ipynb)

## Training GPT

Here Implementing GPT2 Architecture and PreTraining from Scratch to generate next token

- [GPT Model](./3.%20GPT/01_GPT.ipynb)
- [PreTraining GPT](./3.%20GPT/02_PreTraining_GPT.ipynb)

## Fine Tuning for Text Classification

Fine tuning the pretrained GPT2 Model for spam classification.

- [Fine Tuning for Text Classification](./4.%20Fine%20Tuning%20for%20Classification/FineTuning%20-Classification.ipynb)

## Instruction Fine Tuning

Fine tuning the pretrained GPT2 medium model for Instruction following.

- [Instruction Fine Tuning](./5.%20Instruction%20Fine%20Tuning/Instruction-FineTune.ipynb)