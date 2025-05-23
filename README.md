Face Mask Detection with Live Alert System
1. Objective
The main objective of this project is to develop a real-time face mask detection system using deep learning and computer vision techniques. The system can detect whether a person is wearing a face mask or not and trigger an alert if a mask is not detected.
2. Problem Statement
In the wake of global health concerns like the COVID-19 pandemic, wearing masks has become a critical preventive measure. Manual monitoring is labor-intensive and error-prone. This project aims to automate face mask detection to ensure compliance in public places such as schools, hospitals, malls, and offices.
3. Goals
•	Detect faces in real-time using a webcam or CCTV feed.
•	Classify each detected face as “Mask” or “No Mask”.
•	Trigger an audio/visual alert when a person is not wearing a mask.
•	Maintain accuracy, speed, and real-time processing.
•	Enable deployment on edge devices (Raspberry Pi, Jetson Nano).
4. Tools and Technologies Used
•	Python – Core programming language
•	TensorFlow/Keras – Deep learning model training
•	OpenCV – Image processing & real-time detection
•	MobileNetV2 – Pre-trained CNN for feature extraction
•	NumPy, Matplotlib – Data manipulation & visualization
•	Scikit-learn – Metrics and data splitting
•	Tkinter (optional) – GUI for user interface
•	Pygame / Playsound – For audio alerts
5. Dataset
•	Source: Public dataset from Kaggle: “Face Mask Detection”
•	Content: Images of people with/without masks
•	Preprocessing: Image resizing (224x224), Normalization, Data Augmentation
6. Model Architecture
•	Base Model: MobileNetV2 (pre-trained on ImageNet)
•	Custom Layers: GlobalAveragePooling2D, Dense(128), Dropout, Dense(2)
•	Compilation: categorical_crossentropy loss, Adam optimizer, accuracy metric
7. Model Training
•	Epochs: 20–30
•	Batch Size: 32
•	Validation Split: 20%
•	Accuracy Achieved: ~96–98%
8. Real-Time Face Mask Detection Workflow
•	1. OpenCV loads webcam feed
•	2. Detect face using Haar Cascade/DNN
•	3. Crop & resize face
•	4. Predict mask/no mask
•	5. Display result on screen
•	6. Trigger alert if no mask
9. Live Alert System
•	Visual: Red bounding box and label
•	Audio: Alert sound using playsound/pygame
•	Optional: Logging, GUI, and email alerts
10. Evaluation Metrics
•	Accuracy: >95%
•	Precision/Recall for each class
•	Confusion Matrix for performance overview
11. Deployment Options
•	Local System
•	Raspberry Pi (Edge)
•	Flask Web Application
•	Android (via TensorFlow Lite)
12. Future Enhancements
•	Face recognition for known violators
•	IR-based temperature checks
•	Dashboard for real-time monitoring
•	Classifying different mask types
•	Integration with YOLOv8 or Mediapipe
13. Conclusion
This project delivers a robust, real-time solution to monitor mask compliance using AI and computer vision. It’s deployable in real-world scenarios and helps promote public health and safety.
