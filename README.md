# Clinical Skin Lesion Diagnosis

**Authors**: Madamanchi Sai Venkat, Vemula Giri Manohar, Vemavarapu Tejashwini

## Abstract
This research uses Deep Learning and Convolutional Neural Networks (CNNs) to diagnose skin lesions, classifying dermatoscopic images into seven categories of skin cancer using the "HAM10000" dataset. The study addresses data imbalance and compares a simple custom CNN with a more complex VGG-like model to improve diagnostic accuracy and efficiency.

## Introduction
### Overview
Skin cancer diagnosis is a significant public health issue. This project leverages digital imaging and machine learning to improve diagnosis accuracy and efficiency.

### Motivation
Accurate and timely diagnosis is crucial for effective treatment. Traditional methods are laborious and require expertise. A CNN-based Deep Learning system can assist dermatologists, improving diagnostic efficiency.

### Approach
The project uses CNNs to classify skin lesions, utilizing the HAM10000 dataset. It compares different CNN architectures to find the most effective method for medical image analysis.

## Background
The HAM10000 dataset provides over 10,000 dermatoscopic images, aiding in the development of diagnostic models in dermatology. Its diversity enhances model training and diagnostic capabilities.

## Approach
### Data Preparation
- **Dataset**: HAM10000 with 10,015 images across seven categories.
- **Preprocessing**: Images are resized, normalized, and augmented. Class imbalance is addressed through oversampling.

### Model Development
- **Custom CNN**: Sequential architecture with convolutional, max pooling, flattening, and dense layers.
- **VGG-Inspired Model**: Deeper CNN model known for image classification efficacy.
- **Compilation**: Models compiled with sparse categorical cross-entropy loss and Adam optimizer.
- **Training**: Models trained with a validation subset to monitor performance and mitigate overfitting.

### Evaluation
- **Performance Visualization**: Plotting loss and accuracy against epochs.
- **Testing**: Evaluation on a separate test set to determine accuracy.

## Results
### Dataset Characteristics
The HAM10000 dataset shows class imbalance, with Melanocytic nevi being the most prevalent. Gender distribution is relatively balanced.

### Training and Validation Performance
- **Custom CNN**: Training accuracy of 81.51%, validation accuracy of 76.23%.
- **VGG-like Model**: Training accuracy of 89.67%, validation accuracy of 75.11%.
- **Test Accuracy**: 61.41% for custom CNN, 56.27% for VGG-inspired model.

## Discussion
### Model Performance
Data imbalance impacts model performance, with common lesion types overrepresented. More balanced datasets and techniques like oversampling are suggested. Deeper networks might overfit on limited datasets.

### Future Directions
Improvements include using larger, diverse datasets and advanced architectures like ResNet. AI models should complement medical judgment, requiring careful integration into clinical practice.

## Conclusion
CNNs show potential in enhancing dermatological diagnostic processes. Despite challenges, the models achieved commendable accuracy. Further refinement is needed to improve generalization and reduce overfitting, aiming for reliable AI-assisted diagnostic tools to support dermatologists in early and accurate skin cancer diagnosis.
