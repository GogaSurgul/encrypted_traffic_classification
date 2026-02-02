Network Traffic Classification using Machine Learning

This project implements a machine learning pipeline for classifying network traffic data using a neural network. The goal is to compare a baseline model with an improved model that includes regularization techniques such as Dropout and EarlyStopping.

Dataset
The dataset used in this project is `Darknet.csv`, which contains network flow features such as:
- Source IP
- Destination IP
- Ports
- Protocol
- Flow duration
- Packet statistics
- Label (traffic class)

Data Preprocessing
The preprocessing steps include:
- Removing unnecessary columns (Flow ID, Timestamp, Label2)
- Handling missing values
- Converting IP addresses to integers
- Encoding class labels using LabelEncoder
- Scaling features using StandardScaler


Models
Baseline Model
A neural network with:
- Input layer
- Three hidden layers (ReLU activation)
- Output layer with Softmax activation

Improved Model
Enhancements include:
- Dropout layers to reduce overfitting
- EarlyStopping callback
- Same architecture with regularization

Results

| Model | Accuracy |
|-------|----------|
| Baseline Model | 99.28% |
| Improved Model | 99.24% |

Accuracy Improvement: **-0.03%**

Although the improved model applied regularization techniques, the baseline model performed slightly better, indicating that the original architecture was already well suited for this dataset.









Darknet Traffic Activity Classification

This project builds a machine learning model to classify user activity types 
(Label2) from darknet network traffic data.

Activities include:
- Browsing
- Chat
- Email
- File Transfer
- P2P
- VOIP
- Audio Streaming
- Video Streaming

Methods
- Data preprocessing (IP conversion, NaN removal, scaling)
- Label encoding
- Neural network classifier (TensorFlow/Keras)
- Evaluation with accuracy and confusion matrix

Result
Final accuracy: ~85%

Dataset
Darknet.csv
