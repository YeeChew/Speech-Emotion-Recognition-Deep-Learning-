# Deep Learning(Speech Emotion Recognition)
Speech Emotion Recognition Using CNN and CNN+LSTM

This project focuses on speech emotion recognition (SER) by implementing convolutional neural networks (CNN) and a hybrid model that combines CNN with long short-term memory (CNN+LSTM). The Toronto Emotional Speech Set (TESS) dataset is utilized for training and evaluation.

# Toronto Emotional Speech Set (TESS) dataset
[TESS](https://www.kaggle.com/datasets/ejlok1/toronto-emotional-speech-set-tess)

# Data Preprocessing
Three different data preprocessing techniques are applied to the audio data:
Pre-emphasis: Enhances high-frequency components to improve feature extraction.
Hamming Window: Reduces spectral leakage by applying a window function to the audio signal.
Short-Time Fourier Transform (STFT): Converts the audio signal from the time domain to the frequency domain, providing a time-frequency representation

# Feature Extraction
The Mel Frequency Cepstral Coefficients (MFCC) are used for feature extraction. MFCC captures the essential features of the speech signal, representing the phonetic content and emotional tone.

# Model Implementation
CNN: A Convolutional Neural Network is trained to classify emotions based on the extracted MFCC features.
CNN+LSTM: This hybrid model combines the strengths of both CNN and LSTM. The CNN layers learn features from both spatial and time dimensions, while the LSTM network processes the sequence data by looping over time steps and capturing long-term dependencies. Together, the CNN-LSTM network effectively learns from the training data by utilizing convolutional layers to extract features and LSTM layers to understand temporal relationships.
