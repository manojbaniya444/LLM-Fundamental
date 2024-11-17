# Tokenization
Tokenization is the process of breaking down text into smaller units called tokens. These tokens can be words, character, subwords, or symbols depending on the specific method used for tokenization. It is a fundamental step in NLP and is crucial for any NLP task like for language modeling.

# When
Tokenization happens before vectrization.

# Why
- Input prepration
- Granularity contol: character level, word level, subword level
- Vocabulary management
- Feature extraction
- Dimensionality reduction

# How
- Text normalization (cleaning)
- Boundary detection (when start and end of token)
- Token extraction
- Token processing

Example:

`word-level tokenization`: ["I", "Love", "NLP"]

`character-level tokenization`: ["I", "L", "o", "v", "e", "N", "L", "P"]

`sub-word tokenization`: ["un", "defined"]
