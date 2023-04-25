### Talafeef: Early-stage POS Tagging and Lemmatization System

###### Almujaiwel, S., Omar, B., Alshehri, M. (2022). talafeef--arabic--lemmatizer [GitHub repository]. https://github.com/salmujaiwel/talafeef--arabic--lemmatizer

###### This early-stage system was built entirely, starting from the collection of Arabic corpora, to the construction of a complete automatic lemmatizer. The corpus of the five domains identified in this project can be expanded, as we aimed to develop manual tools and methods at the stages of tokenization, segmentation, POS tagging, and lemmatization.

###### The project involves training, testing, and evaluating the following: models such as Conditional Random Fields (CRF), Long Short-Term Memory (LSTM)-(RNN), Skip-Gram, Continuous Bag of Words (CBOW), and araBERT. The models and files saved in the project are:
  - CRF Model: (crf_model.sav)
  - LSTM (RNN) Model: (rnn-model.h5)
  - N-Gram Model: (tag2index.pkl and word2index.pkl)
  - Skip-Gram Model: (model.pt)
  - CBOW Model: (model.h5 and embeddings.npz)
  - araBERTv2 (source: https://huggingface.co/aubmindlab/bert-base-arabertv2): (tokenized_text.npz) and (token_vecs_cat_array.npz) and (tokenized_text.pkl)

###### All are integrated into the NLPiffy_GUI.zip . 
  ###### To execute the GUI, download the zip file named NLPiffy_GUI, and run the file saved as nlpiffy_gui.py.

###### Information about the corpora
Standard--Academic: 10,512 tokens
Standard-- Khutbah: 10,380 tokens
Standard--Newspapers: 10,408 tokens
Standard--Official-Issues: 10,093 tokens
Standard--Web: 10,097 tokens

###### POS Tagset: 
N: Nouns | V: Verbs (VBD: Past tense, VBN: Passive voice, VBP: Present tense, VB: Imperative) | JJ: Derived adjectives | JJR: Comparative adjectives | RB: Adverbs | DT: Demonstrative pronouns | WP: Relative pronouns | IN: Prepositions | CC: Conjunctions | PRP: Personal pronouns | RP: Particles | WRB: Interrogative pronouns | ABBREV: Arabic abbreviations | PUNC: Punctuation marks | CD: Numbers | FW: Lemmas' POS tags

###### Lemmas' POS tags
Noun: N, WP, DT | Adjective: JJ, JJR | Verb: VBD, VBN, VBP, VB | Particle: IN, RP, WRB, CC | Adverb: RB | Number: CD | ABBREV | PUNC | CD | FW
