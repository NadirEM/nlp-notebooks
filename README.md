# NLP Notebooks

[Fine-tune ALBERT for sentence-pair classification](https://github.com/NadirEM/nlp-notebooks/blob/master/Fine_tune_ALBERT_sentence_pair_classification.ipynb) | How to fine-tune an **ALBERT** model or another BERT-based model for the **sentence-pair classification** task | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NadirEM/nlp-notebooks/blob/master/Fine_tune_ALBERT_sentence_pair_classification.ipynb)

This **PyTorch** implementation leverages the Hugging Face *transformers* and *datasets* libraries

The dataset used in this notebook is Microsoft Research Paraphrase Corpus (**MRPC**) which is part of the GLUE benchmark : you have two sentences and you want to predict if one sentence is the paraphrase of the other one. The evaluation metrics are **F1** and **accuracy**.

You should be able to reach on the validation set **91.19** as F1 score (the score reported in the ALBERT paper is 90.9) and **87.5** as accuracy. The fine-tuning takes 35 seconds per epoch and the inference takes 2 seconds.

The **main feature**s of this tutorial are :

[1] End-to-end ML implementation (training, validation, prediction, evaluation)

[2] Easy adaptability to your own datasets

[3] Facilitation of quick experiments with other BERT-based models (BERT, ALBERT, ...)

[4] Quick training with limited computational resources (mixed-precision, gradient accumulation, ...)

[5] Multi-GPU execution

[6] Threshold choice for the classification decision (not necessarily 0.5)

[7] Freeze BERT layers and only update the classification layer weights or update all the weights

[8] Reproducible results with seed settings
