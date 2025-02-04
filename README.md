# AMD-Detection-using-EfficientNet

## Project Overview
This project focuses on detecting Age-related Macular Degeneration (AMD) in retinal fundus images using EfficientNet. To enhance the model's performance, we incorporate Generative Adversarial Network (GAN) for data augmentation, generating synthetic images that closely resemble real fundus images.

## Objectives
- Implement Generative Adversarial Network (GAN) to generate synthetic retinal fundus images for data augmentation.
- Train an EfficientNet-based Convolutional Neural Network (CNN) model to classify AMD and normal cases.
- Evaluate the impact of GAN-based augmentation on model performance using accuracy, sensitivity, and specificity metrics.

## Methodology
1. Data Collection:
- Open-source retinal fundus image datasets, including JSIEC, STARE, RFMID 2.0, and ODIR.
- Two-class classification: Normal vs. AMD.
2. Data Preprocessing:
- Centered Crop & Resize (296×296 pixels).
- CLAHE (Contrast Limited Adaptive Histogram Equalization) for contrast enhancement.
3. Data Augmentation:
Deep Convolutional GAN (DCGAN) generates synthetic fundus images.
4. Model Development:
EfficientNet-B3 is chosen after evaluating various EfficientNet versions (B0-B7).

## Conclusion
This project demonstrates the effectiveness of combining Generative Adversarial Network (GAN) and EfficientNet for detecting Age-related Macular Degeneration (AMD) in retinal fundus images. The use of DCGAN for data augmentation significantly enhances model performance by addressing data imbalance and improving feature representation. Key takeaways from the study include:
- GAN-generated synthetic images closely resemble real fundus images, effectively improving training quality.
- Applying CLAHE preprocessing after GAN augmentation further enhances classification accuracy, with the best performance reaching 92.96% accuracy.
- Although GAN augmentation improves model performance, manual selection of high-quality synthetic images remains necessary.
