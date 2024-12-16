## Coding Attention Mechanism

This folder contains everything about **Attention Mechanism** which include `simple self attention`, `causal self attention` and `multi head self attention`.

Attention mechanism is important in order to get the **Contextual Representation** of Longer Input text data.
**ATTENTION MECHANISM IS THE HEART OF LARGE LANGUAGE MODELS**

![Input Embedding of Token](../images/Embedding%20input.png)

## Why Self Attention Mechanism?

For most of the **Natural Language Processing** task we want a model to have a `Contextual Understanding and Grammar ALignment`. For that there are several Neural Networks like `RNN` which handles sequential data and is suitable for language understanding. RNN based `Encoder Decoder` were popular for most of the NLP task like `Text Summarization`, `Language Translation`, `Question Answering` or any other such **Sequence to Sequence** task.

The big issue and limitation of `Encoder Decoder RNNs` is that the RNN cant directly access earlier hidden states from the encoder during the decoding phase. Consequently, it depends on the hidden state of the decoder after each timestep which encapsulates all information. This lead to **long term dependency** problem causing the model to forget the context if the timestep is very long and for most sequential task yes the context is large.

Hence researchers developed `Bahdanau Attention` for RNNs so that the decoder can selectively access different parts of the input sequence at each decoding step. Then inspired from the `Bahdanau Attention` researchers developed `Self Attention Mechanism` in the original paper `Attention is all you need`.

`**Self-Attention**` Mechanism is a mechanism that allows the model to weight the importance of different words in a sequence relative to each other.Unlik other traditional RNN or CNN, self attention can consider all words in the sequence simultaneously making it highly `parallelizable and efficient`.

## A simple Self Attention

A simple self attention mechanism without any learnable weights.

- [Self Attention without Trainable Weights](./01_simple_sa.ipynb)
  ![Simple Self Attention](../images/Simple%20sa.png)

## Self Attention

Self Attention with trainable weight so that model can learn

- [Self Attention with Trainable Weights](./02_self_attention.ipynb)

![Self Attention](../images/self%20attention.png)

## Causal Self Attention

A causal self attention to mask the future tokens from accessing by the token

- [Causal Self Attention](./03_causal_sa.pynb)

## MultiHead Self Attention

A multihead version of self attention to get the multiple perspective and understaning of context

- [MultiHead Self Attention](./04_multihead_attention.ipynb)

![MultiHead Self Attention](../images/multihead%20self%20attention.png)
