## Transformers
- Until self attention in the OG transformers except the input embeddings there is no learnable params Once MHA comes in, the parameterized Wq, Wk,Wv with sequence, d_model.

- A scaled self attention block takes in the input with shape seq, d_model and outputs the same seq, d_model but now they are contextualized embedings(where each token has attended to every other tokens in the sequence)

- The final linear layer will project the output in seq, vocab_size then apply softmax

- In Cross Attention, the KV comes from Encoder(<SOS> . .  . <EOS>, Q comes from decoder (starts with <SOS>) and is fixed, so we can KV cache to speed up.  

