What Is... Computer Vision
===

**WARNING: This What is... contains far too many acronyms**

![OpenCV](../images/FootfallGif.gif)

## Summary
What is computer vision? 

In laymen’s terms, it is the field of allowing computers to process and understand visual data be that digital images of videos.

OpenCV (Open Computer Vision) is the most popular library of functions which focuses on image analysis, processing and evaluation. It has C++, Python, Java and MATLAB interfaces ie libraries for each language. It is supported by Windows, Linux, Android, iOS and MacOS

OpenCV is used in a range of products and computing systems, such as the field of robotics, Virtual Reality, Automonous Cars, Augmented Reality and ANPR (Automatic Number Plate Recognition). It has more than 2500 algorithms that can perform tasks such as recognizing faces, identifying objects, track moving objects and stiching images together. One way you can think about OpenCV in a reductive way is like the filters in Photoshop.

So there are a number of subsystems / modules of OpenCV well just talk about them in high level.

#### Subsystems

* Image Enhancement
* Transformations
* Filtering
* Color Vision
* Feature Extraction
* Pose Estimation
* Registration
* Visual Recognition

#### Modules
Module | Function
--- | --- 
core | Core functionality 
imgproc | Image processing 
imgcodecs | Image file reading and writing 
videoio | Video I/O 
highgui | High-level GUI 
video | Video Analysis 
calib3d | Camera Calibration and 3D Reconstruction
features2d | 2D Features Framework
objdetect | Object Detection
dnn | Deep Neural Network module
ml | Machine Learning
flann | Clustering and Search in Multi-Dimensional Spaces
photo | Computational Photography
stitching | Images stitching
cudaarithm | Operations on Matrices
cudabgsegm | Background Segmentation
cudacodec | Video Encoding/Decoding
cudafeatures2d | Feature Detection and Description
cudafilters | Image Filtering
cudaimgproc | Image Processing
cudalegacy | Legacy support
cudaobjdetect | Object Detection
cudaoptflow | Optical Flow
cudastereo | Stereo Correspondence
cudawarping | Image Warping
cudev | Device layer
shape | Shape Distance and Matching
superres | Super Resolution
videostab | Video Stabilization
viz | 3D Visualizer

## Common Uses
Ok so there are alot of modules and subsystems that we can get lost in here. Lets focus on a few of the more common tasks and uses of OpenCV.

* Background Subtraction
* Filtering
* Tracking
* Feature Detection
	* Corner Detection
	* SIFT
	* SURF
	* FAST
	* ORB
	* BRIEF
	* Template Matching

## Gotchas
* Lighting: Lighting affects OpenCV using normal cameras. If you use IR / depth cameras lighting isnt so much of an issue.
* Sunlight and Shadow: Especially if you are using OpenCV outdoors. There are ways to combat this such as MOG Filters.
* Occulusion: People covering the camera
* Camera Choice: poor cameras will result in poor image quality.
* Poorly Optimized Systems: I've been guilty of this before and it haunted me afterward. Make sure your system does only what you need.
* Speed: Be smart about what you are looking at. Do you need to be capturing and analysing images at 1080p 30 frames a second. Could you do it at half the resolution.

## Projects

* [Under Scan](http://www.lozano-hemmer.com/under_scan.php) - Rafael Lozano Hemmer
* [Hand from Above](http://www.chrisoshea.org/hand-from-above) - Chris o'Shea
* [Audience] (http://www.chrisoshea.org/audience) - Random International / Chris o'Shea
* [vNS](http://www.davidrokeby.com/vns.html)  - David Rokeby
* [Videoplace](https://www.youtube.com/watch?v=dmmxVA5xhuo) - Myron Krueger
* [Eyewriter](https://vimeo.com/6503448) - Zach Lieberman 
* [Glow](http://www.frieder-weiss.de/works/all/Glow.php) - Chunky Move 
* [Snout](http://www.flong.com/projects/snout/) - Golan Levin
* [Connnected Worlds](http://design-io.com/projects/ConnectedWorlds/) - DesignIO
* [Laser Tag](http://www.theowatson.com/site_docs/work.php?id=40) - Theo Watson
* [Face Substitutions](https://vimeo.com/29348533) - Kyle McDonald
*[Blind Self Portrait](https://vimeo.com/44489751) - Kyle McDonald

## Useful Resources

* Blair Neal made a handy [guide](https://github.com/laserpilot/Guide_To_Cameras_Interactive_Installations/blob/master/Guide_To_Cameras_For_Interactive_Installations.md) exploring cameras in interactive installations
* Here is the official [Tutorials](https://docs.opencv.org/3.4.1/d9/df8/tutorial_root.html) page from Willow Garage who created and maintain OpenCV.
* Kyle McDonalds [openFrameworks OpenCV Wrapper](https://github.com/kylemcdonald/ofxCv)
* Purely for the fact this is called the [Watershed Algorithm](https://docs.opencv.org/master/d2/dbd/tutorial_distance_transform.html#gsc.tab=0) 
* [Presentation](https://www.cse.unr.edu/~bebis/CS485/Lectures/Intro_OpenCV.pdf) on OpenCV
* [Golan Levin's TED Talk](https://www.ted.com/talks/golan_levin_ted2009)

Some of the things we've done with OpenCV.

* How we did the [Shadow Segmentation](https://blogs.wcode.org/2015/01/playable-city-award-2014-shadowing-part-2-computer-vision/) for Shadowing.
* How to [build OpenCV](https://blogs.wcode.org/2014/10/howto-install-build-and-use-opencv-macosx-10-10/) for MacOs. 
* How use [XCode with OpenCv](https://blogs.wcode.org/2014/11/howto-setup-xcode-6-1-to-work-with-opencv-libraries/).
* Our [Footfall Counter](https://blogs.wcode.org/2015/04/footfall-a-camera-based-people-counting-system-for-under-60/).
* [Foreground Segmentation](https://blogs.wcode.org/2017/01/howto-use-foreground-removal-with-the-microsoft-kinect/) 
* [Using IR Camera with OpenCV](https://github.com/WatershedArts/NewTalentResidencies2018/tree/master/Lawerence%20Hoo%20and%20Michael%20Jenkins)


