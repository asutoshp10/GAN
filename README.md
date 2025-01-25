# Generative Adversarial Networks (GANs) Implementation 🎨

This repository contains an implementation of **Generative Adversarial Networks (GANs)** built from scratch using TensorFlow. It includes three types of GANs: **Normal GAN**, **Conditional GAN (C-GAN)**, and **Pix2Pix GAN**. Each type of GAN serves unique purposes in generating and transforming images, demonstrating the versatility of GAN architectures.

## Types of GANs

### 1. **Normal GAN**
- The generator takes random noise as input and generates images that mimic real images from the training dataset.
- The discriminator is trained to distinguish between real images from the dataset and fake images produced by the generator.
- The two models (generator and discriminator) are trained adversarially, improving their respective performances over time.

### 2. **Conditional GAN (C-GAN)**
- Introduces conditional labels to both the generator and discriminator.
- The generator uses random noise along with a condition (e.g., a class label) to produce images matching the specified condition.
- The discriminator evaluates both the image and its associated condition to differentiate between real and fake pairs.

### 3. **Pix2Pix GAN**
- A conditional GAN designed for paired image-to-image translation tasks (e.g., transforming sketches into realistic images).
- Trains the generator to map input images to output images while the discriminator ensures the output images are realistic and consistent with the input images.

---

## Features

- **GAN Training from Scratch**: All three types of GANs are implemented without using pre-built libraries, showcasing custom training loops and loss functions.
- **Versatile Architectures**: Includes examples of unconditional image generation, conditional generation, and image-to-image translation.
- **Custom Losses**: Incorporates adversarial loss, binary cross-entropy, and mean squared error losses.
- **Visualization**: Periodic visualization of generated images during training.

---

## Requirements

Install the required dependencies using:

```bash
pip install tensorflow numpy matplotlib

