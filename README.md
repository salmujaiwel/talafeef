## Talafeef

This project was built entirely from scratch, starting with the collection of Arabic corpora and the development of automatic POS tagging and lemmatization tools, while also creating word-embedding models using the project's data to empirically observe how these models function.

Information about the corpora
  - Standard--Academic: 10,512 tokens
  - Standard-- Khutbah: 10,380 tokens
  - Standard--Newspapers: 10,408 tokens
  - Standard--Official-Issues: 10,093 tokens
  - Standard--Web: 10,097 tokens

#### Arabic Language Models 
  - CRF Model: (crf_model.sav)
  - LSTM (RNN) Model: (RNN-model.h5, RNN_tag2index.pkl, RNN_word2index)
  - Skip-Gram Model: (SkipGram_model.pt)
  - CBOW Model: (cbow_model.h5, CBOW_Embeddings.npz)
  - araBERTv02: (token_vecs_cat_array.pkl, token_vecs_cat_array.npz, tokenized_text.pkl)
  - Fine-tuned model: (fine_tuned_arabertv02.zip)
