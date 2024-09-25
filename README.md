# Cat and Dog Image Classification using CNN

## Overview
This project focuses on classifying images of cats and dogs using a Convolutional Neural Network (CNN) model. The dataset was imported from Kaggle and consists of labeled images of cats and dogs. The model was developed using Keras with TensorFlow backend. Techniques like Batch Normalization and Dropout were used to reduce overfitting and improve model generalization.

## Dataset
The dataset consists of thousands of images of cats and dogs, split into training, validation, and test sets. Each image is resized to 256x256 pixels and normalized before feeding into the model.

**Dataset Source:** [Kaggle: Cats vs Dogs](https://www.kaggle.com/c/dogs-vs-cats/data)

## Model Architecture
The CNN model consists of three convolutional layers, each followed by a Batch Normalization and MaxPooling layer. After flattening, two dense layers are added, followed by a Dropout to prevent overfitting. The final layer uses a sigmoid activation function for binary classification (cat or dog).
          
### Key Techniques
- **Batch Normalization:** Applied after every convolutional layer to normalize the inputs and improve model convergence.
- **MaxPooling:** Used to reduce the dimensionality of feature maps and extract dominant features.
- **Dropout:** Prevents overfitting by randomly dropping units during training.
- **Sigmoid Activation:** Used in the output layer for binary classification (1 for dog, 0 for cat).

## Conclusion
The CNN model built for cat and dog image classification successfully distinguishes between the two categories. With proper preprocessing, augmentation, and regularization techniques, the model generalizes well on new data.
