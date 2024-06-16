# Brain-Tumour-Classification

## Problem Statement:
Radiology is a broad subject that needs more knowledge and understanding of medical science to identify tumors accurately. The need for a tumor detection program, thus, overcomes the lack of qualified radiologists. Using magnetic resonance imaging, biomedical image processing makes it easier to detect and locate brain tumors. In this study, a segmentation and detection method for brain tumors was developed using images from the MRI sequence as an input image to identify the tumor area. This process is difficult due to the wide variety of tumor tissues in the presence of different patients, and, in most cases, the similarity within normal tissues makes the task difficult. The main goal is to classify the brain in the presence of a brain tumor or a healthy brain.

![MRI of a patient with anaplastic astrocytoma](https://upload.wikimedia.org/wikipedia/commons/d/d8/Anaplastic_astrocytoma.jpg)

## Overview

This project focuses on the classification of brain tumor images into four distinct classes: 'glioma', 'meningioma', 'notumor', and 'pituitary'. The primary approach involves fine-tuning the VGG16 model using the PyTorch framework. Additionally, Python's OpenCV library is utilized for image processing, and various image augmentation techniques are applied to enhance model generalization.

## Technologies Used

- **PyTorch:** The deep learning framework for model development and training.
- **OpenCV:** Used for image processing tasks.
- **Python:** The primary programming language for the project.

## Model Architecture

The VGG16 model is employed as the base architecture for the brain tumor classification task. The model is fine-tuned to adapt to the specific requirements of the project.

## Image Augmentation Techniques

To enhance the model's robustness and improve generalization, the following image augmentation techniques are applied:

- Rotation
- Scaling
- Horizontal and Vertical Flipping
- Brightness and Contrast adjustments

## Optimization Techniques

Several optimization techniques are experimented with to fine-tune the model:

1. **Stochastic Gradient Descent (SGD):** A traditional optimization algorithm.
2. **Adam:** An adaptive learning rate optimization algorithm.
3. **RMSprop:** Another adaptive learning rate optimization algorithm.
4. **AdaGrad:** Adaptive gradient optimization algorithm.


## Snapshot Learning using VGG-16
Snapshot learning is a training technique that involves saving multiple snapshots of a model during its training process. This approach is particularly useful for ensemble learning, where combining multiple models can lead to better performance and generalization. One popular architecture for implementing snapshot learning is the VGG-16 model.

Snapshot learning involves training a single model and periodically saving the state of the model (snapshots) at different points in the training process. These snapshots are then used to create an ensemble model that combines the predictions of all saved snapshots, often leading to improved performance.





## Experimentation and Tuning

The optimization parameters for each technique are carefully tuned to achieve optimal performance. The model undergoes thorough experimentation to identify the best combination of hyperparameters and optimization algorithms for the given task.

## Conclusion

The Brain Tumour Classification project demonstrates the successful implementation of a fine-tuned VGG16 model for accurately classifying brain tumor images into four classes. The combination of image augmentation techniques and experimentation with various optimization algorithms contributes to the overall success of the project.

For detailed implementation code and results, refer to the project repository and notebooks.
