# Human Activity Recognition using a Convolution & LSTM neural network

This project focuses on predicting user activities based on their device interactions, which has various applications in everyday life. The aim is to correctly predict activities such as standing/sitting, regular walking, running, and jogging, using data collected from smartphone sensors.

To address this challenge, we used deep learning model that combines convolutional neural networks (CNNs) and long short-term memory (LSTM) networks with self-attention. 

Key Features:

* Data collection from smartphone sensors for a wide range of activities with `1.2 Million+ entries with 13 different activities and their labels`.
* Evaluation of the model using the MHEALTH dataset, yielding an overall accuracy of `95%` in under 10 epochs.
* Integration of CNNs, LSTMs, and self-attention for accurate human activity recognition.
* Possible intergation of the model into mobile devices to constantly predict and list the activity of the user.

## Code Structure

The main code file includes the implementation of the deep learning model. It consists of the following sections:

1. `Data Preprocessing`: The code assumes that the input data is in the form of time series sequences with corresponding labels. The data is preprocessed to create balanced datasets, remove outliers, and split into training and testing sets. 
2. `Model Architecture`: The model architecture is defined using various layers, including Conv1D, LSTM, attention, and Dense layers. These layers are stacked together to capture temporal dependencies in the input sequences.
3. `Model Compilation`: The model is compiled with the Adam optimizer and sparse categorical cross-entropy loss function. The sparse_categorical_accuracy metric is used to monitor the model's performance during training.
4. `Model Training and Evaluation`: The model is trained on the training dataset and evaluated on the testing dataset.

   
![model](https://github.com/kssmp/Human_Activity_Recognition_LSTM/assets/115448106/a15a98ad-70de-4540-91fb-dad917bfcbac)

## Results

The model's performance can be evaluated based on various metrics such as precision, recall & f1 score. 

![Screenshot 2023-07-18 at 7 51 57 PM](https://github.com/kssmp/Human_Activity_Recognition_LSTM/assets/115448106/22f533ca-93c8-4cb6-8f06-743f137b9d72)


## Team Members

* Saket Koppineedi (BT20ECE114)
* Unmay Kharabe (BT20ECE088)
* Sahil Khode (BT20ECE051)
  
## References & Links

[MHealth Dataset](http://archive.ics.uci.edu/dataset/319/mhealth+dataset)

[HAR using tensorflow version 1x by Guillaume Chevalier](https://github.com/guillaume-chevalier/LSTM-Human-Activity-Recognition)
