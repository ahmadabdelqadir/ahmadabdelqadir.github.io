---
title: Dithering and guiding - Dithering Distance - PHD2 + APT
date: 2023-03-09 12:33:00 +0300
categories: [Astrophotography]
tags: [Astrophotography]
math: true
mermaid: true
---

In order to decide the dithering distance, there is a formula which helps us decide what is the optimal distance in relation of both **guide scope + camera** and the **main scope + camera**.

In order to move **"X"** amount of pixels between the subexposures, the general formula is:

                                            X / Dither Scale

This formula returns a number which then we can use to decide the Dithering distance in APT, and then PHD2.

## Dither Scale:

We can calculate the dither scale with the help of this formula :

                    Guide Camera Pixel Scale / Imaging Camera Pixel Scale = Dither Scale

## Pixel Scale:

In order to calculate the pixel scale of both cameras, you need to look up the **Pixel Size** of your camera sensor.
After finding out what is the camera's Pixel Size we can do the following:

        (Guide Camera Pixel Size * 206) / (Guide Scope Focal Length) = Guide Camera Pixel Scale
        (Imaging Camera Pixel Size * 206) (Guide Scope Focal Length) = Imaging Camera Pixel Scale

We then can calculate the Dither Scale, which allows us to calculate the number we need to decide what settings we need to dial in APT and PHD2.

## Example:

- Guide camera Pixel Size = 3.75µm
- Imaging camera pixel size = 3.2µm
- Guide scope focal length = 120mm

                    3.75 * 206 / 120 = 6.4375 arc/pixel = Guide Camera Pixel Size
                    3.2 * 206 / 120 = 5.49 arc/pixel = Imaging Camera Pixel Size

                        Dither Scale = 6.4375 / 5.49 = 1.171875

                Lets say we want to move by 20 pixels after each subexposure:

                        20 / Dither Scale = 20 / 1.171875 = 17.06
                
        Since the guide camera Image scale is 1.171875 times the Imaging Camera Pixel Size
        We can say that if the dither distance in APT for the imaging camera is "X", then
        the dither distance / scale in PHD2 for the guiding camera is 1.171875*x.

        We can then do the following :

                                    x * 1.171875x = 17.06
                By taking the positive result, x ends up being equal to 3.81
                                    and 1.171875x = 4.47
             which results roughly in 4.5 in PHD2 and 4 as dithering distance in APT

