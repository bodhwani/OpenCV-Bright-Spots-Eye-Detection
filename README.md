# Python Eye Detection

This is my simple and hackish eye/retina/pupil detector.
<br>

Operation is simple. Plug in a webcam and run `python pupil_detect.py`. It will show the webcam image. If it sees your iris, it will superimpose a blue dot over it. It will also show (in a box in the upper left) what it thinks your eye is. It will show in another box to the upper slightly-less-left if it thinks it sees a pupil or an iris, and where it thinks the pupil (green) and iris (blue) are (at 2x magnification). If it thinks it sees a sensible pupil/iris combo, it will save a picture with a date stamp in the running directory. Go to the GUI window and push any key to exit (or control-c in the terminal).

Be sure to bring your eye pretty close to the camera, and to be well-lit.

It uses OpenCV cv2 (which uses numpy) to do all the matrix math, camera, and display stuff.

Unfortunately, due to the hackish nature of this program, it will probably only work out of the box on webcams with a similar resolution to mine. If you want it to work on a different resolution (or angle) camera, you will have to tweak it.

### Import packages
- import cv2
- import numpy as np
- import argparse

Run Script :
<br>
python pupil_detect.py
<br>

# Detecting Brightest Spot


### USAGE
- python brightArea.py --image images/retina.png --radius 41
- python brightArea.py --image images/retina-noise.png --radius 41
- python brightArea.py --image images/moon.png --radius 61

# Detecting Multiple Bright Spots

### Usage
- python detect_bright_spots.py --image images/lights_01.png

# Some screenshots - Output 

- Single spot detection

![alt text](/outputImages/singleSpot.png "Eye Point Detection")
<br>
- Multiple spots detection
<br>
![alt text](/outputImages/multiple1.png "Multiple points detection lights")
<br>
![alt text](/outputImages/multiple2.png "Multiple points detection dog")










