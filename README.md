## Garbage Classification with VGG16
# Overview
This project aims to create an efficient garbage classification system using the VGG16 convolutional neural network (CNN) architecture. By classifying waste items into predefined categories (such as glass, cardboard, metal, paper, plastic, and trash), we contribute to environmental sustainability and promote recycling efforts.

# Key Steps
1. Data Collection and Preprocessing
Gathered a diverse dataset of garbage images, including various waste types.
Performed data augmentation, resizing, and normalization to prepare the data for training.
VGG16 mean values were used for normalization: [123.68, 116.779, 103.939].
2. Model Architecture
Utilized the pre-trained VGG16 model, known for its effectiveness in image classification tasks.
Replaced the classifier (fully connected layers) with a new one that fits the number of waste types (6 in this case).
3. Training and Evaluation
Trained the model on the normalized dataset, optimizing for accuracy and minimizing loss.
Evaluated the model’s performance using precision, recall, and F1-score metrics.
Achieved a final test accuracy of approximately 77.27%.
Tested the model with a real image of a plastic item and it was correctly identified as being plastic.
5. Confusion Matrix and Precision-Recall Curve
Visualized the confusion matrix to understand how well the model predicted each waste type.
Calculated precision, recall, and F1-score for each class.
Plotted the precision-recall curve for individual waste types.

# Usage
Data Preparation:
Organize your garbage images into separate folders for each waste type (e.g., glass, cardboard, etc.).
Ensure that the images are in JPG or PNG format.
Training:
Run the provided code to normalize images, split data, and train the VGG16 model.
Fine-tune hyperparameters as needed.
Evaluation:
Evaluate the model on the test data to obtain accuracy, precision, recall, and F1-score.
Visualization:
Use the confusion matrix heatmap to analyze classification performance.
Refer to the precision-recall curve for insights into model behavior.

# Dependencies
Python 3.x
PyTorch
TensorFlow (for data preprocessing)
Matplotlib
Seaborn

# Acknowledgments
The VGG16 model was pre-trained on ImageNet and adapted for garbage classification.
Thanks to the open-source community for providing garbage image datasets.
