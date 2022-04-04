## Style Transfer using CycleGAN

### Project Overview
- One of the complicated tasks in medical imaging is to diagnose MRI(Magnetic Resonance Imaging). Sometimes to interpret the scan, the radiologist needs different variations of the imaging which can drastically enhance the accuracy of diagnosis by providing practitioners with a more comprehensive understanding.
- But to have access to different imaging is difficult and expensive. With the help of deep learning, we can use style transfer to generate artificial MRI images of different contrast levels from existing MRI scans. This will help to provide a better diagnosis with the help of an additional image.
- This project uses **CycleGAN to create T2 weighted MRI scan images from T1 weighted MRI scan images and vice-versa.**
- **Modified U-Net Architechture** was used to build both the **Generator** as well as the **Discriminator.**
- **Data Preprocessing** steps such as ***Data Normalization, Image Resizing and Reshaping, Creating tensor batches*** were performed.
- **Binary Cross-Entropy Loss** was defined for both the Generators and Discriminators, and **Adam** optimizers were used.
- Model generates good translated MRI scan images around **150 Epochs**.

## Generated MRI Images before Training:

![first_mri](/images/gan_first.png)

## GIF of Generated Images during Training:
![mri_gif](/images/gan_gif.gif)
