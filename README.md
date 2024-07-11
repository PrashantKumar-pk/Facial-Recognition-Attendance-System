# Facial Recognition Attendance System

This project implements an automated attendance system using facial recognition technology. It captures video from a webcam, detects faces, and marks attendance for recognized individuals.

## Features

- Real-time face detection and recognition
- Automatic attendance logging with timestamps
- Support for multiple individuals
- Easy setup and configuration

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- NumPy
- face_recognition
- A webcam

## Installation

1. Clone this repository: git clone https://github.com/yourusername/facial-recognition-attendance.git
2. Install the required packages 
3. Make a folder named "imageAttendance" and drop the photos of subjects in it, making sure they're in jpg format.

## Usage

1. Add photos of individuals to the `imageAttendance` folder. Name each file with the person's name (e.g., "John_Doe.jpg").

2. Run the script: python AttendanceProject.py

3. The webcam will activate and start recognizing faces. Recognized individuals will have their names displayed on the video feed.

4. Attendance is automatically logged in `Attendance.csv` with the name and timestamp of each recognized individual.

## How it works

1. The script loads images from the `imageAttendance` folder and encodes the faces.
2. It then captures video from the webcam and detects faces in each frame.
3. Detected faces are compared against the known face encodings.
4. If a match is found, the name is displayed on the video feed and logged in the attendance file.

## Customization

- Adjust the `path` variable to change the folder where images are stored.
- Modify the `markAttendance` function to change how attendance is logged.
