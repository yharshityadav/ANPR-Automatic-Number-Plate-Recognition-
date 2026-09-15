# ANPR-Automatic-Number-Plate-Recognition-
An Automatic Number Plate Recognition (ANPR) system using OpenCV and YOLO to detect vehicle license plates and extract registration numbers from uploaded images and video footage. This project explores computer vision, image preprocessing, object detection, and OCR to automate vehicle number plate recognition.

# Automatic Number Plate Recognition Using OpenCV

## 1. Introduction

Automatic Number Plate Recognition (ANPR) is a computer vision technology used to identify and recognize vehicle registration numbers from images or video footage.

This project uses OpenCV, a computer vision library, to process vehicle images, detect potential number plate regions, and extract the registration number using image processing techniques.

The main objective is to automate the number plate recognition process and reduce the need for manual identification.

## 2. Objectives

* To understand the application of computer vision in vehicle identification.
* To process vehicle images using OpenCV.
* To identify potential number plate regions.
* To extract vehicle registration numbers from images.
* To explore the use of image processing in intelligent transportation systems.

## 3. What Is OpenCV?

OpenCV (Open Source Computer Vision Library) is an open-source library used for image processing, computer vision, and video analysis.

It provides various functions for image enhancement, edge detection, contour detection, image segmentation, and object tracking.

In this project, OpenCV is used to process vehicle images and identify regions that may contain a number plate.

## 4. Working Principle

The system follows a sequence of image processing operations to identify the number plate.

### 4.1 Image Acquisition

The process begins by obtaining an image of a vehicle. The image acts as the input for the number plate recognition system.

### 4.2 Image Preprocessing

Preprocessing improves the quality of the input image and makes it easier to identify important features.

Common preprocessing techniques include:

* Grayscale conversion: Converts a colour image into shades of gray.
* Noise reduction: Removes unwanted variations from the image.
* Image enhancement: Improves the visibility of important features.
* Thresholding: Separates foreground regions from the background based on intensity.

### 4.3 Edge Detection

Edge detection identifies significant changes in image intensity.

The Canny edge detection algorithm is commonly used to identify the boundaries of objects. In number plate recognition, these edges can help identify rectangular regions that may contain a license plate.

### 4.4 Contour Detection

Contours represent the boundaries of connected regions in an image.

OpenCV can detect contours and analyse their properties, such as area, shape, and aspect ratio.

These properties help identify potential number plate regions. However, contours alone cannot guarantee accurate plate detection because other objects may have similar shapes.

### 4.5 Number Plate Localization

Number plate localization is the process of identifying the position of a number plate within a vehicle image.

The system examines candidate regions using geometric properties, rectangular shapes, and other visual characteristics.

Once a suitable region is identified, it can be extracted from the original image for further processing.

### 4.6 Character Recognition

After extracting the number plate region, Optical Character Recognition (OCR) can be used to convert the visible characters into machine-readable text.

OCR is a separate recognition process and is not automatically performed by OpenCV's basic image processing functions.

## 5. Role of Image Processing

Image processing plays an important role in improving the quality of vehicle images and identifying relevant visual features.

Techniques such as grayscale conversion, filtering, thresholding, and edge detection help make number plate regions easier to analyse.

The accuracy of these techniques depends on factors such as lighting, image quality, plate orientation, and background complexity.

## 6. Applications

Automatic Number Plate Recognition can be used in:

* Intelligent transportation systems
* Vehicle access control
* Parking management systems
* Traffic monitoring
* Vehicle identification
* Toll collection systems
* Law enforcement and traffic management

## 7. Advantages

* Reduces manual effort in vehicle identification.
* Provides automated image processing.
* Can process vehicle images consistently.
* Supports the development of intelligent transportation systems.
* Can be extended to video-based recognition systems.

## 8. Limitations

Traditional OpenCV-based number plate detection relies heavily on image processing techniques and manually selected parameters.

Its performance may decrease under:

* Poor lighting conditions
* Blurred or low-resolution images
* Rotated or tilted number plates
* Complex backgrounds
* Damaged or partially hidden plates
* Different number plate sizes and formats

The system may also identify incorrect regions when other objects have visual properties similar to a number plate.

## 9. Future Scope

The project can be improved by integrating deep learning-based object detection models such as YOLO.

YOLO can learn visual features from annotated training images and detect number plates using bounding boxes.

Combining YOLO-based detection with OpenCV-based preprocessing and OCR can provide a more flexible approach to automatic number plate recognition.

Future development may also include real-time video processing, multiple vehicle detection, and a web-based interface for image and video analysis.

## 10. Conclusion

The OpenCV-based Automatic Number Plate Recognition project demonstrates how computer vision and image processing techniques can be applied to vehicle identification.

By using preprocessing, edge detection, contour analysis, and number plate localization, the system can identify potential license plate regions in vehicle images.

The project provides a foundation for understanding ANPR technology and can be further enhanced through deep learning and OCR techniques.
