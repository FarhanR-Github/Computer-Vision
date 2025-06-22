# ﻿Fruit Image Classification Project
**1. Project Overview**

This project focuses on building and comparing different image classification models for a fruit dataset. We explore transfer learning with popular CNN architectures (ResNet50, VGG16, EfficientNetB0) and also evaluate a YOLOv8n-cls model adapted for classification. The goal is to determine which model performs best on this specific task.

**2. Dataset Source**

The dataset used in this project is expected to be organized in a directory structure where each subdirectory represents a different fruit class. (You might want to add a more specific link or description of where the dataset can be obtained if it's publicly available).

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

(This section should be filled in after you have completed the model training and evaluation. You can summarize the performance of each model, highlight the best-performing one, and describe key visualizations like accuracy/loss curves or confusion matrices.)

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

(Mention any specific requirements, e.g., using Google Colab, installing libraries from a requirements.txt file).

**Obtain the dataset:** 

(Provide instructions or a link to download the dataset and place it in the correct directory structure).

**Run the notebook:**

Execute the code cells sequentially in the provided Jupyter Notebook or Google Colab notebook.
