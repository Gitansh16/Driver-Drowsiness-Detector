<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=180&section=header&text=Driver%20Drowsiness%20Detector&fontSize=34&fontAlignY=35&animation=fadeIn"/>


A real-time Driver Drowsiness Detection system developed using Python, OpenCV, dlib, and facial landmark detection techniques to monitor driver alertness and reduce the risk of road accidents caused by fatigue and drowsiness.

The system continuously tracks the driver's eye movements using a webcam and calculates the Eye Aspect Ratio (EAR). If the driver's eyes remain closed for a prolonged period, the system detects possible drowsiness and immediately triggers an audio and visual warning alert.

This project demonstrates the practical application of computer vision and real-time monitoring systems in intelligent transportation and road safety solutions.

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Problem Statement

Driver fatigue and drowsiness are among the leading causes of road accidents worldwide. Long driving hours, lack of sleep, and reduced attention significantly increase the chances of collisions and life-threatening situations.

Traditional monitoring systems often require expensive hardware or specialized sensors, making them difficult to deploy widely.

Major challenges include:

- Detecting driver fatigue in real time
- Preventing accidents caused by reduced attention
- Providing immediate warning systems
- Creating affordable and accessible safety solutions
- Ensuring continuous monitoring without intrusive hardware

This project addresses these issues by building a lightweight computer vision-based drowsiness detection system using only a webcam and facial landmark analysis.

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Project Objectives

The primary objectives of this project are:

- To detect driver drowsiness in real time
- To monitor eye movement continuously
- To calculate Eye Aspect Ratio (EAR)
- To trigger alerts during fatigue conditions
- To improve road safety using computer vision
- To develop a lightweight and affordable monitoring system
- To demonstrate real-time facial landmark tracking

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Core Features

## Real-Time Face Detection

The system uses the `dlib` facial detector to identify the driver's face from webcam video input in real time.

## Facial Landmark Detection

The project utilizes the `shape_predictor_68_face_landmarks.dat` model to detect facial landmarks and accurately locate the eyes.

## Eye Aspect Ratio (EAR) Calculation

The system computes the Eye Aspect Ratio to determine whether the driver's eyes are open or closed.

EAR helps measure eye blinking behavior and prolonged eye closure.

## Drowsiness Detection Logic

If the Eye Aspect Ratio remains below a predefined threshold for a continuous number of frames, the system classifies the condition as driver drowsiness.

## Audio Warning Alert

An alert sound is played using `pygame` whenever drowsiness is detected.

## Visual Warning Display

A warning message appears on the video feed to immediately notify the driver.

## Webcam-Based Monitoring

The project works with a standard webcam and does not require expensive external hardware or sensors.

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# How the System Works

## 1. Webcam Video Capture

The webcam continuously captures live video frames.

## 2. Face Detection

The system detects the driver's face using dlib's frontal face detector.

## 3. Facial Landmark Extraction

Eye landmarks are extracted using the 68-point facial landmark predictor.

## 4. Eye Aspect Ratio Calculation

The Eye Aspect Ratio is calculated using eye landmark coordinates.

## 5. Drowsiness Analysis

If:

```bash
EAR < 0.25
```

for:

```bash
20 consecutive frames
```

the system identifies potential drowsiness.

## 6. Alert Generation

The system:

- Plays an audio warning
- Displays a visual alert
- Continues monitoring until the eyes reopen

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Advantages of the Project

- Real-time drowsiness monitoring
- Lightweight and affordable implementation
- No specialized hardware required
- Improves road safety
- Easy to deploy and test
- Webcam-based monitoring
- Real-time alert system
- Simple and understandable logic
- Practical computer vision application

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Technologies Used

## Programming Language

- Python

## Libraries and Frameworks

- OpenCV
- dlib
- imutils
- scipy
- pygame

## Computer Vision Techniques

- Facial Landmark Detection
- Eye Aspect Ratio (EAR)
- Real-Time Video Processing
- Face Detection

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Installation and Setup

## Install Dependencies

```bash
pip install opencv-python dlib imutils scipy pygame
```

## Required Files

Place the following file inside the `models/` directory:

```bash
shape_predictor_68_face_landmarks.dat
```

Ensure:

```bash
music.wav
```

is present in the same directory as:

```bash
Drowsiness_Detection.py
```

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Running the Project

Run the system using:

```bash
python Drowsiness_Detection.py
```

After execution:

- Allow webcam access
- The system will start monitoring the driver
- Alerts will trigger automatically during drowsiness detection

Press:

```bash
q
```

to quit the application.

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Applications

This project can be applied in:

- Smart transportation systems
- Vehicle safety systems
- Driver monitoring solutions
- Accident prevention systems
- Computer vision research
- Intelligent surveillance systems

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Limitations

- Works best under good lighting conditions
- Accuracy may reduce with occlusions or sunglasses
- Webcam quality affects detection performance
- Prototype implementation for educational purposes

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Future Enhancements

Potential future improvements include:

- Deep learning-based fatigue analysis
- Head pose estimation
- Yawning detection
- Mobile application integration
- Infrared/night vision support
- Cloud-based monitoring
- IoT vehicle integration
- Multi-driver support

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Educational Value

This project demonstrates practical implementation of:

- Computer Vision
- Facial Landmark Detection
- Real-Time Video Processing
- Human Attention Monitoring
- OpenCV Applications
- AI-Based Safety Systems

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Conclusion

The Driver Drowsiness Detector is a real-time intelligent monitoring system developed to improve road safety and reduce fatigue-related accidents.

By combining computer vision, facial landmark detection, and Eye Aspect Ratio analysis, the system provides an affordable and efficient driver monitoring solution capable of detecting drowsiness and generating immediate alerts.

The project highlights the practical role of AI and computer vision in intelligent transportation and human safety systems.

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=2.5"/>

# Developer

Gitansh Pise

GitHub:
https://github.com/Gitansh16

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=120&section=footer"/>
