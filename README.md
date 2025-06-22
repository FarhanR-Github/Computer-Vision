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

**Set up your environment:** 

It is recommended to run this notebook in Google Colab for easy access to GPUs and pre-installed libraries.
If running locally, ensure you have Python 3.7 or higher installed.

Install the required libraries using pip. You can generate a requirements.txt file from the notebook by running !pip freeze > requirements.txt and then install them using pip install -r requirements.txt.

**Obtain the dataset:** 

The dataset is expected to be located in your Google Drive, specifically at /content/drive/MyDrive/Colab Notebooks/EDA/CV/CV_Portfolio_Project/fruite-360 (15 classes).

If you are running this notebook locally, you will need to download the dataset and update the dataset_path variable in the notebook to point to the correct location of your dataset.

Image dataset is provided in this repository

**Run the notebook:**

If using Google Colab, mount your Google Drive by running the cell containing from google.colab import drive and drive.mount("/content/drive").

Execute the code cells sequentially from top to bottom. The notebook is structured to perform data loading, preprocessing, model training, and evaluation in order.
