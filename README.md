# Tutorial for measuring psychological variables in text using a Gold-standard accuracy approach

This repository contains three tutorial Python notebooks concerning **how to measure psychological variables in text** using a "gold-standard" accuracy approach. A gold-standard accuracy approach (common in the Natural Language Processing literature but not Psychology) involves the use of a manually coded dataset to develop and validate classifiers using accuracy statistics. All three notebooks are based on a case study for measuring misunderstandings in online dialogues (at a sentence level). 

## Tutorial notebooks description

1. [Tutorial 1](Tutorial_1_Inter_rater_reliability.ipynb): Conducting inter-rater reliability on a subset of a gold-standard dataset, hand-coded by multiple coders for a psychological construct.  
2. [Tutorial 2](Tutorial_2_Rule_based_dictionary_classifier.ipynb): Developing and validating a rule-based dictionary classifier using the gold-standard dataset. This tutorial relies heavily on the [spaCy](https://spacy.io/) Python package (Honnibal et al., 2020), specifically it's [rule-based matcher](https://spacy.io/usage/rule-based-matching). 
3. [Tutorial 3](Tutorial_3_Deep_learning_BERT_classifier.ipynb): Developing and validating a deep-learning classifier using the gold-standard dataset (fine-tuning a [BERT](https://aclanthology.org/N19-1423/) (Devlin et al., 2019) model through transfer learning). This tutorial relies heavily on the [ktrain](https://github.com/amaiya/ktrain) Python package (Maiya, 2020). 

## Data description

The [data](data/) folder contains the datasets for the tutorial notebooks and the [dictionaries](data/dictionaries/) for the rule-based classifier. The notebook tutorials automatically link to these folders and it is therefore not necessary to download the data.

# Demonstration of trained Misunderstanding BERT classifier:

Also included is a [demonstration notebook](Demonstration_BERT_Misunderstanding_Predictor.ipynb) allowing the user to experiment with our trained classifier (`F1-score = 0.81`). It allows the user to type in a sentence and observe the classifier's prediction. For the demonstration to work, the notebook should be run in Google Colab.

# References:

Devlin, J., Chang, M.-W., Lee, K., & Toutanova, K. (2019). BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding. *Proceedings of the 2019 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers)*, 4171-4186. https://doi.org/10.18653/v1/N19-1423

Honnibal, M., Montani, I., Van Landeghem, S., & Boyd, A. (2022). *spaCy: Industrial-strength natural language processing in Python*. Explosion.

Maiya, A.S. (2022). ktrain: A Low-Code Library for Augmented Machine Learning. (arXiv:2004.10703). arXiv. https://doi.org/10.48550/arXiv.2004.10703
