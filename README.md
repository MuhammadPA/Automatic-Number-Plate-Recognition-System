### README: Automatic Number Plate Recognition (ANPR) System

#### Overview
This project implements an Automatic Number Plate Recognition (ANPR) system using YOLOv8 for real-time detection and tracking of vehicles and license plates from video footage. It integrates object detection, vehicle tracking, and OCR to read and store license plate numbers.

#### Features
- **Real-time Vehicle and License Plate Detection**: Utilizes YOLOv8 models for accurate detection.
- **Vehicle Tracking**: Employs SORT for tracking detected vehicles across video frames.
- **License Plate Recognition**: Applies image processing techniques for OCR to read license plate numbers.

#### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/computervisioneng/automatic-number-plate-recognition-python-yolov8.git
   ```
2. Install required packages:
   ```sh
   pip install -r requirements.txt
   ```

#### Usage
1. Load and run the ANPR system:
   ```python
   from ultralytics import YOLO
   import cv2
   from sort.sort import Sort
   from util import get_car, read_license_plate, write_csv
   ```
2. Execute the main script:
   ```python
   python main.py
   ```

#### Output
The results, including detected vehicles and recognized license plate numbers, are saved in a CSV file (`test.csv`).
