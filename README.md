## Camera Calibration with OpenCV

The IPython notebook in this repository contains code to calculate the camera matrix and distortion coefficients using the images in the "calibration_wide" folder.

First of all I launched the notebook with:
jupyter notebook camera_calibration.ipynb

I started to execute the initial code but a package was missing:
```bash
ImportError: No module named 'PyQt4'
```

I activated the Conda environment for the class:
```bash
source activate carnd-term1
```

Nothing changed. Then I installed them with conda inside carnd-term1:
```bash
conda install pyqt
```

But it installed pyqt-5.6.

Then I decided to comment some code on the notebook where QT was required and try to use something else.

The code as is is not working on Mac: the windows showing the image never close. I found the soulution on the ubiquitous [stackoverflow]( http://stackoverflow.com/questions/6116564/destroywindow-does-not-close-window-on-mac-using-python-and-opencv)


Waiting for the paper with the chessboard :)
