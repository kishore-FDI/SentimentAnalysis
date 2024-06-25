Project Title: Audio Classification with LSTM and MFCC Features

Table of Contents
About
Data
Installation
Usage
Model
Results
Contributing
License
About
This project aims to classify audio files using LSTM (Long Short-Term Memory) networks with MFCC (Mel-Frequency Cepstral Coefficients) features. The goal is to leverage LSTM's ability to handle sequential data for effective audio classification.

Data
The dataset consists of 7442 audio files from the CREMA-D dataset. Each audio file is preprocessed to extract MFCC features, which are then used as input to the LSTM model. The dataset is split into training, validation, and test sets to evaluate the model's performance.

Installation
Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/audio-classification-lstm.git
Navigate to the project directory:
bash
Copy code
cd audio-classification-lstm
Install the required dependencies:
Copy code
pip install -r requirements.txt
Usage
Preprocess the data:
python
Copy code
python preprocess.py
Train the model:
python
Copy code
python train.py
Evaluate the model:
python
Copy code
python evaluate.py
Model
The model architecture consists of:

Two LSTM layers with 128 and 64 units respectively.
Batch normalization layers for stable training.
A Dense layer with 64 units and ReLU activation.
A Dropout layer with a rate of 0.3 to prevent overfitting.
An output Dense layer with 6 units and softmax activation for classification.
Results
The model achieved an accuracy of approximately 18% on the test set after training for 50 epochs. Further tuning and improvements are ongoing to enhance performance.

Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes. Ensure that your code adheres to the project's coding standards and includes appropriate tests.

License
This project is licensed under the MIT License. See the LICENSE file for details.
