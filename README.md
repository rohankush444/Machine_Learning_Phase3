# Machine_Learning_Phase3

1. Project Title
   
Explainable-Plant-Disease-Detection

3. Background and Motivation
   
Agriculture plays a vital role in food production worldwide. Plant diseases can significantly reduce crop yield and quality, leading to economic losses for farmers. Traditional disease identification relies on expert knowledge and manual inspection, which can be time-consuming and inaccurate.

Recent advances in Deep Learning and Computer Vision, particularly Convolutional Neural Networks (CNNs), have shown excellent performance in image classification tasks. CNN-based disease detection systems can automatically identify plant diseases from leaf images with high accuracy. However, most deep learning models operate as "black boxes," making their decisions difficult to understand.

This project aims to develop an explainable plant disease detection system that not only classifies plant diseases but also provides visual explanations using Grad-CAM, improving trust and interpretability.

3. Problem Statement
   
Manual identification of plant diseases is labor-intensive, expensive, and dependent on expert availability. There is a need for an automated and explainable system capable of accurately detecting plant diseases from leaf images while providing visual evidence for its predictions.

5. Selected Dataset and Dataset Link
   
Dataset: PlantVillage Dataset

Dataset Link: https://www.kaggle.com/datasets/emmarex/plantdisease

5. Dataset Description
   
Number of Images
Approximately 54,000+ images

Number of Classes
38 classes

Image Type
RGB color images of healthy and diseased plant leaves

Class Distribution
The dataset contains multiple crop species and disease categories. Most classes are relatively balanced, although slight variations exist in image counts.

Example classes include:

Tomato Early Blight
Tomato Late Blight
Potato Healthy
Potato Early Blight
Apple Scab
Apple Healthy
Corn Common Rust
Pepper Bacterial Spot
6. Research Questions
How accurately can CNN models classify plant diseases from leaf images?
Does transfer learning improve classification performance compared to a custom CNN?
Can Grad-CAM effectively explain the model's predictions?
Which model provides the best trade-off between accuracy and computational complexity?
7. Expected Results
Classification accuracy above 90%.
Transfer learning models expected to outperform the custom CNN.
Grad-CAM visualizations highlighting infected leaf regions.
Reliable classification report and confusion matrix.
Explainable predictions for improved transparency.
8. Proposed Methodology
Step 1: Data Collection
Obtain the PlantVillage dataset.

Step 2: Data Preprocessing
Image resizing (224 × 224)
Pixel normalization
Label encoding
Dataset splitting
Step 3: Data Augmentation
Rotation
Horizontal flip
Zoom
Width shift
Height shift
Step 4: Model Development
Model A: Custom CNN

Model B: Transfer Learning (MobileNetV2)

Step 5: Training
Cross-entropy loss
Adam optimizer
Early stopping
Model checkpointing
Step 6: Evaluation
Accuracy
Precision
Recall
F1-score
Confusion Matrix
Step 7: Explainability
Apply Grad-CAM to visualize disease regions influencing predictions.

9. CNN Model Design
Input Layer
224 × 224 × 3

Convolution Block 1
Conv2D (32 filters)
ReLU
MaxPooling
Convolution Block 2
Conv2D (64 filters)
ReLU
MaxPooling
Convolution Block 3
Conv2D (128 filters)
ReLU
MaxPooling
Fully Connected Layers
Flatten
Dense(256)
Dropout(0.5)
Output Layer (Softmax)
10. Transfer Learning Models
MobileNetV2
Advantages:

Lightweight architecture
Fast training
High accuracy
Optional additional model:

EfficientNetB0
Used for performance comparison.

11. Evaluation Metrics
The following metrics will be used:

Accuracy
Precision
Recall
F1-score
Confusion Matrix
ROC Curve (optional)
AUC Score (optional)
12. Expected Figures and Tables
Figures
Figure 1: Sample Dataset Images

Figure 2: Data Augmentation Examples

Figure 3: Training Accuracy Curve

Figure 4: Validation Accuracy Curve

Figure 5: Training Loss Curve



Tables

Table 1: Dataset Summary

Table 2: CNN Architecture

Table 3: Hyperparameters

Table 4: Model Performance Comparison

Table 5: Classification Report Summary

Expected Contribution
The project will demonstrate how explainable AI techniques can improve trust in plant disease detection systems while maintaining high classification accuracy through CNNs and transfer learning.
