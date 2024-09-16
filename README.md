#This project was completed in June 2024 and has been uploaded to GitHub in September 2024 to showcase the work done during that period.

# Image Colorization with U-Net and GAN 
This project implements image colorization using deep learning models, specifically leveraging a ResNet18-based UNet generator and a PatchGAN discriminator. 
The goal is to take grayscale images and produce realistic colorized versions using a generative adversarial network (GAN). 
The model is trained on a subset of the COCO dataset and uses a combination of adversarial loss and L1 loss to optimize the output, ensuring both color accuracy and realism.

Features:
Multilingual Dataset Support: Trained on a diverse subset of the COCO dataset with 10,000 images for robust performance.

UNet Generator: The generator uses a ResNet18 backbone with skip connections, allowing for the recovery of fine image details during the colorization process.

PatchGAN Discriminator: This discriminator improves the realism of the generated color images by using small image patches to classify real and fake outputs.

Pretraining and Fine-tuning: The model undergoes pretraining using only L1 loss before fine-tuning with adversarial GAN loss.

LAB Color Space: The model converts grayscale images to LAB color space during training, ensuring smooth color transitions.

Real-Time Visualization: Provides a function to visualize the colorization process, comparing grayscale inputs with both the generated and ground-truth color images.

This project showcases the potential of GANs in transforming black-and-white images into vivid, colorized versions, offering a highly effective deep learning pipeline for image colorization.
