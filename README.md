Talafeef: A Trial System for Arabic POS Tagging and Lemmatization
Almujaiwel, S., Omar, B., Alshehri, M. (2022). talafeef--arabic--lemmatizer [GitHub repository]. https://github.com/salmujaiwel/talafeef--arabic--lemmatizer
The Arabic Lemmatizer system includes:
A lemmatization methodology for Arabic words
Extraction of definitions and synonyms for Arabic words
Development of a Long Short-Term Memory (LSTM) recurrent neural network (RNN) model instead of a Conditional Random Field (CRF) model for POS tagging
Development of Continuous Bag of Words (CBOW) and Skip-Gram models for predicting contextually similar words
Contextual word prediction using the pre-trained BERT model; Source: https://huggingface.co/aubmindlab/bert-base-arabertv2
Models in order, written in English for clarity (all these models are placed in a folder named: Arabic Lemmatizer Models)
CRF Model: (crf_model.sav)
LSTM (RNN) Model: (rnn-model.h5)
N-Gram Model: (tag2index.pkl and word2index.pkl)
Skip-Gram Model: (model.pt)
CBOW Model: (model.h5 and embeddings.npz)
araBERTv2: (tokenized_text.npz) and (token_vecs_cat_array.npz) and (tokenized_text.pkl).
All are integrated into the GUI. We first created the bert-model.h5, then we created a list of embeddings to use at this stage.
To execute the GUI, download the zip file named NLPiffy_GUI, and run the file saved as nlpiffy_gui.py.
The concept of the Talafeef system for the Arabic Lemmatizer
This system was built entirely, starting from the collection of Arabic corpora, to the construction of a complete automatic lemmatizer. The texts of the five domains identified in this project can be expanded, as we aimed to develop manual tools and methods at the stages of segmentation, tokenization, POS tagging, and lemmatization.

Information about the corpora
Standard--Academic: 10,512 tokens.
Standard-- Khutbah: 10,380 tokens.
Standard--Newspapers: 10,408 tokens.
Standard--Official-Issues: 10,093 tokens.
Standard--Web: 10,097 tokens.

Why these specific domains? The Arabic language is rich in diversity of domains, with few fields and topics. We limited these domains to only five, due to their inclusiveness. It is known that scientific fields and topics, such as medicine, are scarce in Arabic, but this scarcity can be addressed by reducing the number of domains in favor of balancing those few fields. This strategy is proposed by the team leader and will help increase our corpus in the future, and in this increase, a balance may be achieved. How? If we brought many domains, the increase in what is abundantly available in them may weaken the lexicographical materials in the corpus, such as newspapers, where the same words, moderately repetitive, abound, regardless of their geographies and subjects. This assumption led us to determine the most important domains that include the language as a representative language in which levels of eloquence and clarity are represented, and these domains are: academic, religious, journalistic, official publications, and web.
