### Interpreting Induction Circuits in Transformers

This repository documents my implementation and exploration of Mechanistic Interpretability using TransformerLens, centered around understanding Induction Circuits - one of the first mechanistically understood algorithms discovered inside transformer language models

### Breaking Open the Black Box

I began by learning how to inspect transformer internals using TransformerLens, exploring model architecture, tokenization, attention patterns, activation caches, and hidden representations. This provided the foundation for studying model behavior beyond its final predictions

### Discovering Induction Heads

The next step was understanding Induction Heads - attention heads that recognize repeated patterns in a sequence and use earlier occurrences to predict what comes next. By analyzing attention patterns on repeated-token sequences, I identified these heads and developed an intuition for the algorithm they implement

### Looking Beyond Attention

Attention visualizations alone don't explain why a model behaves the way it does. To move from observation to explanation, I explored hooks, activation patching, direct logit attribution, and targeted ablations to measure how individual components causally contribute to model predictions

### Reverse Engineering the Circuits

Finally, I moved beyond activation analysis and investigated the model directly through its learned weights. By analyzing QK and OV circuits, composition scores, and factored matrices, I reconstructed the induction circuit itself, understanding not only which heads are responsible for in-context learning, but how they cooperate to implement the underlying algorithm

### Acknowledgement

- Independently studied Alignment Research Engineer Accelerator curriculum. My sincere thanks to whole ARENA team, Neel Nanda and all contributors for creating one of highest quality open educational resources on AI Safety ❤️
- https://www.lesswrong.com/posts/TvrfY4c9eaGLeyDkE/induction-heads-illustrated - This blog post genuinely helped me a lot till the end in visualising and getting intution of induction heads, previous token head, induction circuits and K composition 
