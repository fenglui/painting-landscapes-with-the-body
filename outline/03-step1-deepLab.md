# Step 1: Semantic Image Segmentation using DeepLab
1. In RunwayML, add DeepLab to a Workspace<br>
    [![Open in RunwayML Badge](https://open-app.runwayml.com/gh-badge.svg)](https://open-app.runwayml.com/?model=genekogan/spade-landscapes)
2. Set these options
    * Inference Options Command === Mask One
    * Inference Options Class == Person
3. Input === Camera
4. Output === Preview
5. Click Run Remotely
6. If all goes well, you should see a semantic image map that looks like the image below.
7. Next, click the Output Export button to save a series of images from the video capture into a folder on your computer.
    * Export Type === Image Directory 
    * File Name === select this to set the name and location for an image directory to store the exported images
    * Stop Model After Export === On
    * Click Export 
    * When finished, click Stop Export
    * Check your new directory for your saved images!

<br></br>
Next [Step 2: Batch Color Labeling using Adobe Photoshop](https://github.com/ellennickles/painting-landscapes-with-the-body/blob/master/outline/04-step2-photoshop.md)