# 🎯 VisionVoice Assist

### Real-Time Object Detection with Voice Feedback using YOLOv5

------------------------------------------------------------------------

## 📌 Overview

**VisionVoice Assist** is an AI-powered real-time object detection and
voice feedback system designed to assist visually impaired individuals
by converting visual information into speech.

The system uses YOLOv5 for fast and accurate object detection and
integrates Google Text-to-Speech (gTTS) to provide real-time audio
feedback. A user-friendly Tkinter GUI displays detected objects along
with a live video feed and allows dynamic adjustment of the confidence
threshold.

------------------------------------------------------------------------

## 🚀 Features

-   Real-time object detection using YOLOv5\
-   Voice feedback for detected objects\
-   Multi-object recognition with object counting\
-   Confidence threshold adjustment via slider\
-   GUI interface using Tkinter\
-   Prevention of repeated announcements\
-   Live bounding box visualization

------------------------------------------------------------------------

## 🛠️ Technologies Used

-   Python\
-   PyTorch\
-   YOLOv5\
-   OpenCV\
-   gTTS\
-   Pygame\
-   Tkinter\
-   PIL (Pillow)\
-   Scikit-learn

------------------------------------------------------------------------

## 🧠 System Architecture

1.  Webcam captures live video frames.\
2.  YOLOv5 processes each frame.\
3.  Objects are detected above a selected confidence threshold.\
4.  Detected objects are counted and converted into structured speech
    text.\
5.  gTTS converts text into audio.\
6.  Pygame plays the generated speech.\
7.  Tkinter GUI displays live video feed, detected labels, and
    confidence slider.

------------------------------------------------------------------------

## 📂 Project Structure

VisionVoice-Assist/ │ ├── vision_voice.ipynb ├── README.md

------------------------------------------------------------------------

### Install Dependencies

pip install torch torchvision torchaudio\
pip install opencv-python\
pip install gtts\
pip install pygame\
pip install pillow\
pip install scikit-learn

------------------------------------------------------------------------

## ▶️ How to Run

### Run via Jupyter Notebook

jupyter notebook

Open the notebook and run all cells.

### Run as Python Script

python vision_voice.py

------------------------------------------------------------------------

## 🎛️ Adjustable Confidence Threshold

The GUI includes a slider that allows users to dynamically adjust
detection sensitivity:

-   Range: 0.1 -- 1.0\
-   Default: 0.6\
-   Higher value → More strict detection\
-   Lower value → More detections (may include false positives)

------------------------------------------------------------------------

## 🔊 Voice Output Logic

-   Announces objects only when a change is detected.\
-   Counts multiple occurrences (e.g., "2 persons and 1 laptop").\
-   Prevents repeated announcements.

------------------------------------------------------------------------

## 📊 Model Used

YOLOv5s (Small variant)\
Loaded via PyTorch Hub: torch.hub.load('ultralytics/yolov5', 'yolov5s',
pretrained=True)

Pre-trained on COCO dataset (80 object classes)

------------------------------------------------------------------------

## 🌍 Applications

-   Assistive technology for visually impaired users\
-   Smart home systems\
-   Robotics navigation\
-   Surveillance systems\
-   AI accessibility tools

------------------------------------------------------------------------

## 🔐 Limitations

-   Requires internet connection for gTTS\
-   Performance depends on lighting conditions\
-   Limited to COCO dataset object classes\
-   Real-time performance depends on hardware capability

------------------------------------------------------------------------

## 🚀 Future Improvements

-   Offline speech engine integration\
-   Custom object training\
-   Mobile application deployment\
-   Depth estimation for distance awareness\
-   Multi-language voice support

------------------------------------------------------------------------

