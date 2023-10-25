# Online Harassment Detection Capstone Project
Using NLP to identify online harassment

## Important Links
* Link to data: [Jigsaw Toxic Comment Classification Challange](https://www.kaggle.com/competitions/jigsaw-toxic-comment-classification-challenge/data)
* [Slideshow](https://docs.google.com/presentation/d/1sIyA66zn8tSioSQeL-PfIgbk4osqfjKKVfznTv9qQ1E/edit?usp=sharing)
* [Collab Notebook](https://colab.research.google.com/drive/173EBJAcL5LSN_q5-QKomYLWSfO6IPKEr?usp=sharing)
* [BERT Collab Notebook](https://colab.research.google.com/drive/1cpWFaNgGR0gjVR4oKRShtcNb1ps4hBTI?usp=sharing)

## Overview and Understanding
Online harassment is a pervasive issue that affects a significant portion of the population, with serious consequences for individuals and society. According to a 2021 Pew research poll, a majority of respondents believe that social media companies are not doing enough to address online harassment. Harassment affects everyone, but has a more significant impact on BIPOC and LGBTQIA communities, as well as women.

Social media platforms play a crucial role in disseminating information and shaping public sentiment. Therefore, use of social media sites through creation of a hostile environment by an extreme few can not, and should not be condoned. Detecting and addressing hate speech and toxic comments are essential tasks in the information age.

Our client, a small social media site that specializes in neighborhood forums, is looking to combat an uptick in trolling on their site.  The goal of this capstone project is to build a virtual moderator (vMOD) using Natural Language Processing (NLP) techniques. The vMOD will accurately predict whether a comment is harassment or not. This model will not only help in reducing the impact of toxic commentary but also alleviate the financial onus of needing to employ a large group of human moderators, in addition to lessening the emotional toll of the remaining human moderators.

## Data Understanding

Our dataset is derived from the Kaggle competition titled [Identifying Toxic Comments: Jigsaw Toxic Comment Classification Challenge](https://www.kaggle.com/competitions/jigsaw-toxic-comment-classification-challenge/data). It contains 159,571 comments from Wikipedia, with six target variables: toxic, severe_toxic, obscene, threat, insult, and identity_hate.


## Data Preprocessing

We began by cleaning and preprocessing the data. We removed stopwords and applied various regex expressions to clean the comments, removing non-ASCII characters, websites, and non-words. We also considered the length of comments to prepare for tokenization.

## Model and Evaluation

We explored different models, including a Multinomial Naive Bayes model, to classify toxic comments. We initially faced class imbalance issues but improved the model's performance by transforming it into a binary classification task. This reduced false positives significantly.

We also experimented with word embeddings and neural networks to improve model performance but encountered challenges in reducing false negatives.
<img width="583" alt="Screenshot 2023-10-24 at 3 01 41 PM" src="https://github.com/slowings/NLP_identifying_trolls/assets/113614318/2c8db969-7f99-4ede-a4f0-1160a6f7b78f">

## Conclusion

Our capstone project aims to address the critical issue of online harassment through NLP models. While we've made progress in classifying toxic comments, there's room for improvement, especially in reducing false negatives. Our initial results suggest that oversampling the minority class may be necessary.  That being said, we can utilize our binary MNB classifier to begin the work of filtering comments. 

## Next Steps

1. Address Class Imbalance: Implement a sampling strategy with our neural network to undersample our majority class

2. BERT Model: Complete the BERT (Bidirectional Encoder Representations from Transformers) model and assess its precision in detecting toxic comments.

3. Further Model Enhancements: Continue exploring advanced NLP models and techniques to improve the accuracy and reliability of the virtual moderator.

4. Deployment: Consider how to deploy the virtual moderator to actively moderate online platforms and contribute to safer online spaces.
