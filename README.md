Mars Terrain Image Segmentation
Project Overview
This project is the second homework assignment for the "Artificial Neural Networks and Deep Learning" course. The task is to perform semantic segmentation on 64x128 grayscale images of Martian terrain. The goal is to develop a deep neural network that accurately classifies each pixel into one of five categories: Background, Soil, Bedrock, Sand, and Big Rock.

<img width="1578" height="299" alt="Image" src="https://github.com/user-attachments/assets/f61b408a-559e-463a-b1f4-5f0b1f0b9c58" />

Our approach involved an initial data inspection, cleaning of outliers, and extensive experimentation with various U-Net architectures, custom loss functions, and data augmentation techniques to create a model that generalizes well despite the suboptimal quality of the provided dataset. The final model achieved a Mean Intersection over Union (MIoU) of 0.58 on the test set.

Dataset Description
The dataset consists of 64x128 grayscale images of Mars terrain and their corresponding segmentation masks.

Key Challenges & Characteristics
A preliminary analysis revealed several key challenges that guided our development process:

Poor Mask Quality: Many of the provided masks were of low quality, often misrepresenting the intended segmentation of the corresponding image.

Outliers: The dataset contained outlier images, most notably images of aliens that all shared the same mask.

Class Imbalance: Some classes were significantly over-represented in the masks compared to others, which could bias the model during training.

The primary challenge was to create a robust model that could learn meaningful features and generalize well when trained on a noisy and imperfect dataset.
