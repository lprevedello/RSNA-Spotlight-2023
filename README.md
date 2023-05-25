# RSNA Spotlight 2023

## AI Implementation: Building Expertise and Influence.

## Acknowledgements

The medical images for this session (chest x-rays) were obtained from: Wang X, Peng Y, Lu L, Lu Z, Bagheri M, Summers RM. ChestX-ray8: Hospital-scale Chest X-ray Database and Benchmarks on Weakly-Supervised Classification and Localization of Common Thorax Diseases. IEEE CVPR 2017 and available [here](https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publicly-available-chest-x-ray-datasets-scientific-community).

## 1. Basics of Image Classification
In the field of radiology, one of the most commmon tasks is the interpretation of chest X-rays. This task, at its core, is image classification.

## 2. How Convolutional Neural Networks (CNNs) work
To aid in this classification task with the use of computers, we will introduce a Convolutional Neural Network (CNN), a type of neural network that is specially good in recognizing patterns and objects in images, much like a team of specialized radiology trainees.

### 2.1. Layers of the CNN
#### Convolutional Layers:
Imagine that each of these specialized radiology trainees focuses in identifying certain features in the X-ray. One might be proficient at noticing abnormalities in the cardiomediastinal contour, another at discerning variations in lung textures, and another at spotting abnormalities in the bone. Their observations are like looking at the X-ray through 'special lenses' or in the case of a CNN: filters.

#### Pooling Layers:
Now imagine that each of the previous trainees are providing information to a second more senior trainee that takes the detailed observations and summarizes them. If the first trainee notes several areas of abnormal lung texture with opacification of the inferolateral portion of one lung, the second trainee could summarize this as "lung opacity" and "blunting of the costophrenic angle". The process of summarization of the observations is by pooling layers in CNNs.

#### Fully Connected Layers:
Finally, a senior trainee considers these summarized notes and forms a preliminary diagnosis, such as "pneumonia" and "plaural effusion". The fully connected layers of a CNN are mapped to expected outcomes or pre-defined labels.

## 3. Training the Network (Backpropagation and Gradient Descent)
The trainees are shown a vast number of chest X-rays already diagnosed by expert radiologists - this 'labeled data' forms their training material.

Same as when an expert radiologist points out the errors of a trainee, when a CNN makes an incorrect preliminary diagnosis, there are mechanism (i.e. backpropagation and gradient descent) that help the network adjust its approach to maximize correct responses. This process is performed iteratively and since there are so many different starting points and potential solutions, each training run might identify different optimal paths. This randomness results in diverse solutions that the CNN can use to diagnose X-rays accurately. However, once a solution is identified (the final weights of the network), we can expect consistent performance. As long as we keep the network configuration the same, we can expect the same high level of performance each time we use it.
