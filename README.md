# Chest-X-Ray-Classification-using-CNN-and-Transfer-Learning-with-EfficientNetB0
This project aims to build a deep learning-based system for the automatic classification of chest X-ray images into two categories: Normal and Pneumonia.  
I used the Chest X-Ray Images (Pneumonia) dataset, which contains thousands of labeled chest X-ray images. For experimentation and to reduce training time, I selected a limited subset of the dataset—2000 images for training, and 500 each for validation and testing. All images were resized to 256x256 pixels and normalized for optimal model performance. 

The project is implemented in two phases:

1. Custom Convolutional Neural Network (CNN)
I developed a simple CNN architecture from scratch using TensorFlow/Keras. It includes multiple convolutional and max-pooling layers, followed by fully connected dense layers and a sigmoid output for binary classification. This model learns features like edges, patterns, and textures directly from the X-ray images.

2. Transfer Learning using EfficientNetB0
To enhance performance, I employed transfer learning with EfficientNetB0, a state-of-the-art deep learning model pre-trained on ImageNet. The model was used as a feature extractor, and a custom classification head was added. By freezing the base layers and training only the new layers, the model achieves faster convergence and improved accuracy even with limited data.

The models were evaluated using standard metrics such as accuracy, precision, recall, and F1 score. The results show that the transfer learning approach outperforms the custom CNN in terms of both speed and accuracy.
