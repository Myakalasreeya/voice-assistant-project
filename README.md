Real-Time Object Detection with SOS Feature

This project implements a real-time object detection system using Python. It uses pre-trained deep learning models such as YOLO and SSD for object recognition. Built using OpenCV and TensorFlow, the system can identify objects from a live webcam or video stream and optionally trigger an SOS alert when specific objects (e.g., weapons, fire) are detected.

---

Hardware Requirements

- Laptop/PC with camera or USB webcam
- Optional: Raspberry Pi or Jetson Nano for edge deployment
- Power Supply (for mobile setups)
- Internet (for downloading models and updates)

---

Software Requirements

- Python 3.7+

Libraries:

- opencv-python
- tensorflow
- numpy
- matplotlib

imutils

- pyaudio (if using with voice commands)
- IDE: Jupyter Notebook, PyCharm, or VS Code

Install dependencies

- pip install -r requirements.txt

---

Model Support

- Supported object detection models:

> YOLOv3 / YOLOv4 / YOLOv5
> SSD (Single Shot Detector)
> MobileNetV2
> Faster R-CNN (for higher accuracy)

Pre-trained weights can be loaded from TensorFlow Model Zoo or Darknet YOLO format.

---

Setup & Usage

1. Clone Repository
   git clone https://github.com/your-repo/object-detection-sos.git
   cd object-detection-sos
2. Download Pre-trained Model Place your downloaded .pb or .pt model inside the models/ folder.
3. Run Main Script
   python detect.py

This will:

- Start your webcam
- Detect objects in real-time
- rigger an SOS action (e.g., print/log alert) if a predefined threat object is found

---

Features

- Real-time object detection from video feed
- Supports multiple deep learning models (YOLO, SSD, MobileNet)
- Modular and customizable detection classes
- Optional integration with:
  > Email/SMS alert system
  > Text-to-Speech or Buzzer alert
  > GPS tagging
- Portable to embedded systems (e.g., Raspberry Pi)

---

Example Output

- Bounding boxes and labels will be drawn on screen:

[Person] Confidence: 0.87

---

Customization

- To add a new object class:
  > Update coco.names or relevant labels file
  > Modify class detection threshold in detect.py

---

Future Enhancements

- Add facial recognition for intruder alert
- Implement object tracking (DeepSORT)
- Edge optimization with TensorRT or ONNX
- Multi-camera support
- SMS/GPS-based emergency notification

---

Developed By

- G. Yamini Siri[160621737301]
- S. Akshitha[1606021737047]
- M. Sreeya[160621737305]

Stanley College of engineering and technology for women
Information technology
2025
