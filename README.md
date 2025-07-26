## Breast Cancer Classification using Ultrasound Images

This notebook explores various deep learning models for classifying breast cancer using the "Breast Ultrasound Images Dataset" from Kaggle.

## 1. Data Preparation

- The dataset is downloaded from Kaggle and unzipped.
- The images are loaded and split into training, validation, and test sets. The labels are derived from the folder names: "benign," "malignant," and "normal."

## 2. Models Explored

### a. Simple CNN

A custom-built Convolutional Neural Network (CNN) is implemented and trained on the dataset. The model's performance is evaluated, and the impact of image size on accuracy is explored.

### b. Deeper CNN

A deeper CNN with more convolutional layers is also implemented and trained to see if a more complex model can achieve better results.

### c. ResNet with Linear Probe

A pre-trained ResNet model is used with a linear probe to classify the images. This approach leverages transfer learning by using the features learned by ResNet on the ImageNet dataset.

### d. Vision-Language Model (CLIP)

The CLIP (Contrastive Language-Image Pre-Training) model is used for zero-shot classification and fine-tuning.

#### i. Zero-Shot Classification

The CLIP model is used to classify the images without any training on the breast cancer dataset. This demonstrates the model's ability to generalize to new tasks.

#### ii. Fine-Tuning

The CLIP model is fine-tuned on the breast cancer dataset to improve its performance. A new classification head is added to the vision encoder, and only this head is trained.

## 3. Results

The notebook includes the training and validation accuracy for each model, as well as the test error for the fine-tuned CLIP model. The results show the progression from a simple CNN to a more advanced vision-language model, highlighting the benefits of transfer learning and fine-tuning.
