# 🧠👀 Multilingual Eye-Tracking Communication System  
### AI-Powered Augmentative & Alternative Communication (AAC)

A low-cost, webcam-based **eye-tracking communication application** that enables individuals with severe motor disabilities to communicate using **eye and head movements**, enhanced with **predictive language models** and **multilingual support**.

---

## 🚀 Overview

Traditional input devices such as keyboards and mice are inaccessible to many individuals with motor impairments. This project introduces an **AI-driven Augmentative and Alternative Communication (AAC) system** that allows users to type using eye gaze and receive intelligent word suggestions in real time.

The system is designed to be:
- Non-invasive
- Affordable
- Language-inclusive
- Real-time and responsive

---

## ✨ Key Features

- 👁 **Webcam-Based Eye & Head Tracking**  
  Uses computer vision and CNNs without requiring specialized hardware.

- ⌨️ **Gaze-Controlled Virtual Keyboard**  
  Characters are selected using eye fixation and head orientation.

- 🤖 **Predictive Text & Language Modeling**  
  Context-aware word and sentence recommendations using LSTM and Transformer models.

- 🌍 **Multilingual Support**  
  Supports multiple languages and scripts using multilingual tokenizers such as mBERT and XLM-R.

- 🔊 **Text-to-Speech (TTS)**  
  Converts typed text into spoken output in the selected language.

- ⚡ **Real-Time Performance**  
  Optimized for low latency and smooth user interaction.

---

## 🏗️ System Architecture

1. Face and eye detection using webcam input  
2. Region of Interest (ROI) extraction  
3. CNN-based gaze estimation  
4. Temporal smoothing and context management  
5. Predictive language modeling  
6. Multilingual virtual keyboard UI  
7. Text-to-speech output  

---

## 🧠 Technologies Used

- **Language:** Python  
- **Computer Vision:** OpenCV  
- **Deep Learning:** CNN, LSTM, Transformer models  
- **NLP:** n-gram models, mBERT, XLM-R  
- **Eye Tracking:** Webcam-based gaze estimation  
- **UI:** Virtual keyboard with Unicode rendering  

---

## 📊 Evaluation Metrics

The system performance is evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- Typing speed
- Prediction accuracy

Experimental results demonstrate improved performance compared to traditional AAC systems.

---

## 🎯 Use Cases

- Assistive communication for individuals with motor disabilities
- Augmentative and Alternative Communication (AAC) research
- Inclusive human–computer interaction systems
- AI-based accessibility solutions


---

## 🛠️ Installation & Setup

bash
git clone https://github.com/your-username/eye-tracking-aac.git
cd eye-tracking-aac
pip install -r requirements.txt
python main.py
🔮 Future Enhancements

-Blink / wink-based selection confirmation
-Improved personalized prediction using adaptive learning
-Mobile and web deployment
-Advanced multilingual speech synthesis
-User studies for cognitive load evaluation

👨‍💻 Author

G. G. Naveen
B.Tech – Artificial Intelligence and Data Science
📜 License

This project is developed for academic and research purposes.
License details can be added as required.

