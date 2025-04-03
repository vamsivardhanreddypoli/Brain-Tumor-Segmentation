# Brain-Tumor-Segmentation
An open-source AI framework for automated brain segmentation, abnormality detection, and statistical analysis in neuroimaging using deep learning models like U-Net with Attention Mechanisms and MONAI. Features real-time inference and testing.

# 1. Introduction

Objective: Develop an automated AI-based framework for brain tumor segmentation using deep learning.

Significance: Early and accurate detection of brain tumors is crucial for diagnosis and treatment planning.

Approach: Utilized deep learning models (U-Net with Attention Mechanisms) and MONAI for neuroimaging analysis.

# 2. Dataset Overview

Dataset Name: BraTS 2020 (Brain Tumor Segmentation Challenge)

Data Format: NIfTI (.nii) medical imaging files.

Types of MRI Modalities:

FLAIR (Fluid Attenuated Inversion Recovery)

T1-weighted MRI

T1ce (T1-weighted with contrast enhancement)

T2-weighted MRI

Segmentation Mask (Ground truth labels)

Classes in Segmentation Mask:

0: No tumor

1: Necrotic/core tumor

2: Edema

3: Enhancing tumor

# 3. Data Preprocessing

Loading Data: Used nibabel to load NIfTI files.

Normalization: Scaled pixel intensity values for uniformity.

Augmentation: Applied transformations (rotation, flipping, scaling) to improve model generalization.

Resizing: Standardized image size for model input.

# 4. Data Visualization

MRI Slices Visualization: Plotted different slices of MRI images.

Segmentation Mask Overlay: Displayed tumor masks overlayed on the images.

3D Rendering: Generated 3D volume representations of the brain scan.

# 5. Model Development

Model Architecture: Modified U-Net with Attention Gates for segmentation.

Loss Function: Categorical Cross-Entropy.

Evaluation Metrics:

Dice Coefficient

Precision

Sensitivity (Recall)

Specificity

Training Strategy: Used MONAI's data pipeline for efficient training.

# 6. Training and Validation

Splitting Data: Train (70%), Validation (20%), Test (10%).

Training Pipeline:

Used MONAI for dataset loading and augmentation.

Trained using TensorFlow/Keras.

Used callbacks (EarlyStopping, ReduceLROnPlateau, ModelCheckpoint).

# 7. Performance Evaluation

Metrics Computation: Dice Score, Precision, Recall, Specificity, Train Accuracy, Validation Loss.

# 8. Model Inference and Deployment

Inference Pipeline: Tested the trained model on new MRI scans.



