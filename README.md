# Overview
In this project, we leverage the power of Deep Neural Networks (DNNs) to classify music genres effectively.

# Preprocessing
Audio files can be extremely large, sometimes containing millions of data points. To address this, we transform the audio data into the frequency domain using Discrete Fourier Transform (DFT). The result of this preprocessing is a 2D image representation where the x-axis represents various frequency values, and the y-axis indicates the amplitude of each frequency.

# Model Prototyping
Our model is inspired by the ResNet-50 architecture, known for its efficacy in handling complex image data. We have tailored the architecture to suit our needs by replacing the final classification layer with a fully connected layer that categorizes the input into one of ten music genres. We employ CrossEntropyLoss as our loss function to guide the model in accurately identifying the music genre.

# Training Process
The dataset is divided into a 70-30 training-evaluation split. This means 70% of the data is used for training the model, while the remaining 30% is reserved for evaluation purposes.

# Evaluation and Results
We assess the model's performance by evaluating the classification accuracy for each genre individually. The results are as follows:
```
Accuracy for class: blues is 71.4 %
Accuracy for class: classical is 95.5 %
Accuracy for class: country is 66.7 %
Accuracy for class: disco is 64.5 %
Accuracy for class: hiphop is 85.3 %
Accuracy for class: jazz  is 84.4 %
Accuracy for class: metal is 83.3 %
Accuracy for class: pop   is 80.8 %
Accuracy for class: reggae is 77.4 %
Accuracy for class: rock  is 30.6 %
```
