# Face Recognition and Attendance System

This project implements a deep learning-based face recognition and attendance system using TensorFlow and Flask. Developed as part of the MSc Big Data Analytics program at AIMIT, St. Aloysius College, Mangalore, the system enhances physical security and automates attendance recording.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [File Descriptions](#file-descriptions)
- [Methodology](#methodology)
- [System Design](#system-design)
- [Testing](#testing)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction
The Face Recognition and Attendance System is designed to identify individuals and record their attendance automatically. It uses the FaceNet model architecture within a TensorFlow environment, leveraging deep convolutional neural networks for high-accuracy facial recognition. 

## Features
- Real-time face detection and recognition
- Automated attendance recording
- High accuracy using deep learning
- Unauthorized person detection and alert system
- Weekly visualizations of attendance data

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/Au9u5tu-s/FaceNet-FaceRecognition.git
   cd FaceNet-FaceRecognition
   ```

2. Install the required packages:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
1. **Data Preprocessing**:
   Prepare your dataset using `data_preprocess.py`.
   ```sh
   python data_preprocess.py --data_dir <your_dataset_directory>
   ```

2. **Training**:
   Train the FaceNet model using `train_main.py`.
   ```sh
   python train_main.py --data_dir <your_preprocessed_data_directory> --output_dir <output_model_directory>
   ```

3. **Face Detection and Recognition**:
   Use `detect_face.py` for detecting and recognizing faces in images or videos.
   ```sh
   python detect_face.py --input <input_image_or_video> --model <trained_model_directory>
   ```

4. **Classification**:
   Classify new faces using `classifier.py`.
   ```sh
   python classifier.py --model <trained_model_directory> --input <input_image_or_video>
   ```

## File Descriptions
- `classifier.py`: Script for classifying faces.
- `data_preprocess.py`: Script for preprocessing the dataset.
- `detect_face.py`: Script for detecting faces in images or videos.
- `train_main.py`: Main training script.
- `requirements.txt`: List of required packages.
- `README.md`: Project documentation.

## Methodology
The project follows an Agile methodology, ensuring iterative development and continuous collaboration with stakeholders. The neural network is trained using TensorFlow, and Flask is used for the web application interface.

## System Design
The system comprises two main modules:
- **Face Recognition Module**: Detects and identifies individuals, retrieving their details from the database.
- **Attendance Module**: Scans faces to record attendance, updating the database and generating visualizations.

## Testing
The system undergoes multiple levels of testing, including unit testing, integration testing, system testing, and performance testing to ensure robustness and reliability.

## Results
The system successfully identifies authorized personnel and records attendance with high accuracy. Unauthorized persons are detected and alerts are generated. The attendance data is visualized weekly.

## Contributing
Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) for more details.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- **Project Guide**: Mrs. Laveena C Crasta
- **Internship Organization**: iHub IT Solutions, Mangalore
- **Principal**: Rev. Dr. Praveen Martis SJ
- **Director**: Rev. Fr. Melwyn Pinto SJ
- **Dean**: Prof Santhosh Rebello

---
