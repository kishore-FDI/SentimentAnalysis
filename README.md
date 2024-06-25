### GitHub README

**Project Title: Audio Classification with LSTM and MFCC Features**

#### About
This project focuses on classifying audio files using LSTM (Long Short-Term Memory) networks in conjunction with MFCC (Mel-Frequency Cepstral Coefficients) features. Audio classification is a critical task in various applications, including speech recognition, music genre classification, and emotion detection. Leveraging LSTM networks allows for handling the sequential nature of audio data effectively.

#### Data
The dataset used in this project is the CREMA-D (Crowd-sourced Emotional Multimodal Actors Dataset), which comprises 7442 audio files. Each file contains a spoken utterance with different emotional expressions. This dataset provides a rich source of varied audio signals, making it suitable for training and testing audio classification models.

#### Features
To extract meaningful features from the audio files, MFCCs are used. MFCCs capture the short-term power spectrum of a sound and are widely used in speech and audio processing. In this project, the MFCC features are extracted from each audio file, providing a robust representation for the LSTM model.

#### Model
The model architecture consists of the following key components:
- **LSTM Layers**: Two LSTM layers with 128 and 64 units respectively, designed to capture the temporal dependencies in the audio data.
- **Dense Layers**: A Dense layer with 64 units and ReLU activation to learn complex representations.
- **Dropout Layer**: A Dropout layer with a rate of 0.3 to prevent overfitting during training.
- **Output Layer**: A Dense layer with 6 units and softmax activation for classification into six categories.

#### Training and Evaluation
The model is trained using the processed MFCC features. The dataset is split into training, validation, and test sets to evaluate the model's performance. During training, techniques such as batch normalization and learning rate scheduling are employed to improve the model's convergence and stability. Early stopping and reducing the learning rate on plateau help in preventing overfitting and ensuring efficient training.

#### Results
After training for 50 epochs, the model achieved an initial accuracy of approximately 18% on the test set. While this indicates room for improvement, it provides a solid foundation for further tuning and optimization of the model. Future work includes experimenting with different model architectures, hyperparameters, and feature extraction techniques to enhance classification accuracy.

This project demonstrates the potential of combining LSTM networks with MFCC features for effective audio classification. The approach can be extended to various audio classification tasks, paving the way for more sophisticated and accurate models in the field of audio processing.
