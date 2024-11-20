# South Asian Identification Tensorflow
South Asia boasts a rich and diverse musical heritage with a wide array of instruments, each characterized by unique tonal qualities, shapes, and
playing techniques. Instrument classification focuses on identifying the probability of a mixture of instruments being played in a piece of music. In this project, we are hoping to perform this task on a number of South Asian instruments, and provide the baseline for further work, such as development of software providing the real-time classification of instruments playing during a performance.

## CNN Model Results
The CNN model has been implemented using Keras API provided by Tensorflow framework. It has a 3x3 convolutional layer followed by three 2x2 convolutional layers all with 2x2 max pooling. The number of filters were 32, 64, 128, and 256 with ReLu activation. The model uses sigmoid as the decision activation function in order to assign probabilities to the 15 categories. The total trainable parameters are 8,565,807.

The training of the model was performed on Google Colab using a T4 GPU. After shuffling and splitting our 6000 samples into 80% train and 20% test our model was
trained for 10 epochs with a batch size of 32 and a learning rate of 0.001 with binary cross entropy as the loss measure. We arrived at a learning rate of 0.001 as greater learning rates had lesser accuracies and smaller learning rates would have taken greater time.

## Report
You can find the detailed project report containing our reseach question, literature review, results and findings and conlusion [report](https://github.com/saadabdulhakimqureshi/South-Asian-Identification-Tensorflow/blob/main/Report.pdf).

## References
The reference code for the CNN model used in this project can be found in the Kaggle notebook [kaggle](https://www.kaggle.com/code/siddhantojha17/musical-instruments-classification-cnn/notebook).
