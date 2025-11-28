Real-Time Face Recognition using OpenCV

A real-time face detection and recognition system built using Python, OpenCV, and the LBPH Face Recognizer. This project captures face data, trains a recognition model, and performs live recognition using a webcam.

<div align="center">








</div>

## 🚀 Features
- Real-time face detection using Haar Cascade Classifiers  
- Face recognition using LBPH (Local Binary Patterns Histogram)  
- Data collection system for capturing face images  
- Model training module that generates classifier.yml  
- Lightweight, fast, and works on any webcam  
- Easy to extend for multiple users  



📂 Project Structure

## Face-Recognition-Project/
│
├── data/                 # Stores captured face images
├── classifier.yml        # Generated trained model (after Step 2)
├── Data_Generator.py     # Capture face images using webcam
├── Classifier.py         # Train LBPH model
├── Recognize.py          # Real-time recognition script
├── haarcascade_frontalface_default.xml
└── README.md

🛠️ Requirements
Install the required Python libraries:
```
pip install opencv-contrib-python numpy pillow

```
🧪 How to Run

Follow these steps in order:

Step 1: Generate Face Data
  .	Open Data_Generator.py
  .	Set a unique user_id for each person
  .	Run the script to capture 100 face images using your webcam

```
python Data_Generator.py

```
Step 2: Train the Model
Train the classifier using LBPH algorithm:

```
python Classifier.py

```
A new file called classifier.yml will be created — this is your trained model.

Step 3: Recognize Faces (Real-Time)
Run the recognition script:

```
python Recognize.py

```
Your webcam will open, and recognized faces will be labeled in real time.

📘 File Descriptions


•	Data_Generator.py: Captures and saves face images from a webcam for training.
•	Classifier.py: Trains the face recognizer on the saved images and creates classifier.yml.
•	Recognize.py: Uses the webcam and the trained classifier.yml to perform real-time face recognition.
•	haarcascade_*.xml: Pre-trained models from OpenCV used for detecting objects like faces and eyes.






