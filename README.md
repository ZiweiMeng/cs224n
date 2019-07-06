# cs224n
Natural Language Processing

* Week 1 - Word Vectors
  - a1/exploring_word_vectors.ipynb
  - a1/Gensim word vector visualization.ipynb

* Week 2 - Skipgram model, SGD
  - a2/a2_solution.pdf (theoretic part)
  - a2/word2vec.py
  - a2/sgd.py
  - a2/run.py
  
* Week 3 - Adam, Dropout, Neural Transition-Based Dependency Parsing
  - a3/a3_solution.pdf (theoretic part)
  - a3/demo.png (an example of parsing)
  - a3/parser_transitions.py
  - a3/parser_model.py
  - a3/run.py
  
* Week 4 - Neural Machine Translation with LSTM and attention
  - a4/nmt_model.py
  - a4/model_embeddings.py
  - a4/utils.py
  - Why enc_masks?
    * enc_masks sets all padded word to -inf, since -inf*(any real number)=-inf, after applying softmax function padded word (which means in original sentence there is no word present at position) will be assigned 0.0 score, tell model not to pay attention to padded word.
