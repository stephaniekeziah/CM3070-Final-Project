Breast Cancer Detection using Deep Learning (VGG16 + Explainable AI)

Project Overview

This project focuses on detecting breast cancer from mammogram images using a deep learning model based on transfer learning. A pre-trained VGG16 Convolutional Neural Network (CNN) was used and fine-tuned to classify mammogram images into cancerous and non-cancerous classes.

In addition to building a classification model, this project also includes Explainable AI (XAI) techniques such as Grad-CAM and LIME to help visualise how the model makes predictions. This makes the system more interpretable and suitable for medical image analysis.

Objectives

The main objectives of this project are:

- To build a deep learning model that can classify mammogram images.
- To apply transfer learning using a pre-trained CNN (VGG16).
- To improve model interpretability using Grad-CAM and LIME.
- To evaluate the model using accuracy, F1-score, and AUC.
- To demonstrate how deep learning can assist in early breast cancer detection.

Dataset

The dataset used in this project is the Breast Cancer Detection Dataset (BCDD) obtained from Mendeley Data.

The dataset consists of mammography images stored in separate folders for training and testing. Each image is associated with an annotation file that contains the class label (cancerous or non-cancerous).

Technologies Used:
Python
TensorFlow / Keras
NumPy
OpenCV
Matplotlib
Scikit-learn
LIME (Local Interpretable Model-Agnostic Explanations)
Jupyter Notebook
 
Model Architecture

The model is based on transfer learning using VGG16:

Pre-trained VGG16 convolutional base (ImageNet weights)
GlobalAveragePooling2D
Dense layer (ReLU activation)
Dropout layer
Output layer (Sigmoid activation for binary classification)

Model Evaluation

The model was evaluated using multiple performance metrics:

Accuracy
F1-score
AUC (Area Under the Curve)
ROC Curve
Training and Validation Loss

These metrics were used instead of relying only on accuracy because the dataset contains class imbalance.

Explainable AI (XAI)

To improve interpretability, two explainability techniques were implemented:

Grad-CAM

Highlights the important regions in the mammogram that influenced the model’s prediction.

LIME

Identifies the most important image regions using superpixel segmentation and local explanations.

These techniques help us understand whether the model is focusing on relevant areas in the mammogram images.
