---
title: Dithering and guiding - What is Dithering ?
date: 2023-03-09 14:33:00 +0300
categories: [Astrophotography]
tags: [Astrophotography]
math: true
mermaid: true
---
## What is Dithering in Astrophotography ?

In astrophotography, to dither means to shift the pointing direction of your telescope in random directions between subexposures.

This technique is a useful way to create images with a better signal-to-noise ratio by “canceling out” hot pixels, fixed pattern noise (or walking noise), and more.

By moving the pointing direction of the telescope, dithering shifts the stars to a slightly different place in each frame. As you process your images, you will align and stack individual frames based on the stars in each image. 

Astro Photography Tool (APT) can communicate with various guiding programs and devices to monitor your autoguiding performance. This communication between the camera capture software and your devices is necessary to provide dithering. 

The **Sigma clipping pixel rejection** method in different stacking softwares extracts the random pixel data and preserves the signal. The more light frames collected, the better this technique will work.

## The image below shows the Dithering settings page in APT:

![alt text](https://astrobackyard.com/wp-content/uploads/2021/09/auto-dithering.jpg)


## Here is an example of a dithered vs an undithered result :

![alt text](https://astrobackyard.com/wp-content/uploads/2021/09/dithering-before-after-768x1098.jpg)

The "Walking Noise" patttern is obvious and it ruined the whole image. What is worse is that it is almost impossible to remove it in post-processing. So it is almost mandatory to dither every imaging session.