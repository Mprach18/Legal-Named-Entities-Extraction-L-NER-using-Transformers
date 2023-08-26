# Legal Named Entities Extraction (L-NER) using Transformers

The Indian legal system typically provides information
about legal cases in the form of unstructured
documentation. Today, though this data is kept in
a digital format, the legal industry faces special
difficulties when it comes to extraction of key
information out of the documents. The structure
of legal documents and the use of domain-specific
language are to blame for this. Finding pertinent
information in unstructured textual content is
never an easy task, despite the fact that it is filled
with information. The language terms used in
Indian courts make it challenging for the most
advanced NLP model to extract any pertinent
information, which is why this is the case. These
terms include "Tehsil-dar" (Collector), "Daroga"
(Constable), and others. Depending on the specific
situation and the intended use, understanding these
terms can be essential. The extraction of such
case-specific information from the current NLP
task development has not progressed as much.
For our experiment, we are performing this task
of named entity recognition on dataset of Indian
legal documents Kalamkar et al. (2022) which are
written in the English language.
We propose a transformer-based solution that
can extract global and local feature-level information
using a self-attention mechanism. The initial
approach relied on a BERT-base-cased transformer
for obtaining encoded features of the tokenized
input sequence and further used LSTM-based
sequence classification for producing entity-wise
tag sequence. There were certain limitations
with this approach which restricted its overall
performance and therefore, we then discovered an
alternative approach. This approach used a similar
idea as the earlier approach, where a pre-trained
BERT-base-cased transformer is used in our
proposed architecture to encode token-level input
sequence and decode it into a tag-labeled sequence.
While performing various experiments on the
LegalNER dataset, we discovered several intricacies
that are needed to be analyzed and processed
for extracting the relevant entity-level information.
The design decisions for our approaches
were derived by considering how IOBE
tagging can be utilized for span-level entity categorization.
