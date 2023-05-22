# RSNA Spotlight 2023

## AI Implementation: Building Expertise and Influence.

## Acknowledgements

The medical images for this session (chest x-rays) were obtained from: Wang X, Peng Y, Lu L, Lu Z, Bagheri M, Summers RM. ChestX-ray8: Hospital-scale Chest X-ray Database and Benchmarks on Weakly-Supervised Classification and Localization of Common Thorax Diseases. IEEE CVPR 2017 and available [here](https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publicly-available-chest-x-ray-datasets-scientific-community).

## 1. Basics of Image Classification
In the field of radiology, one of the most commmon tasks is to examine chest X-rays and categorize them based on observed features, such as the cardiomediastinal contour, lung opacity, and bone condition to determine if a patient may have a specific disease. This task at its core is image classification.

## 2. How Convolutional Neural Networks (CNNs) work
To aid in this classification task, we introduce a Convolutional Neural Network (CNN), a type of neural network that is specially good in recognizing patterns and objects in images, much like a team of specialized radiology trainees.

### 2.1. Layers of the CNN
Convolutional Layers
Each trainee specializes in identifying certain features in the X-ray. One might be proficient at noticing abnormalities in the cardiomediastinal contour, another at discerning variations in lung textures, and another at spotting bone structure irregularities. Their observations are like looking at the X-ray through 'special glasses'.

Pooling Layers
A second type of trainee then takes these detailed observations and simplifies them. If the first trainee notes several areas of abnormal cardiomediastinal contour, the second trainee could summarize this as "abnormal cardiomediastinal contour detected".

Fully Connected Layers
Finally, a senior trainee considers these summarized notes and forms a preliminary diagnosis, such as "Potential cardiovascular abnormality or mediastinal mass present".

## 3. Training the Network (Backpropagation and Gradient Descent)
The trainees are shown a vast number of chest X-rays already diagnosed by expert radiologists - this 'labeled data' forms their training material.

### 3.1. Backpropagation
When the CNN trainees make an incorrect preliminary diagnosis, the expert radiologist points out their errors. This learning from mistakes and adjusting their approach is called backpropagation.

### 3.2. Gradient Descent
Improving their performance requires a strategic approach. The CNN trainees need to understand how to fine-tune their analytical lenses to get better at identifying the correct features. This strategy is known as gradient descent.

Imagine gradient descent as climbing to the peak of a foggy mountain. The trainees, like blindfolded climbers, feel the slope with their feet to discern the uphill path, indicating where improvements can be made. They adjust their approach and repeat the process, continuously improving their performance.

The size of the steps they take, or the learning rate, determines the pace of their learning. If the steps are too large, they risk missing the peak; if they are too small, the climb to peak performance might take too long.

In the beginning, the starting position of the trainees on this mountain is chosen randomly. Due to these different starting points, each training run might identify different optimal paths and peaks. This randomness results in diverse solutions that the CNN can use to diagnose X-rays accurately.

However, once a peak has been identified, and the 'GPS coordinates' (the final weights of the network) have been recorded, we can expect consistent performance from the trainee. As long as we keep the network configuration the same (returning to the same GPS coordinates), we can expect the same high level of performance each time we use it.

Through this process of learning, adjusting, and refining, the CNN trainees (the network) become an increasingly valuable tool, enhancing the capabilities of radiologists in their vital work.
