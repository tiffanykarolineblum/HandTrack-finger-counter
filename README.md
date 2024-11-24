# ✋ HandTrack: Real-Time Finger Counting with OpenCV ✨
This project implements a real-time finger counter using **OpenCV**, a powerful computer vision library. The program detects and counts the number of visible fingers within a defined region of interest (ROI) in a webcam feed. It leverages image processing techniques such as background subtraction, thresholding, contour detection, and convex hull analysis to accurately segment and count fingers.

---

## Key Features

- **Background Modeling**: Initializes a static background for the ROI to effectively segment hand movements.
- **Segmentation**: Isolates the hand from the image using absolute difference and thresholding.
- **Finger Counting**: Determines the number of fingers by analyzing the convex hull and identifying the most extreme points.

---

## Applications

This project is ideal for:
- **Real-time gesture-based control systems**
- **User-friendly interfaces** for IoT or AR devices
- **Interactive games** controlled by hand movements

---

## Features

- Real-time analysis and visualization of hand segments.
- Finger counting using a circular region of interest (ROI) to filter out irrelevant objects.
- Adaptive to different hand positions and movements.

---

## Tech Stack

- 🐍 **Python 3.x**
- 👁️‍🗨️ **OpenCV** (Computer Vision)
- 🔢 **NumPy** (Numerical computations)
- 🧮 **scikit-learn** (for Euclidean distance calculations)

---

## How It Works

1. **Background Modeling**:
   - The camera is initialized, and the background modeling takes place during the first 60 frames.
2. **Real-Time ROI Analysis**:
   - Once the background is captured, the program analyzes the ROI in real time.
3. **Hand Segmentation and Counting**:
   - The program detects and segments the hand, counting the number of visible fingers.
4. **Display Results**:
   - The contours of the hand and the finger count are displayed on the screen.

---

## Requirements

Install the following dependencies:
- `opencv-python`
- `numpy`
- `scikit-learn`

You can install them using:
```bash
pip install -r requirements.txt
