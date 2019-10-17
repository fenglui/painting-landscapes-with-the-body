# Introduction
[Memo Akten Portfolio](http://www.memo.tv/works/#selected-works)<br>
[Memo Akten Learning to See (2017)](http://www.memo.tv/portfolio/learning-to-see/)<br>
[Learning to See: Gloomy Sunday Video](https://vimeo.com/260612034)<br>
[Based on this process for a similar project using a pix2pix model](http://github.com/memo/webcam-pix2pix-tensorflow)<br>
[Christopher Hesse’s Image-to-Image Demo with pix2pix-tensorflow](https://affinelayer.com/pixsrv/)<br>

Semantic Image Synthesis (our goal)<br>
[NVIDIA’s SPADE](https://nvlabs.github.io/SPADE/)<br> 
[SPADE Code](https://github.com/agermanidis/SPADE)<br>
SPADE-Landscapes Model<br>
[![Open in RunwayML Badge](https://open-app.runwayml.com/gh-badge.svg)](https://open-app.runwayml.com/?model=genekogan/spade-landscapes)

Semantic Image Segmentation (our starting point)<br> 
[DeepLab Code](https://github.com/genekogan/deeplab-pytorch)<br>
[COCO-Stuff Dataset: Things and Stuff Classes in Context](https://github.com/nightrome/cocostuff)<br>
DeepLab Model<br>
[![Open in RunwayML Badge](https://open-app.runwayml.com/gh-badge.svg)](https://open-app.runwayml.com/?model=genekogan/DeepLab)

## Overview of Our Process Today
1. Create semantic image maps of our bodies using the DeepLab model
2. Use Adobe Photoshop to batch “color label” our semantic maps
3. Synthesize new images from these semantic maps using SPADE-Landscapes model
4. (Optional) Create a video from our new images with GIF Brewery

<br></br>
Next [Step 1: Semantic Image Segmentation using the DeepLab Model](outline/03-step1-deepLab.md)