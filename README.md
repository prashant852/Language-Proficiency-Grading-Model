# Language-Proficiency-Grading-Model
Automated language proficiency grading model using deep learning 

## **Dataset description**
Dataset contains english essays written by language learners (8th-12th grade)
>Original dataset can be found [here](https://www.kaggle.com/competitions/feedback-prize-english-language-learning/data/)

Whole dataset is divided into modeling data (labeled) and unseen data (unlabeled)

Modeling data is further divided into train-test in a 80:20 ratio which contains columns:
>**text_id**: Unique essay ID\
>**full_text (input)**: Raw text of essay\
>**cohesion (output)**: Analytic measure\
>**syntax** (output): Analytic measure\
>**vocabulary (output)**: Analytic measure\
>**phraseology (output)**: Analytic measure\
>**grammar (output)**: Analytic measure\
>**conventions (output)**: Analytic measure

## **Approaches**
Preprocessing of text is done using below approaches followed by keras functional api architecture
> **Bert Base Uncased** (Transformer model pretrained on a large corpus of English data in a self-supervised fashion) Modeling_Code_BERT_BASE_UNCASED.ipynb\
> **Deberta v3** (Improvement on the BERT and RoBERTa models using disentangled attention and enhanced mask decoder) 


Modeling code are in separate files for both approaches\
>**Bert Base Uncased**: Modeling_Code_BERT_BASE_UNCASED.ipynb\
>**Deberta v3**: fp3-ell-deberta.ipynb
