# Legal Named Entities Extraction (L-NER) using Transformers

Our approach presents a transformer-based model for named entity recognition in Indian legal documents. The main contribution is a model that accurately detects different named entities for Preamble and Judgment sets of Legal NER corpus. We experimented with 2 different approaches to solve the problem. Our best approach involves using a Bert transformer-based encoder and decoder model in the SimpleTransformer library. Our initial approach uses a transformer-based encoder and an LSTM-based model as a decoder for sequence classification for named entity recognition. We have also compared our results with a fine-tuned baseline transformer model and achieve good F1 scores of 80.29 for judgment and 71.57 for the preamble.

