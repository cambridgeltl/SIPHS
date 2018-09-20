# MS-LSTM code and resources

Code and resources for the EMNLP 2018 paper "Mapping Text to Knowledge Graph Entities using Multi-Sense LSTMs" [1] can be found at the following repository:

[https://bitbucket.org/dimkart/ms-lstm](https://bitbucket.org/dimkart/ms-lstm)

The model maps efficiently unrestricted text to knowledge graph entities using the following process:

1. The KB graph is extended with textual features weighted by their importance with respect to the entity nodes.
2. A synthetic "corpus" of biased random walks is created and used as input to the skipgram model. This generates an enhanced KB space to be used as target for the text-to-entity mapping process
3. The transformation from text to entities/concepts is achieved via a supervised multi-sense compositional model, which generated a point in the KB space for every input text. The model is an LSTM equipped with an attentional mechanism that dynamically disambiguates the embeddings of the input words given the surrounding context.

[1] D. Kartsaklis, M.T. Pilehvar, N. Collier (2018). **Mapping Text to Knowledge Graph Entities using Multi-Sense LSTMs**, in _Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing (EMNLP)_, Brussels, Belgium [\[pdf\]](https://arxiv.org/pdf/1808.07724.pdf)
