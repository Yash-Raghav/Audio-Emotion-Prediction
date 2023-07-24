# Audio-Emotion-Prediction

Human emotions help communicate the inner feelings of every being and most often it’s easily done through speech, through semantics and voice attributes, such as pitch, loudness, etc. Human beings have innate ability to recognize these emotions expressed in speech, but this task is not easy for machines, yet! This project aims to build a simple neural network solution to try and predict some basic human emotions given audio speech data.

Datasets used:
- [RAVDESS](https://smartlaboratory.org/ravdess/)
- [CREMA-D](https://github.com/CheyneyComputerScience/CREMA-D)
- [SAVEE](http://kahlan.eps.surrey.ac.uk/savee/)
- [TESS](https://tspace.library.utoronto.ca/handle/1807/24487)

Proposed models:

- 1D Convolutional Neural Network based model - A simple Deep Neural Network was designed for the classification task is reported operationally in the below fig. It is a simple One-Dimensional Convolutional Neural Network, containing 2 hidden layers.

![image](https://github.com/Yash-Raghav/Audio-Emotion-Prediction/assets/82383225/973798c1-ee4c-4a32-9052-3c1caac46e6c)


- 2D LSTM - Among the variants of the RNN function, we LSTM based Neural Network. It is a simple network with 3 hidden layers as shown in the figure below:

![image](https://github.com/Yash-Raghav/Audio-Emotion-Prediction/assets/82383225/910a0e72-239a-477a-ad85-59f287a59899)


- 2D Mel-Spectrum based– Transfer Learning Model - Here we tested with pre-trained image recognition CNN models from the keras applications including VGG-16, VGG-19, Xception and Inception V3. Each of these models uses multiple 2D CNNs, pooling and Batch Normalization operations the layers. The final layers after freezing the pre-trained layers are as below:

![image](https://github.com/Yash-Raghav/audioEmotionPrediction/assets/82383225/16c5774e-9415-46ee-87a7-7295c484459b)

Evaluation:
The best results were achieved with the 2D mel-spectrum based models with training accuracy of 73% with a loss of 0.71 and validation accuracy of 0.68 with a loss of 0.95.
On test set accuracy achieved was 68% with a loss of 0.89.

![image](https://github.com/Yash-Raghav/audioEmotionPrediction/assets/82383225/97d7733e-a916-4649-a227-96072d919ca7)
![image](https://github.com/Yash-Raghav/audioEmotionPrediction/assets/82383225/7c635c19-e709-45ba-bcd4-e60be78c6f63)


Individual class and label evaluation:

![image](https://github.com/Yash-Raghav/audioEmotionPrediction/assets/82383225/03accdb8-e3a5-4cbe-aa25-b8084d244795)


A detailed report with the audio features and mathematical functions can be read [here](https://github.com/Yash-Raghav/audioEmotionPrediction/blob/main/Report.pdf).
