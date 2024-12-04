# GAN-Medical-Imaging
Inspired by the need to bring change and transformative solutions to the world, I have embarked on journey to impact and bring positive change to the healthcare


# Stroke Image Generation using GANs

## Overview

This project implements a **Generative Adversarial Network (GAN)** to generate synthetic stroke-related medical images. The GAN model is trained on stroke images, and the generator creates new, synthetic images that resemble the original dataset. This synthetic data can be used to augment existing datasets, improve model performance, or aid in medical research where annotated stroke data is scarce.

![Stroke GAN](./images/gan_synthetic_images.png)

## Project Components

### 1. **Generator**
The **Generator** network takes random noise as input and produces synthetic images that resemble stroke-related images. The goal of the generator is to fool the **Discriminator** into believing that the images it generates are real.

### 2. **Discriminator**
The **Discriminator** network is a binary classifier that distinguishes between real images (from the dataset) and fake images (produced by the Generator). The goal of the Discriminator is to correctly identify whether an image is real or synthetic.

### 3. **Adversarial Training**
The Generator and Discriminator are trained together in an adversarial process. The Generator improves its ability to generate realistic images, while the Discriminator enhances its ability to differentiate real from fake images.

---

## Requirements

Before running the project, you will need to install the following Python dependencies:

```bash
pip install tensorflow numpy matplotlib
