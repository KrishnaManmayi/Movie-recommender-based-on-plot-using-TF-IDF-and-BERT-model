# Movie-recommender-based-on-plot-using-TF-IDF-and-BERT-model

First approach: Term Frequency-Inverse Document Frequency (TF-IDF)
Term Frequency (TF):-
The number of times a word appears in a document divided by the total number of words in the document. Every document has its own term frequency.
Inverse Data Frequency (IDF):-
The log of the number of documents divided by the number of documents that contain the word.
Inverse data frequency determines the weight of rare words across all documents in the corpus.

Second approach: Using a pre-trained BERT(Bidirectional Encoder Representations from Transformers) model to understand the context of movie plot in a bi-directional manner.
BERT is a stack of transformer or encoder layers. It understands the context of a sentence efficiently by observing the sentence from the left as well as from right i.e., bidirectionally.
It is a pre trained language model, which performs the following two tasks:-
1. Masked Language Modelling (MLM) : This task helps BERT achieve bidirectionality. In every sentence that is given as input, 15% of the words are randomly masked, which are understood as missing tokens. 
The model predicts the masked words and learns from the feedback of its prediction.
2. Next Sequence Prediction (NSP): In this task, pairs of sentences are considered. 50% of the data are correctly paired, whereas, the rest of the data are paired wrongly i.e., The sentence following the first sentence does not follow it in the original data.
The model then learns the right pairs from the feedback.

Cosine Similarity:
The movie plots are transformed as vectors in a geometric space. Therefore angle between two vectors represents the closeness of those two vectors. 
Cosine similarity calculates similarity by measuring the cosine of angle between two vectors.
