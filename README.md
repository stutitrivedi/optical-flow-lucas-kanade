# optical-flow-lucas-kanade
 Improved Lucas-Kanade optical flow to remove static corners and highlight only moving objects.

This project focuses on improving the results of a Lucas-Kanade sparse optical flow implementation. The original program, as provided in the course material, detects many static corner points that do not belong to moving objects. The task is to modify the code so that it filters out these "still" corners and tracks only the truly moving features in the video.

Problem Statement

In motion detection using optical flow, many corner points may be detected across both static and dynamic regions. However, corners on non-moving areas can create misleading results. The objective of this assignment is to improve the Lucas-Kanade method by excluding points with negligible motion, as demonstrated in the comparison between the original and expected outputs.

Solution Overview

Modification of the Lucas-Kanade optical flow implementation provided in the sample code.

A motion threshold to eliminate static or nearly static points that do not represent movement.

Visual tracking output that includes only the relevant moving points.

Relative file paths used for reading input and saving output.

Well-commented code for clarity and academic review.

Key Features

Improved filtering of corner points based on displacement

Tracks only moving features frame-to-frame

Fully written in a Jupyter notebook format as per submission guidelines

Uses OpenCV and NumPy libraries

Does not include video files as required

Project Structure

optical-flow-lucas-kanade/

OpticalFlow.ipynb : Jupyter Notebook with enhanced Lucas-Kanade implementation

Figure1.jpg : Sample frame with original noisy corner detection

Figure2.jpg : Sample frame with improved corner detection (expected result)

README.md : Project description and instructions


Requirements

Python 3.x

numpy

opencv-python
