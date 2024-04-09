# PRODIGY_ML_03
Image Classification using CNN:

Data Preparation: The script reads training and testing images from specified directories.

Data Augmentation: ImageDataGenerator is used for data augmentation. It rescales pixel values to [0,1] and applies transformations such as shear, zoom, and horizontal flip to augment the training dataset.

CNN Model Architecture: A Sequential model is constructed for the CNN:

Convolutional layers (Conv2D) with ReLU activation extract image features.
MaxPooling layers reduce spatial dimensions of feature maps.
Flatten layer converts 2D feature maps to a 1D vector.
Dense layers with ReLU activation introduce non-linearity.
Final Dense layer uses sigmoid activation for binary classification.
Model Compilation: The model is compiled with:

Adam optimizer
Binary crossentropy loss function (for binary classification)
Accuracy as the evaluation metric
Model Training: The model is trained on the training dataset using the fit function for a specified number of epochs (e.g., 10). Validation dataset (test_generator) is used for monitoring model performance during training.

Model Evaluation: After training, the model is evaluated on the test dataset using the evaluate method, and the test accuracy is printed.

Feel free to customize and adjust the provided content to match the specifics of your project. This summary outlines the essential steps and components of an image classification project leveraging Convolutional Neural Networks.
