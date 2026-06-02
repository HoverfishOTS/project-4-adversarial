# Securing Biometric Models

A 10-week summer research project for high school students.

**Title:** Securing Biometric Models (Adversarial AI)
**Research question:** How vulnerable are image-based emotion classifiers to adversarial attacks, and can we defend against them?

## How to start

1. Open [`project_4_adversarial.ipynb`](project_4_adversarial.ipynb) -- or launch it directly in Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HoverfishOTS/project-4-adversarial/blob/main/project_4_adversarial.ipynb)
2. Switch the runtime to **GPU** (Runtime -> Change runtime type -> T4 GPU).
3. Fill in every `TODO` cell from top to bottom.

Ask your instructor if stuck.

## 10-Week Plan

| Week | Tasks |
|------|-------|
| 1 | Learn neural network training, gradients, and backpropagation |
| 2 | Load pre-trained emotion model and FER-2013 dataset & Literature review (1 or 2 references) |
| 3 | Learn theory behind Adversarial Examples and FGSM |
| 4 | Write algorithm to generate adversarial noise |
| 5 | Execute attack on test dataset, record degraded accuracy |
| 6 | Visualize attack: side-by-side original vs altered images |
| 7 | Explore defensive strategies: generate adversarial images |
| 8 | Retrain classifier with clean + adversarial dataset |
| 9 | Interpret security implications and real-world dangers |
| 10 | Prepare final poster/paper with attack architecture and results |

## Datasets

- **FER-2013 (Facial Expression Recognition)** -- Consists of 48x48 pixel grayscale images of faces automatically registered. (Used to attack a pre-trained model). [Kaggle Link](https://www.kaggle.com/datasets/msambare/fer2013)
- **Pre-trained Model: Emotion Detection CNN (.h5)** -- A Keras Convolutional Neural Network pre-trained on FER-2013. You can download the `.h5` weights directly from this repository to skip the training phase. [Kaggle Link](https://www.kaggle.com/datasets/abhisheksingh016/machine-model-for-emotion-detection)

## Key references

- Goodfellow et al., "Explaining and Harnessing Adversarial Examples" (FGSM): <https://arxiv.org/abs/1412.6572>
- TensorFlow FGSM tutorial: <https://www.tensorflow.org/tutorials/generative/adversarial_fgsm>
