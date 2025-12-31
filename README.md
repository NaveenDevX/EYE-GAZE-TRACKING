# 🧠👀 Multilingual Eye-Tracking Communication System

### AI-Powered Augmentative & Alternative Communication (AAC)

An affordable, webcam-based **eye-tracking communication application** designed for individuals with severe motor disabilities (such as ALS, MND, or Spinal Cord Injuries). This system enables seamless communication through **eye and head movements**, powered by **predictive language models** and robust **multilingual support**.

---

## 🚀 Overview

Traditional input devices like keyboards and mice are often inaccessible to individuals with motor impairments. This project introduces an **AI-driven AAC system** that allows users to type using eye gaze and receive intelligent, real-time word suggestions.

### Core Philosophy:
* **Non-invasive:** No specialized hardware—just a standard laptop webcam.
* **Affordable:** Low-cost implementation for wider accessibility.
* **Language-inclusive:** Designed for a global audience with multilingual scripts (English, Hindi, Tamil, etc.).
* **Real-time:** Optimized for low latency and fluid interaction.

---

## ✨ Key Features

* 👁 **Webcam-Based Tracking:** Uses Dlib and OpenCV for CNN-based gaze estimation.
* ⌨️ **Gaze-Controlled Keyboard:** Character selection via fixation duration (dwell time) and head orientation.
* 🤖 **Predictive Text:** Context-aware word/sentence recommendations using **LSTM** and **Transformers**.
* 🌍 **Multilingual Support:** Integration of **mBERT** and **XLM-R** for diverse script support.
* 🔊 **Text-to-Speech (TTS):** Instant vocalization of typed text using `gTTS` or `pyttsx3`.
* ⚡ **High Performance:** Optimized pipeline for smooth, real-time user experience at 30+ FPS.

---

## 🏗️ System Architecture

1.  **Input Module:** Captures video stream and detects facial landmarks (68-point predictor).
2.  **Tracking Engine:** Extracts the eye Region of Interest (ROI) and calculates the Gaze Ratio.
3.  **Smoothing Layer:** Applies temporal filters to prevent "jitter" in gaze movement.
4.  **Interaction Layer:** A virtual keyboard UI where keys light up based on gaze coordinates.
5.  **NLP Engine:** Takes current input and suggests the next 3 most likely words.
6.  **Output Module:** Converts the final string into a natural-sounding voice.

---

## 🧠 Technologies Used

| Category | Tools & Frameworks |
| :--- | :--- |
| **Language** | Python 3.8+ |
| **Computer Vision** | OpenCV, Dlib, Mediapipe |
| **Deep Learning** | TensorFlow / PyTorch |
| **NLP** | HuggingFace (mBERT, XLM-R), NLTK |
| **UI/UX** | Tkinter / PyQt5 |
| **Audio** | gTTS (Google Text-to-Speech) |

---



## 📂 Dataset Pipeline
The system utilizes a hybrid approach, combining custom datasets with public corpora for maximum accuracy.

🔹 Eye & Gaze Tracking Data
Data points: Annotated gaze directions (Left, Right, Up, Down, Center).

Head Pose: Yaw, Pitch, and Roll angles extracted for hybrid control.

Source: Custom recorded frames and the MPIIGaze dataset.

🔹 Language Modeling Data
Supports multiple languages and scripts using mBERT tokenizers.

Languages: English, Tamil, Hindi, and growing.

## 📊 Evaluation Metrics
The system is rigorously tested against the following benchmarks:

Gaze Accuracy: Measured by angular error (degrees).

Typing Speed: Characters Per Minute (CPM) / Words Per Minute (WPM).

KSR (Keystroke Saving Rate): Efficiency gained through AI word predictions.

Latencies: Inference time per frame (target < 30ms).

## 🛠️ Installation & Setup
1. Prerequisites
Ensure you have Python installed. It is recommended to use a virtual environment.

Bash

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
2. Install Dependencies
Bash

pip install opencv-python dlib numpy tensorflow torch transformers gTTS
Note: If installing dlib fails, ensure you have CMake and Visual Studio C++ build tools installed.

3. Download Shape Predictor
Download the shape_predictor_68_face_landmarks.dat file and place it in the models/ folder.

4. Run the Application
Bash

python main.py
## 🎮 Usage Instructions
Calibration: Follow the on-screen dot with your eyes to calibrate the webcam to your environment.

Typing: Focus on a letter for 2 seconds (Dwell time) to select it.

Head Movement: Use slight head tilts to navigate between keyboard sections.

Prediction: Click on the top-bar suggestions to complete words instantly.

Speak: Look at the "Speak" button to convert text to audio.

## 🔮 Future Enhancements
Gesture Shortcuts: Use eye blinks or winks for "Space" or "Delete" functions.

Adaptive Learning: The AI learns your specific vocabulary and frequently used phrases over time.

Mobile Deployment: Lightweight version for tablets using Mediapipe Iris.

Cloud Sync: Save user profiles and custom dictionaries across devices.

## 👨‍💻 Author
G. G. Naveen B.Tech – Artificial Intelligence and Data Science

## 📜 License
This project is licensed under the MIT License - see the LICENSE file for details. Developed for academic and research purposes to enhance human accessibility.
