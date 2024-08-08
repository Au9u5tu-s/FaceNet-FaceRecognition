# Face Recognition and Attendance System

This project implements a deep learning-based face recognition and attendance system using TensorFlow and Flask. Developed as part of the MSc Big Data Analytics program at AIMIT, St. Aloysius College, Mangalore, the system enhances physical security and automates attendance recording.

## Table of Contents
1. [Introduction](#1-introduction)
2. [Survey of Technologies](#2-survey-of-technologies)
3. [Requirements and Analysis](#3-requirements-and-analysis)
4. [System Design](#4-system-design)
5. [Implementation and Testing](#5-implementation-and-testing)
6. [Results and Discussion](#6-results-and-discussion)
7. [Conclusion](#7-conclusion)
8. [References](#8-references)
9. [Glossary](#9-glossary)
10. [Installation](#installation)
11. [Usage](#usage)
12. [File Descriptions](#file-descriptions)
13. [Contributing](#contributing)
14. [License](#license)
15. [Acknowledgements](#acknowledgements)

---

## 1. Introduction

### 1.1 Background
The "Face Recognition and Attendance System" is designed to enhance security by identifying individuals and automatically recording their attendance. It employs the FaceNet model architecture within a TensorFlow environment to achieve high accuracy.

### 1.2 Objectives
- To develop a system that identifies employees and records attendance automatically.
- To ensure high accuracy in face recognition, even with changes like facial hair or glasses.
- To alert security staff in case of unauthorized access.

### 1.3 Purpose, Scope, and Applicability
**Purpose**: Document the software requirements and guide users on effective software usage.  
**Scope**: The system design includes major data structures, file formats, and modules.  
**Applicability**: The system is operated by Security Staff and Admin.

### 1.4 Achievements
The project introduced new technologies and concepts in deep learning, providing practical experience in neural networks using the TensorFlow environment.

---

## 2. Survey of Technologies

### 2.1 Deep Learning
Deep learning mimics human brain functions for data processing and pattern creation, essential for AI systems handling big data.

### 2.2 Computer Vision
Replicates human vision system capabilities in computers, enabling object identification in images and videos.

### 2.3 Face Detection
Detects faces in images, a crucial step for face recognition, and is influenced by various factors like pose, expression, and lighting.

### 2.4 Face Recognition
Uses techniques like geometric-based, appearance-based, and neural networks to identify faces.

### 2.5 Flask
A lightweight WSGI web application framework that allows quick and easy web application development.

### 2.6 Flutter
An open-source UI software development kit by Google, used for creating natively compiled applications for multiple platforms.

### 2.7 MongoDB
An open-source document database, leading in the NoSQL database category, known for its flexibility and scalability.

### 2.8 Perceptron
A neural network unit that processes input data to detect features or business intelligence.

### 2.9 Convolutional Neural Network (CNN)
A deep learning algorithm that processes input images, assigns importance to various aspects, and differentiates objects within the images.

### 3.0 TensorFlow
An open-source platform for machine learning, providing tools and libraries for building and deploying ML-powered applications.

### 3.1 Keras
An API designed for human beings, built on top of TensorFlow 2.0, known for its ease of use and scalability.

### 3.2 FaceNet
A face recognition system developed by Google, which produces high-quality face embeddings for face identification.

---

## 3. Requirements and Analysis

### 3.1 Problem Definition
Develop a smart surveillance system to recognize employees and ensure safety by detecting unauthorized users.

### 3.2 Requirement Specification
**Stable Internet Connection**: Required for data loading.  
**Software Quality Attributes**: Must ensure reliability and availability.

### 3.3 Planning and Scheduling
Detailed milestones and timelines for requirement specification, technology familiarization, database creation, system design, frontend implementation, and integration testing.

### 3.4 Software and Hardware Requirements
- **Hardware**: Minimum 8 GB RAM, Nvidia 1050 GTX GPU
- **Software**: Python, Flask, Dart, CUDA 9.0, TensorFlow-GPU, MongoDB

### 3.5 Preliminary Product Description
The system enhances physical security and improves attendance accuracy using deep learning.

### 3.6 Conceptual Models
Data Flow Diagrams (DFD) and schema designs for understanding data processing and storage.

---

## 4. System Design

### 4.1 Basic Modules
- **Face Recognition Module**: Identifies employees and retrieves their details.
- **Attendance Module**: Records attendance by recognizing faces.

### 4.2 Data Design
Schema design for employee, attendance, and visitor databases.

### 4.3 Procedural Design
Includes sequence diagrams, use case diagrams, activity diagrams, state chart diagrams, and class diagrams.

### 4.4 User Interface Design
Screens for login, face scan, face recognition, and attendance.

### 4.5 Security Issues
Emphasis on secure login information to prevent system compromise.

### 4.6 Test Case Design
Defines various software testing methods like unit testing, integration testing, and system testing.

---

## 5. Implementation and Testing

### 5.1 Implementation Approaches
Focuses on turning theoretical design into a working system with effective training for users.

### 5.2 Coding Details and Code Efficiency
Adherence to coding standards and efficiency checks using IDE tools.

### 5.3 Testing Approach
Includes unit testing, integration testing, user acceptance testing, performance testing, and load/stress testing.

### 5.4 Modifications and Improvements
Fixing identified bugs and incorporating customer feedback.

---

## 6. Results and Discussion

### 6.1 Test Reports
Details of successful tests for user login and face recognition.

### 6.2 User Documentation
The application is designed to be user-friendly, with straightforward navigation and operation.

---

## 7. Conclusion

### 7.1 Conclusion
The system provides an efficient way to manage physical security and automate attendance.

### 7.2 Limitations
Requires a stable internet connection and powerful hardware.

### 7.3 Future Scope
Potential to evolve into an IoT-based system for real-time person detection and identification.

---

## 8. References

Books and websites referenced for project development, including works on software engineering, neural networks, and machine learning.

---

## 9. Glossary

List of abbreviations and their descriptions used throughout the document.

---

## 10. Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/Au9u5tu-s/FaceNet-FaceRecognition.git
   cd FaceNet-FaceRecognition
   ```

2. Install the required packages:
   ```sh
   pip install -r requirements.txt
   ```

---

## 11. Usage
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

---

## 12. File Descriptions
- `classifier.py`: Script for classifying faces.
- `data_preprocess.py`: Script for preprocessing the dataset.
- `detect_face.py`: Script for detecting faces in images or videos.
- `train_main.py`: Main training script.
- `requirements.txt`: List of required packages.
- `README.md`: Project documentation.

---

## 13. Contributing
Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) for more details.

---

## 14. License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 15. Acknowledgements
Special thanks to Mrs. Laveena C Crasta, Ihub IT Solutions, and the faculty of AIMIT, St. Aloysius College, Mangalore, for their guidance and support throughout the project.

---
