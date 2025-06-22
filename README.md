# ﻿Fruit Image Classification Project
**1. Project Overview**

This project focuses on building and comparing different image classification models for a fruit dataset. We explore transfer learning with popular CNN architectures (ResNet50, VGG16, EfficientNetB0) and also evaluate a YOLOv8n-cls model adapted for classification. The goal is to determine which model performs best on this specific task.

**2. Dataset Source**

The dataset used in this project is available in GitHub repository expected to be organized in a directory structure where each subdirectory represents a different fruit class. 

**3. Tools/Libraries Used**

The project utilizes several Python libraries for data handling, image processing, model building, and evaluation:

pandas
numpy
matplotlib
seaborn
tensorflow
opencv-python
split-folders
scikit-learn
ultralytics
Pillow

**4. Key Findings or Visualizations**

**Model Performance:** 

ResNet50: Validation Loss: ~0.609, Validation Accuracy: ~0.825. Achieved ~0.83 accuracy on confusion matrix/classification report. Training Time: ~1 hour.

VGG16: Validation Loss: ~0.002, Validation Accuracy: ~0.999. Achieved ~0.06 accuracy on confusion matrix/classification report. Training Time: ~1.5 hours.

EfficientNetB0: Validation Loss: ~2.684, Validation Accuracy: ~0.089. Achieved ~0.06 accuracy on confusion matrix/classification report. Training Time: ~19.61 minutes.

YOLOv8n-cls: Training Loss: ~0.003, Validation Top-1 Accuracy: 1.0, Validation Top-5 Accuracy: 1.0. Achieved ~0.06 accuracy on confusion matrix/classification report. Training Time: ~2.8 hours.

**Best Performing Model:** 

Based solely on the evaluation metrics from the validation dataset, the YOLOv8n-cls model appears to be the best performing with a perfect Top-1 and Top-5 accuracy on the validation set after training, although the classification report and confusion matrix metrics for all models seem inconsistent with the validation accuracy metrics, which might indicate an issue during the generation of the classification reports and confusion matrices.

**Visualizations:** 

(Describe the insights gained from the training curves and confusion matrices)

**5. How to Run the Code**

(This section should provide instructions on how to set up the environment and run the notebook. You might need to adapt these steps based on where the notebook and data are stored.)

**Set up your environment:** 

You should use Google Colab  ![Copilot_20250622_190245](https://github.com/user-attachments/assets/0322d9f0-cb8d-4975-a648-fd1791652687)
as all the above listed necessary libraries are pre-installed.

**Obtain the dataset:** 

Image dataset is provided in this repository

**Run the notebook:**

Execute the code cells sequentially in the provided Jupyter Notebook or Google Colab notebook.
