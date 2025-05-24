# 👀 Blink Detection CAPTCHA System

A Python-based CAPTCHA refinement tool that distinguishes humans from bots using blink pattern detection.

## 🚀 Features

- Real-time blink detection using facial landmarks
- Dlib-based facial feature extraction
- Streamlit-powered interactive web interface
- Configurable blink threshold and count targets
- Time-limited verification session
- Visual feedback with live webcam feed

## 3. Computer Vision Foundations

### Facial Landmark Detection
The system uses Dlib's 68-point facial landmark model:

### Eye Aspect Ratio (EAR) Algorithm
The core blink detection uses:
```math
EAR = \frac{||p_2-p_6|| + ||p_3-p_5||}{2||p_1-p_4||}
