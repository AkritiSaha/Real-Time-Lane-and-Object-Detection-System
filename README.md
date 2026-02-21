# 🚗 Autonomous Vehicle Lane & Object Detection System

# 🏢 Developed At
# Codec Technologies

# 📌 Project Overview

This project implements a real-time Lane Detection and Object Detection pipeline for autonomous driving applications using classical computer vision and deep learning techniques.

The system processes dashcam video frames and simultaneously:

-Detects road lane boundaries

-Identifies surrounding vehicles and objects

-Overlays structured visual outputs in real-time

The objective is to simulate a simplified perception module of an autonomous vehicle.


# 🎯 Problem Statement

Autonomous vehicles must:

Stay within lane boundaries

Detect nearby vehicles, pedestrians, and obstacles

Process video frames efficiently in real time

This project builds a foundational perception system that combines both lane tracking and object detection into a unified pipeline.


# 🧠 Technical Approach

The system is divided into two major modules:

1️⃣ Lane Detection Pipeline (Classical Computer Vision)

Steps applied on each video frame:

Convert frame to Grayscale

Apply Gaussian Blur (noise reduction)

Perform Canny Edge Detection

Apply Region of Interest (ROI) Mask

Detect line segments using Hough Transform

Filter lines based on slope

Average left & right lanes

Overlay final lane boundaries

Key Techniques Used:

Edge Detection

Spatial Filtering

Hough Line Transform

Linear Regression-based averaging

2️⃣ Object Detection Module (Deep Learning)

YOLO (You Only Look Once) model

Real-time bounding box detection

Class identification (cars, trucks, pedestrians, etc.)

The YOLO detections are merged with the lane detection output to produce a unified frame.


# ⚙️ Tech Stack

Python

OpenCV

NumPy

Ultralytics YOLO

Matplotlib



# 🚀 How To Run

Install dependencies:

pip install -r requirements.txt

Open Jupyter Notebook:

jupyter notebook

Run all cells sequentially.


# 📊 Key Learning Outcomes

Understanding spatial image processing

Edge detection theory and implementation

Hough Transform mathematics

ROI masking logic

Combining classical CV with deep learning

Real-time video frame processing
