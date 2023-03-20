---
title: Dithering and guiding - Guide Scope Focal Length
date: 2023-03-10 13:33:00 +0300
categories: [Astrophotography]
tags: [Astrophotography]
math: true
mermaid: true
---

## Choosing the correct focal length of the Guide Scope:

In order to choose the correct focal length of the Guide Scope, there is a formula which lets us calculate the minimum focal length of the guide scope in relation of the main Imaging Scope.

#### Note:

 The minimum focal length of the guide scope is calculated in order to avoid large scales between the pixel scale of the guiding camera and scope and the main imaging scope and camera which leads to poor guiding.


According to the formula, the minimum focal length of the guide scope equals :

                              (s * F * R * 0.1)/(S * E) = Min Focal Length(mm)

### Where :

- s = Guide Camera Pixel Size(µm)
- S = Imaging Camera Pixel Size(µm)
- F = Main Imaging Scope Focal Length(mm)
- R = Imaging Reducer Factor (equals 1 if no reducer is attached)
- E = Acceptable tracking error(pixels) (you can set that to 1)


### Example:

- My guiding camera is the **ZWO ASI 120mm mini**, which has a pixel size of **3.75µm**.
- My main imaging scope is on **500mm** focal length.
- My imaging camera is the **Canon EOS 90D**, which has a pixel size of **3.2µm**.
- For the R value, my camera has an **APS-C sensor**, which has a crop factor of **1.6**.
- Acceptable tracking error is **1 pixel**.

##### According to the formula :

                              (3.75 * 500 * 1.6 * 0.1)/(3.2 * 1) = 93.75mm

So my guide scope focal length should be at a **minimal** value of **93.75mm** to avoid guiding errors.
