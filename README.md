# Image Captioning Model Project NLP @ the AI Guild 

## Project 1: MNIST Convolutional Neural Network
We created separate branches to test out our own hyperparameters and find the most accurate model. The branch [Ian-de-leon-b1](https://github.com/ghubnerr/nlp-image-captioning/tree/Ian-de-leon-b1) was the one with the highest precision for the MNIST dataset.
![image](https://github.com/ghubnerr/nlp-image-captioning/assets/91924667/2e6025c2-2b31-4ec9-9bda-a577d75ddf8d)

### Hyperparameters
- Batch size: 64
- Epochs: 7
- Optimizer: rmsprop
- Loss function: Categorical Cross-entropy

### Layer Structure
- Conv2D(64, (3,3), activation="relu")
- MaxPooling2D((2,2))
- Conv2D(64, (3,3), activation="relu")
- MaxPooling2D((2,2))
- Flatten()
- Dense(128, activation="relu")
- Dense(10, activation="softmax")
