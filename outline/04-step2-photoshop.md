# Step 2: Batch Color Labeling using Adobe Photoshop

## Part 1: Get the segmentation map colors from SPADE-Landscapes
1. In RunwayML, add SPADE-Landscapes to a Workspace
2. Input === Segmentation
3. Under Options (on the right), find the tiny `Export Colors` button, above the color labels. Click it to download the color labels to your computer for reference.

<br></br>
(👇Perhaps the trickiest part of the workshop)
## Part 2: Use Photoshop batch color change the images exported from DeepLab
1. Open your first DeepLab image in Photoshop
2. Let’s create an action to save all the steps that we need to update the colors of this image. Then, we can apply that action to the rest of the your DeepLab images.
    1. Launch the Actions panel: Window → Actions
    2. In that panel, click the icon left of the trash can to “create a new action”
    3. Name it Action 1 and click Record
    4. Select the paint bucket 
    5. Click to set the foreground color and type in hex color `#aaaaaa`
    6. Click to fill the white portion of your DeepLab image--watch where you click!
    7. Click to set the foreground color and type in the hex color `#5fdbff`
    8. Fill in the black portion of your DeepLab image with your new color--watch where you click!
    9. Save the image file: File → Save As (save into a new folder)
    10. Close the image file: File → Close
    11. Your Action should have these steps:
        * Set Foreground Color
        * Fill
        * Set Foreground Color
        * Fill
        * Save
        * Close
    12. Press Stop in the Action panel
3. Let’s apply this Action to the rest of the images in your DeepLab directory: File → Automate → Batch
    1. Play, Action: Action 1
    2. Set Source Folder, click Choose… → select your DeepLab directory
    3. Set the Destination Folder, click Choose… → choose the new folder you just created
    4. Click OK to run the batch. If successful, your new folder should be full of images that look something like this:


![demo](https://github.com/ellennickles/painting-landscapes-with-the-body/blob/master/images/demo_Adobe.png)

<br></br>
Next [Step 3: Semantic Image Synthesis using the SPADE-Landscapes Model](https://github.com/ellennickles/painting-landscapes-with-the-body/blob/master/outline/05-step3-spadeLandscapes.md)
