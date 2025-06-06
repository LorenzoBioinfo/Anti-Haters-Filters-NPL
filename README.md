🛡️ Anti-Hater Filter for Social Networks

Final project for the course "Deep Learning and Artificial Neural Networks"
Master’s Program in Data Science

📌 Overview

This project aims to develop a system that automatically classifies user comments based on their level of harmful language using deep learning techniques.
The goal is to build a tool that can be integrated into social media platforms to detect toxic, offensive, or hateful content, promoting safer digital spaces.

🧠 Model Architecture

The core of the system is a deep neural network with recurrent layers (RNNs), designed for a multi-label classification task.
The model is trained to recognize the following labels:

toxic
severe_toxic
obscene
threat
insult
identity_hate

🛠️ Project Workflow

Text Preprocessing
Data cleaning
Removal of tokens that carry no significant semantic value
Text to Sequence Transformation
Tokenization and conversion of the corpus into numerical sequences
Model Construction
Deep Learning model with recurrent layers (e.g., LSTM or GRU)
Configured for multi-label output
Prediction and Output Interpretation
Output: a 6-element binary vector (one per class)
Example:
Safe comment → [0, 0, 0, 0, 0, 0]
Harmful comment → [1, 0, 0, 0, 1, 0]
📊 Dataset

The dataset used includes six binary labels per comment, indicating the presence or absence of various forms of harmful content.




📈 Evaluation Metrics

During training, the model is evaluated using multi-label classification metrics such as:

Precision
Recall
F1-score (macro and micro)
