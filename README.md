# Online Harassment Detection Capstone Project
Using NLP to identify online harassment

## Overview and Understanding
Online harassment is a pervasive issue that affects a significant portion of the population, with serious consequences for individuals and society. According to a 2021 Pew research poll, a majority of respondents believe that social media companies are not doing enough to address online harassment. Harassment affects various demographics, with women and LGBTQ+ individuals being particularly vulnerable.

Social media platforms play a crucial role in disseminating information and shaping public sentiment. The misuse of these platforms can lead to severe consequences. Detecting and addressing hate speech and toxic comments are essential tasks in the information age.

The goal of this capstone project is to build a virtual moderator (vMOD) using Natural Language Processing (NLP) techniques. The vMOD will accurately predict whether a comment is harassment or not. This model will not only help in reducing the impact of toxic commentary but also alleviate the psychological burden on human moderators.

## Data Understanding

Our dataset is derived from the Kaggle competition titled [Identifying Toxic Comments: Jigsaw Toxic Comment Classification Challenge](https://www.kaggle.com/competitions/jigsaw-toxic-comment-classification-challenge/data). It contains 159,571 comments from Wikipedia, with six target variables: toxic, severe_toxic, obscene, threat, insult, and identity_hate.

To work with this dataset, we've downloaded and accessed the files from our cloud drive, as it's too large to upload directly to Git.

## Data Preprocessing

We began by cleaning and preprocessing the data. We removed stopwords and applied various regex expressions to clean the comments, removing non-ASCII characters, websites, and non-words. We also considered the length of comments to prepare for tokenization.

## Model and Evaluation

We explored different models, including a Multinomial Naive Bayes model, to classify toxic comments. We initially faced class imbalance issues but improved the model's performance by transforming it into a binary classification task. This reduced false positives significantly.

We also experimented with word embeddings and neural networks to improve model performance but encountered challenges in reducing false negatives.

## Conclusion

Our capstone project aims to address the critical issue of online harassment through NLP models. While we've made progress in classifying toxic comments, there's room for improvement, especially in reducing false negatives. Our initial results suggest that oversampling the minority class may be necessary.

## Next Steps

1. Address Class Imbalance: Implement a different sampling strategy, such as SMOTE, to improve model performance, particularly in reducing false negatives.

2. BERT Model: Complete the BERT (Bidirectional Encoder Representations from Transformers) model and assess its precision in detecting toxic comments.

3. Further Model Enhancements: Continue exploring advanced NLP models and techniques to improve the accuracy and reliability of the virtual moderator.

4. Deployment: Consider how to deploy the virtual moderator to actively moderate online platforms and contribute to safer online spaces.
