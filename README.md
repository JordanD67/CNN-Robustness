# Adversarial Attack Generator

## Project Summary
This project explores the generation of adversarial perturbations using a neural network trained to produce noise directly from input images.  
The goal is to replace iterative optimization attacks (like PGD) with a learned generator capable of quickly producing effective adversarial examples.

---

## Objective
Train a model that learns the mapping:
image → adversarial_noise so that adding the generated noise causes a classifier to misclassify the image.

---

## Approach
- **Dataset:** Generate `(image, adversarial_noise)` pairs using PGD on MNIST.  
- **Model:** Train a generator (e.g., U-Net) to predict adversarial noise from clean images.  
- **Evaluation:** Test attack success on the original model and transferability to other models.


