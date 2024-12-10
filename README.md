# Hate Speech Detection with BERT: Addressing Class Imbalance

This repository contains the implementation and resources for our project on hate speech detection using the (tdavidson/hate_speech_offensive) dataset and BERT. The project addresses the challenges of class imbalance in hate speech detection by leveraging data augmentation, majority class downsampling, and class weighting techniques.

## Project Overview

Hate speech detection plays a crucial role in moderating online content and mitigating abusive language. This project tackles the severe class imbalance in the (tdavidson/hate_speech_offensive) dataset, where 76% of the data is offensive language, 19% is neutral, and only 5% constitutes hate speech.

## Key Contributions
1. **Data Augmentation: Using ContextualWordEmbsAug() from the nlpaug library, we augmented the minority classes (neutral and hate speech).
2. **Class Downsampling: The majority class (offensive language) was downsampled to reduce its dominance.
3. **Class Weighting: Adjusted the loss function to reweight the contributions of each class during training.
4. **Model Fine-Tuning: Fine-tuned the BERT model to classify hate speech, offensive language, and neutral comments.

## Results

The final BERT model achieved a significantly improved performance compared to the initial proposal metrics, particularly in detecting hate speech and neutral language. Below are the final recall values:

### Final Recall:
1. **Hate Speech: 0.61
2. **Offensive Seech: 0.90
3. **Neutral: 0.89

### Initial Proposal Recall:
1. **Hate Speech: 0.24
2. **Offensive Speech:0.96
3. **Neutral: 0.90

