# Face Detection and Recognition System using OpenCV

## Overview

This project implements a real-time Face Detection and Face Recognition system using Python and OpenCV. The system captures facial images through a webcam, trains a recognition model using collected face datasets, and identifies known individuals in real time.

The project uses Haar Cascade Classifiers for face detection and the Fisher Face Recognizer algorithm for face recognition.

---

## Features

* Real-time face detection using webcam
* Automatic face image dataset collection
* Face recognition using Fisher Face Recognizer
* Identification of registered users
* Detection of unknown persons
* Image capture for unknown faces
* OpenCV-based implementation

---

## Technologies Used

* Python
* OpenCV
* NumPy
* Haar Cascade Classifier
* Fisher Face Recognition Algorithm

---

## Project Workflow

### Step 1: Face Detection

The system detects human faces in real time using OpenCV's Haar Cascade Classifier.

* Captures video from webcam
* Detects faces in each frame
* Draws bounding boxes around detected faces
* Displays live detection results

---

### Step 2: Dataset Creation

The dataset collection module:

* Captures face images from webcam
* Converts images to grayscale
* Resizes images to a fixed size (130 × 100)
* Stores images in a dataset directory

Example:

```text
datasets/
└── Suren/
    ├── 1.png
    ├── 2.png
    ├── 3.png
    └── ...
```

---

### Step 3: Model Training

The training module:

* Reads face images from the dataset
* Assigns labels to each person
* Trains a Fisher Face Recognizer model
* Creates a facial recognition model for real-time predictions

---

### Step 4: Face Recognition

The recognition system:

* Detects faces from webcam feed
* Compares detected faces against trained datasets
* Displays recognized person's name
* Labels unrecognized faces as "Unknown"
* Saves images of unknown persons for further analysis

---

## Screenshots

### Face Detection

![Face Detection](face_detection.png)

### Face Recognition

![Face Recognition](face_recognition.png)

---

## Project Structure

```text
Face-Recognition-System/
│
├── datasets/
│   └── Suren/
│       ├── 1.png
│       ├── 2.png
│       └── ...
│
├── screenshots/
│   ├── face_detection.png
│   └── face_recognition.png
│
├── haarcascade_frontalface_default.xml
├── face_detection.py
├── dataset_creator.py
├── face_recognition.py
└── README.md
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/sriarani16/Face-Recognition-System.git
cd Face-Recognition-System
```

### Install Dependencies

```bash
pip install opencv-python
pip install opencv-contrib-python
pip install numpy
```

---

## Running the Project

### Run Face Detection

```bash
python face_detection.py
```

### Create Dataset

```bash
python dataset_creator.py
```

### Train and Run Face Recognition

```bash
python face_recognition.py
```

---

## Future Improvements

* Deep Learning based face recognition
* Multiple user registration
* Attendance management integration
* Cloud database integration
* Real-time alert notifications
* Improved recognition accuracy using CNN models

---

## Learning Outcomes

This project helped develop skills in:

* Computer Vision
* OpenCV Development
* Image Processing
* Machine Learning Fundamentals
* Real-Time Video Processing
* Python Programming

---

## Author

**Sriarani Surenther**

Master of Information Technology (First Class Honours)
University of Waikato

GitHub: https://github.com/sriarani16
LinkedIn: https://www.linkedin.com/in/sriarani-surenther
