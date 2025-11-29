# Tomato-Leaf-Disease-Classification-DenseNet121-EfficientNetB0-SMOTE-
Hybrid tomato leaf disease classifier using DenseNet121 and EfficientNetB0 for deep feature extraction, SMOTE for class balancing, and an ensemble of SVM, Random Forest, and XGBoost for robust prediction. Achieves high accuracy and AUC for reliable, real-world disease detection.
This repository contains a hybrid deep learning framework for robust tomato leaf disease detection, integrating DenseNet121, EfficientNetB0, and SMOTE-optimised ensemble machine learning classifiers. The project addresses the challenge of early, accurate plant disease identification by combining deep feature extraction with balanced, high-performance classification techniques.

Project Overview

Tomato plants are highly susceptible to fungal, bacterial, and viral infections. Traditional manual inspection is slow, expensive, and error-prone. This research proposes a hybrid deep feature–ensemble learning system to achieve reliable, scalable, and automated disease classification using images from the PlantVillage dataset.

The model integrates:
DenseNet121 for dense feature reuse and enhanced gradient flow
EfficientNetB0 for efficient compound-scaled spatial representation
Concatenated deep features forming a unified descriptor
SMOTE to address class imbalance by synthetically oversampling minority disease categories
Multi-classifier ensemble (Random Forest, SVM, XGBoost) with soft voting for final prediction
This combination significantly improves feature diversity, robustness, and generalizability compared to single CNN or standalone ML classifiers.

 Key Features

Hybrid CNN feature extraction with DenseNet121 + EfficientNetB0
Image preprocessing (CLAHE, Bilateral Filtering, Normalization)
Extensive data augmentation for model generalization
SMOTE-based oversampling of minority classes
Multi-classifier ensemble using Random Forest, SVM, and XGBoost
High classification accuracy with improved AUC and F1-scores
Well-structured pipeline for training, evaluation, and reproducibility

Dataset

The model uses the PlantVillage Tomato Leaf Dataset, consisting of healthy and multiple disease classes such as:
Early Blight
Septoria Leaf Spot
Bacterial Spot
Tomato Mosaic Virus
Healthy
All images were resized to 224×224, converted to RGB, and normalized using ImageNet statistics.

Methodology
Preprocessing
CLAHE contrast enhancement
Bilateral filtering
Image resizing + normalization
Augmentation (rotation, flipping, scaling)
Deep Feature Extraction
Remove classifier heads
Extract 1024 (EfficientNetB0) + 1024 (DenseNet121) feature vectors
Concatenate into a unified deep descriptor
Data Balancing with SMOTE
Oversamples minority disease classes
Prevents classifier bias
Improves recall and AUC
Ensemble Classification
Random Forest
Support Vector Machine (RBF)
XGBoost
Soft voting for final prediction

Evaluation Metrics
Accuracy
Precision, Recall, F1-score
Confusion Matrix
ROC Curves + AUC
Classification Report

Results

The hybrid feature–ensemble model achieved:
High accuracy across all disease classes
Improved recall of minority diseases due to SMOTE
Stronger generalization than single CNN and single ML models
AUC > 0.95 on most classifiers
The integration of deep hybrid features and ensemble machine learning provides a reliable pipeline for real-world tomato disease identification.
