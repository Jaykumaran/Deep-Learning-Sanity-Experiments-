## Transformers
- Until self attention in the OG transformers except the input embeddings there is no learnable params Once MHA comes in, the parameterized Wq, Wk,Wv with d_model, d_model -> d_model, num_heads , d_model/num_heads.

- A scaled self attention block takes in the input with shape seq, d_model and outputs the same seq, d_model but now they are contextualized embedings(where each token has attended to every other tokens in the sequence)

- The final linear layer will project the output in seq, vocab_size then apply softmax

- In Cross Attention, the KV comes from Encoder("""< SOS> . .  . < EOS>""", Q comes from decoder (starts with < SOS>) and is fixed, so we can KV cache to speed up.


## Vision Transformers
- In ViT arent autoregressive so we dont apply any sort of masking unlike language tasks.
- To transformer model we need to give a batch of sequence so make sure the shape is from (B,embed_dim, num_patches) -> (B, num_patches, embed_dim)

