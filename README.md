# Multiclassification-on-Neurological-Diseases
## 📌 Project Overview
This objective of the project aims to classify an input handwriting image into Alzheimer patient, Parkinson patient or healthy individuals. We approach this by performing full data science pipeline that:

- Preprocess image data(normalization, transformation, merge datasets from different sources)
- Train multiple classification models (CCNet-12, CBAM, MobileNetV2, ResNet) with 3-fold cross validation
- Evaluate model performances using metrics like Accuracy, F1-Score, and Confusion Matrices.
-  Summarize insightful information in a set of slides and an 8-page write up.

## 🛠️Tools and Technologies

- Language: Python
- Architectures: ResNet, MobileNetV2, CCNet-12, CBAM
- Data Processing: Numpy, torch transformation, train-test-split
- Frameworks: Pytorch, Scikit-Learn
- Analysis: 3-Fold Cross-Validation, Confusion Matrices, F1-Score Analysis
## 🧬 Data Science Pipeline
1. Image Preprocessing
   
   - Standardizes image dimensions, normalizations and transformations
   - Merges Parkinson and Alzheimer datasets to create balanced, multi-disease training set.
2. Model Setup and Training

   - Implement existing architectures to set basedline benchmarks for Parkinson and Alzheimer's, trained for binary classification tasks
   - Select a few best-performing models to train on combined dataset, trained for multiclassification task
   - Fine-tune the models to improve performance based on matric scores.
3. Evaluation

   - Used 3-fold cross validation to avoid overfit issues, making the models more reliable and robust.
     
## 📈 Model Performances
Alzheimer’s Detection
The models demonstrated high sensitivity in detecting early cognitive decline through stroke analysis.Smaller accuracy becasue the existing architectures were used to process 1-d image, but out project used them for 2-d image processings. 

Best Model: DenseNet121

Key Metric: 69.7%

Parkinson’s Detection
Focused on identifying motor-control irregularities (tremors and pressure variations).

Best Model: CC-Net with CBAM

Key Metric: 92.3%

Multi-Class (Combined) Results
When distinguishing between all three classes simultaneously, the MobileNetV2 provided the most stable F1-Score across the board.

## 📁 Deliverables

- Code: Modular Python scripts for training and inference.

- White up: An 8-page technical write-up detailing the methodology, literature review, and statistical significance of the results.

- Presentation: A slide deck summarizing insights. 

