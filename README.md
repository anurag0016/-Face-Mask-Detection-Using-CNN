# -Face-Mask-Detection-Using-CNN
 The Face Mask Detection project leverages deep learning and computer vision techniques to automatically identify whether a person is wearing a face mask. 
The global COVID-19 pandemic underscored the importance of preventive measures like wearing face masks in public spaces. Manual enforcement of mask usage is labor-intensive, prompting the need for automated solutions. This project aims to develop an AI-powered face mask detection system using Convolutional Neural Networks (CNNs), a specialized deep learning architecture well-suited for image classification tasks.

The primary objective of the project was to build a robust model capable of accurately classifying whether a person is wearing a face mask or not, based on image inputs. The dataset, structured into two categories — with_mask and without_mask — was used to train and evaluate the model. Data preprocessing steps included normalization, resizing images to 100x100 pixels, and applying data augmentation techniques like zooming, shearing, and horizontal flipping to improve generalization and reduce overfitting.

A CNN was implemented using TensorFlow and Keras libraries. The architecture consists of multiple convolutional layers with ReLU activation functions, followed by max-pooling layers to reduce spatial dimensions. The flattened output is passed through a fully connected dense layer with dropout regularization before being fed into the final sigmoid-activated output layer, which determines the binary classification.

The model was trained for 10 epochs using binary cross-entropy as the loss function and the Adam optimizer. The training and validation accuracy were tracked across epochs, with the model achieving over 90% accuracy, demonstrating its effectiveness in distinguishing masked from unmasked faces. The trained model was then saved as a .h5 file, making it suitable for deployment in real-time applications.

An additional functionality was implemented to test predictions on individual images using the model, enabling easy integration with future enhancements such as real-time video feed monitoring using OpenCV.

In conclusion, this face mask detection model is a reliable and scalable solution that can be integrated into surveillance systems to automate health safety monitoring. The project showcases proficiency in deep learning, computer vision, and model deployment workflows, providing a foundation for building more advanced human safety compliance tools.
