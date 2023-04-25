## Talafeef: Arabic POS Tagging and Lemmatizer

#### Almujaiwel, S., Omar, B., Alshehri, M. (2022). Talafeef: A POS Tagging and Lemmatization System for Diverse Genres of Modern Standard Arabic Texts [GitHub repository]. [https://github.com/salmujaiwel/talafeef--arabic--lemmatizer](https://github.com/salmujaiwel/talafeef--arabic--lemmatizer)

#### This early-stage system was built entirely from scratch, starting with the collection of Arabic corpora, followed by the construction of automatic POS tagging and lemmatization tools.
#### The corpora for the five domains identified in this project can be expanded, as our goal was to develop tools and methods for tokenization, segmentation, POS tagging, and lemmatization stages.
#### Word-embedding models were created using the project's data to experimentally observe how these models function.

##### Information about the corpora
  - Standard--Academic: 10,512 tokens
  - Standard-- Khutbah: 10,380 tokens
  - Standard--Newspapers: 10,408 tokens
  - Standard--Official-Issues: 10,093 tokens
  - Standard--Web: 10,097 tokens

#### POS Tagset (inspired by STANFORD)
| Tag    | Description                          |
|--------|--------------------------------------|
| N      | Nouns (Non-tagged specific features) |
| VBD    | Past tense                           |
| VBN    | Passive voice                        |
| VBP    | Present tense                        |
| VB     | Imperative                           |
| JJ     | Derived adjectives                   |
| JJR    | Comparative adjectives               |
| RB     | Adverbs                              |
| DT     | Demonstrative pronouns               |
| WP     | Relative pronouns                    |
| IN     | Prepositions                         |
| CC     | Conjunctions                         |
| PRP    | Personal pronouns                    |
| RP     | Particles                            |
| WRB    | Interrogative pronouns               |
| ABBREV | Arabic abbreviations                 |
| PUNC   | Punctuation marks                    |
| CD     | Numbers                              |
| FW     | Non-Arabic                           |

#### The project involves training, testing, and evaluating the following: models such as Conditional Random Fields (CRF), Long Short-Term Memory LSTM (RNN), Skip-Gram, Continuous Bag of Words (CBOW), and araBERTv02. The models and files saved in the project:
#### Trained, tested, evaluated models using classification metrics.
  - CRF Model: (crf_model.sav)
  - LSTM (RNN) Model: (RNN-model.h5, RNN_tag2index.pkl, RNN_word2index)
#### Word embeddings using Skip-Gram, CBOW, and araBERTv02:
  - Skip-Gram Model: (SkipGram_model.pt)
  - CBOW Model: (cbow_model.h5, CBOW_Embeddings.npz)
  - araBERTv02 (source: https://huggingface.co/aubmindlab/bert-base-arabertv2): (token_vecs_cat_array.pkl, token_vecs_cat_array.npz, tokenized_text.pkl)
#### Fine-tuned pre-trained araBERTv02 Model on the project-specific data
  - fine_tuned_arabertv02.zip
