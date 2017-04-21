---
layout: post
title: Metis Final Project
---
## Identifying Blurry Photos with AI
For my final project I wanted to classify good and bad quality photos using a neural network. I thought this would be useful when I uploaded several hundred photos from my digital SLR camera and needed to sort through them. My initial experimentation involved applying transfer learning to the "Inception" architecture, which is pre-trained for photo classification. However, I quickly realized that since my primary goal was to identify and separate blurry photos from a library of images, I needed a convolutional neural network (CNN) architecture that simply did well with edge detection. Thus I started with the LeNet architecture, often considered a good starting point for a basic CNN. This architecture has 5 layers: 2 convolutional layers and 3 dense (fully-connected) layers. I trained the model using clear images and images with an artificial blur applied (Gaussian blur using OpenCV).