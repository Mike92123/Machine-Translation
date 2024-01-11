# Machine Translation Using Custom and Pre-trained Transformers
## Introduction
Author: Zheng Zheng
Email: zheng.zheng2@northeastern.edu
Submission Date: 11/27/2023

This report presents an in-depth analysis of machine translation, focusing on comparing a custom transformer implementation with a pre-trained transformer RNN model. The primary task is French to English translation, evaluated based on accuracy, efficiency, and BLEU scores.

## Objective
To design and assess the performance of custom and pre-trained transformer models in translating French to English, and to identify the most effective approach in terms of quality and computational efficiency.

## Dataset Acquisition
Data Source: French to English sentences.
Data Loading: Utilizing pd.read_csv for importing data.
Data Conversion: Transforming data into TensorFlow datasets.
### Examples:
English: "You're demented."
French: "Vous êtes fous."
## Custom Transformer Implementation
Development: Creating a transformer tailored to the dataset.
Components: Positional encoding, add and normalization, feed-forward network, encoder, decoder, and training.
### Sample Translation:
Input: "Parlez-vous anglais?"
Prediction: "Are you speaking English?"
## Pre-trained Transformer Usage (RNN Model)
Text Preprocessing: Including standardization and vectorization.
Encoder/Decoder: Implementing a bidirectional RNN encoder and attention mechanism.
Inference and Training: Efficient execution and training process.
### Sample Translation:
Input: "Qu’avez-vous mangé?"
Prediction: "What did you eat?"
## Comparative Analysis
Methodology: Assessing translation quality, BLEU scores, and computational efficiency.
## Results:
Translation Quality: Custom model shows higher fidelity but also inaccuracies; pre-trained model has a mix of accurate and inaccurate translations.
BLEU Scores: Custom model achieved a higher average score of 0.3713 compared to 0.3638 for the pre-trained model.
Efficiency: Custom model required more time (5 hours for training), while the pre-trained model demonstrated higher efficiency (7 minutes for training).
## Discussion
Custom Transformer: Offers accuracy but with higher resource and time intensity.
Pre-trained Transformer RNN: Suitable for quick response times and computational efficiency despite slightly lower accuracy.
## Conclusion
The choice between custom and pre-trained transformer models depends on the specific requirements of the task. For accuracy and resource availability, the custom model is preferable, while the pre-trained model is more apt for speed and computational efficiency.

## Appendix
### Evaluation Data:
Input sentences in French with ground truth translations in English.
Comparative output translations by both models.
BLEU score evaluations and visual data representations.
