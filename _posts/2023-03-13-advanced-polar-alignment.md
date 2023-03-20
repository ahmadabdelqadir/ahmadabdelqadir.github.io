---
title: N.I.N.A Three Point Polar Alignment (Without a Polar Scope)
date: 2023-03-13 14:10:00 +0300
categories: [Polar Alignment, Astrophotography]
tags: [Polar Alignment]
render_with_liquid: false
---

A software called N.I.N.A (Nighttime Imaging 'N' Astronomy) can help achieve an almost perfect Polar Alignment.

## Download the Plugin

After downloading the software, you are going to need to head to the Plugins tab and download the plugin called : "Three Point Polar Alignment".

![alt text](https://www.sternwarte-meckesheim.de/wp-content/uploads/2022/02/nina_astap_plugin_2.png)

## Configure Settings

Head to the Options tab and configue your camera and the focal length of the scope you are attaching your camera to.

Connect both the camera, and the Mount.

##### Note: Putting in the wrong focal length can lead to a failure in the Polar Alignment


## Download ASTAP (Astrometric Stacking Program)

This program will be used by N.I.N.A to plate solve the images the camera will capture

##### Download a Star DataBase from the same website


## Configure Plate Solver Settings

Head to the Options Tab and choose Plate Solving. Choose ASTAP as the plate solver.
Then in the plate solver settings, select ASTAP and browse the ASTAP location to where you installed it.


## Sequencer and Advanced Sequencer

Head to the Sequencer tab, and select Advanced sequencer.

Now scroll down and drag the "Three Point Polar Alignment" to the Sequencer.
Turn on "Start from current position".

Adjust the exposure and gain for you camera. I personally use 2 seconds exposure and 50 gain since i Use the ZWO ASI 120mm mini as the guide camera.

Hit the play button and the camera should start taking exposures and N.I.N.A will tell the mount to slew the amount of degrees was dialed in the settings. 

After this procedure ends, the camera will continue taking exposures and ASTAP will plate solve these images and the amount of error will be displayed on the screen. 

According to the instruction on screen, you have to adjust the mount's latitude and Azimuth with the correct bolts.

After reaching an acceptable error margin, you are all set and polar aligned.

![alt text](https://www.cloudynights.com/uploads/monthly_02_2022/post-335382-0-60380100-1644227605.jpg)


