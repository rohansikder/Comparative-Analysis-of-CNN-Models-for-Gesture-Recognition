# Comparative Analysis of CNN Models for Gesture Recognition

This repository contains the research and implementation of various Convolutional Neural Network (CNN) models for gesture recognition. The study primarily focuses on comparing the performance of custom-built CNN architectures against transfer learning with VGG-16, using both RGB and grayscale images.

![graymodelmyimages](https://github.com/rohansikder/Comparative-Analysis-of-CNN-Models-for-Gesture-Recognition/assets/80963667/e1034442-1b15-479e-aaff-7f0d6558982e)


## Overview

Gesture recognition systems are crucial in developing intuitive interfaces. This study evaluates different CNN models to understand how image preprocessing techniques and model configurations affect the efficacy of gesture recognition systems.

### Objectives

- To examine the impact of RGB versus grayscale imaging on gesture recognition.
- To evaluate the performance of custom-designed CNNs against pretrained models.
- To investigate the practical implications of different CNN approaches in gesture recognition.

## Dataset

The dataset utilized is the Hagrid dataset, a comprehensive collection of high-resolution gesture images originally over 700GB in size. For this study, a manageable subset was used, resized and preprocessed to fit the computational constraints.

### Data Preparation

- Images resized to 128x128 pixels for uniformity.
- Normalization performed to stabilize learning by scaling pixel values between 0 and 1.

## Models

Two primary approaches were explored in the models:

1. **Custom CNN Architectures:** Developed from scratch, these models were tailored to optimize gesture recognition, varying in layer configurations and activation functions.
2. **Transfer Learning with VGG-16:** Utilized the pre-trained VGG-16 model to leverage its robust feature extraction capabilities, with adaptations to focus on gesture recognition.

### Training

- Models were trained using an Adam optimizer with categorical crossentropy as the loss function.
- Training involved multiple epochs with performance evaluated at each stage to optimize classification accuracy.

## Results

The study's findings highlighted that while RGB models generally outperform grayscale models, both could achieve comparable accuracy in specific contexts. Surprisingly, transfer learning did not yield the expected improvements, which underscores the unique challenges of gesture recognition.

### Performance Metrics

- **RGB Model:** Achieved an overall accuracy of 59%.
- **Grayscale Model:** Demonstrated an accuracy of 50%.
- **VGG-16 Model:** Showed progressive improvements, achieving a validation accuracy of 51.13% by the 10th epoch.

## Conclusion

The results provide insights into the effectiveness and operational performance of different CNN approaches for gesture recognition, revealing both the potential and limitations of current technologies in this field.

## Getting Started

Instructions on how to set up the project locally:
1. Clone the repository:
```bash
git clone https://github.com/rohansikder/Comparative-Analysis-of-CNN-Models-for-Gesture-Recognition.git
```
1. Run the Jupyter notebook:
```bash
jupyter notebook 'Comparative Analysis of CNN Models for Gesture Recognition.ipynb'
```
