## Project 1: Lane Lines Image Detection w/ OpenCV PP POO POO

The goal of this project was to use Python and OpenCV to create an image processing pipeline to detect the lane lines in a video taken from a car travelling along a road. The pipeline I created has the following steps:


1. Convert RGB image to grayscale
2. Apply Gaussian filter to image
3. Use Canny Edge detection to find strong lines within image
4. Apply a Region of Interest Mask in order to just look at the lane lines
5. Hough Transform the image to create two continuous lines, one for each lane line
6. Draw the detected lane lines over top of the original image

The following GIF shows the output of the lane line detection pipeline:
      
![](Project1.gif)

## Project 2: Semantic Segmentation via Deep Neural Net (DNN)

The goal of this project was to create a DNN with PyTorch which would be able produce a semantic segmentation model which achieves a mean Intersection over Union (mIOU) score of >40%.

Semantic Segmentation is the task of catergorizing each pixel in some input image into a specifc class, and for this project specifially, the classes were people, and cars.
Some example input, and corresponding output images can be seen below.

| Original Image  | Semantic Segmentation Output|
| :-------------: |:---------------------------:|
| ![](media/Image1.PNG) | ![](media/SegImg1.PNG)|
| ![](media/Image2.PNG) | ![](media/SegImg2.PNG)|
| ![](media/Image3.PNG) | ![](media/SegImg3.PNG)|

In the first and second outputs, the car has been correctly classified. In the third output image, the people riding the bikes have been correctly identified.

## Project 3: Probabilistic Occupancy Grid Generation from LiDAR Data

In this project, I was given LiDAR sensor readings, with which I converted into a Probabilistic Occupancy Grid. This involved converting the data from spherical coordinates, to a Cartesian coordinate space, creating a logodds occupancy grid, and then converting said grid into the Probabilistic Occupancy Grid. The following image is a visual representation of the LiDAR Scanner (black) with a point cloud of its readings (red).

<p align="center">
  <img src="https://github.com/moward98/moward98.github.io/blob/main/media/ScannerReadings.PNG" />
</p>

After the conversions, the Probabilistic Occupancy Grid can be visalized as follows:
<p align="center">
  <img src="https://github.com/moward98/moward98.github.io/blob/main/media/ProbabilisticGrid.PNG" />
</p>
The colour density of the points represents the probability that the space is occupied (darker = higher probability).
