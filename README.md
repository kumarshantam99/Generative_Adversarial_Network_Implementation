# Generative_Adversarial_Network_Implementation
## Implementation of Pipeline to build a GAN from scratch and generating new images.


### Objectives
1. Setting up of environment
2. Building a Data pipeline
3. Creating a generator and discriminator
4. Buildinga a new custom training loop
5. Generating new images


### Introduction

![GAN Architecture](filename)

Generative Adversarial Networks (GANs) are a class of generative AI models that have revolutionized the field of artificial intelligence by generating realistic and high-quality content. GANs consist of two neural networks: a generator and a discriminator, which work in a competitive setting.

The generator network takes random noise as input and generates synthetic samples, such as images, based on that noise. Initially, the generator produces crude outputs that do not resemble the desired data distribution. The discriminator network, on the other hand, receives both real and generated samples and aims to distinguish between them accurately. It learns to differentiate between real and fake samples by updating its weights during the training process.

GANs have demonstrated remarkable success in generating high-fidelity images, realistic audio, and even text. They have been employed in various creative applications, such as art generation, image synthesis, and data augmentation. GANs have also found applications in improving image quality, anomaly detection, and style transfer.

In every GAN, you supply a Random Noise Seed or a latent vector which can be a dimensional or two-dimensional array that is sent as a noise as an input to the generator. The generator network upscales this array to create a fake two-dimensional image. Now both the fake and real images are sent to the discriminator network which is trained to sort the real and fake images.

Based on the generator loss and discriminator loss the fine-tuning is done to a maximum number of epochs.

5 STEPS TO GANs
•	Define the GAN architecture based on the application
•	Train the discriminator to distinguish real from fake
•	Train the generator to fake the data which can fool the discriminator and look realistic
•	Continue discriminator and generator training for multiple epochs.
•	Save the generator model to create new fake data.
During the training of the generator, the discriminator values as a constant similarly while training the discriminator holds the generator value as a constant. Each should be trained under a static adversary.


