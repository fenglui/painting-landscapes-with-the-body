# Step 2: Batch Color Labeling using Adobe Photoshop

## Part 1: Get the segmentation map colors from SPADE-Landscapes
1. In RunwayML, add SPADE-Landscapes to a Workspace
2. Input === Segmentation
3. Under Options (on the right), find the tiny `Export Colors` button, above the color labels. Click it to download the color labels to your computer for reference.
4. Note the hex colors: clouds `#aaaaaa` and sky `#5fdbff`

<br></br>
(👇Perhaps the trickiest part of the workshop)
## Part 2: Use Photoshop batch color change the images exported from DeepLab
1. Open your first DeepLab image in Photoshop
2. Let’s create an action to save all the steps that we need to update the colors of this image. Then, we can apply that action to the rest of the your DeepLab images.
    1. Launch the Actions panel: `Window → Actions`
    2. In that panel, click the icon left of the trash can to `create a new action`
    3. Name it `Action 1` and click the `record button`
    4. Let's make the first color change:
        1. Click to set the `foreground color` and type in cloud hex color `#aaaaaa`
        2. Select everything that is white: `Select → Color Range'
        3. ...and from the `Select` drop-down menu, choose `Highlights` and click OK
        4. Now let's fill everything that was selected with the cloud hex color: `Edit → Fill`
        5. ...and from the `Contents` drop-down menu: choose `Foreground Color` and click OK
    5. Let's make the second color change:
        1. Click to set the `foreground color` and type in sky hex color `#5fdbff`
        2. Select the inverse of what is currently selected: `Select → Inverse' 
        3. Now let's fill everything that was selected with a different color: `Edit → Fill`
        4. ...and from the `Contents` drop-down menu: choose `Foreground Color` and click OK
    6. Click the `stop button` in the Action panel
    7. Let’s apply this Action to the rest of the images in your DeepLab directory: `File → Automate → Batch`
        1. Under Play, set the Action to `Action 1`
        2. Set Source Folder, click Choose… → select your DeepLab directory
        3. Set the Destination Folder, click Choose… → choose the new folder you just created
        4. Click OK to run the batch. 
        5. Final result: a folder full of these!<br>
        ![demo](https://github.com/ellennickles/painting-landscapes-with-the-body/blob/master/images/demo_Adobe.png)


(Here's an alternative method for changing the colors using the paint bucket tool, but it's not as good at the above. Why? Because this version here is dependent on mouse location and continous areas of color. Here's a [video](https://www.youtube.com/watch?v=VBFle_SIFEE) with all the steps.)

  
<br></br>
Next [Step 3: Semantic Image Synthesis using the SPADE-Landscapes Model](https://github.com/ellennickles/painting-landscapes-with-the-body/blob/master/outline/05-step3-spadeLandscapes.md)
