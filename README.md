# Deep Learning Based Image Generation

## Project Overview
This project showcases the implementation of a deep learning model for image generation, focusing on the creation of realistic images. Utilizing PyTorch, the project involves setting up Generative Adversarial Networks (GANs) for this purpose.

## Key Features
- **Data Preparation**: The dataset consists of images loaded from a predefined directory. These images are resized, center-cropped, transformed into tensor format, and normalized.
- **Model Architecture**:
  - **Generator**: A neural network model designed to generate images. It includes layers such as ConvTranspose2d, BatchNorm2d, and ReLU activations.
  - **Discriminator**: A neural network model for distinguishing between real and generated images, comprising Conv2d layers, BatchNorm2d, and LeakyReLU activations.
- **Training Process**: The models are trained for a set number of epochs, using Binary Cross Entropy Loss and Adam optimizer. The process includes training the Discriminator with both real and fake images, and subsequently training the Generator.
- **Visualization**: The training process is visualized through plots of Generator and Discriminator losses, and a grid of generated fake images.

### Parameters used for training include:
- Batch size: 128
- Image size: 64x64
- Number of epochs: 15
- Learning rate: 0.0003
- Optimizers: Adam for both Generator and Discriminator
