## Positional Encoding
Positional Encoding is a method introduced in the Attention is all you need paper to provide a sense of order to the sequence of tokens in a transformer model. It encodes positional information about the token in the sequence to get a notion of position since the model execute in parallel and we need some way to encode the position information.

## Types of Positional Encoding methods:
There are several ways we can encode position. There are **absolute and relative** positional encoding methods.

- Sinusoidal Positional Encoding (SPE)
- Relative Positional Encoding (RPE)
- Rotary Positional Encoding (RoPE)
- Attention with Linear Biases (AliBi)