# Adversarial Attacks on Deep Neural Networks

## Project Overview

This project focuses on understanding and implementing adversarial attacks on Deep Neural Networks (DNNs) using the MNIST digits dataset. The main objectives include exploring both untargeted and targeted adversarial perturbations, evaluating the effectiveness of adversarial training as a defense mechanism, and assessing the robustness of retrained DNNs against adversarial inputs.

## Dependencies

- Python 3.8+
- TensorFlow or PyTorch
- NumPy
- Matplotlib (for visualization)

## Dataset

The project utilizes the MNIST digits dataset, which includes 28x28 grayscale images of handwritten digits. This dataset is integrated within the TensorFlow and PyTorch libraries, making it easily accessible for the experiments.

## Implementation Details

### Model Architecture

The baseline DNN model consists of a single-layer network with a 784-dimensional input layer (corresponding to the 28x28 images) and a 10-dimensional output layer (representing the class probabilities for digits 0-9).

### Adversarial Attacks

1. **Untargeted FGSM Attacks**: Implement the Fast Gradient Sign Method (FGSM) to generate adversarial perturbations aimed at misleading the DNN. Measure and report the success rate of these attacks.
   
2. **Targeted FGSM Attacks**: Modify the FGSM implementation to enforce misclassification into specific target classes, evaluating the success rate of these targeted perturbations.

### Adversarial Training

Implement adversarial retraining strategies by incorporating adversarially perturbed images into the training process. Evaluate the classification accuracy of the retrained model on clean inputs and its robustness against new adversarial samples.

## Outputs

- Colab Notebook detailing the implementation and results.
