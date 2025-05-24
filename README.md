# 👀 Blink Detection CAPTCHA System

A Python-based CAPTCHA refinement tool that distinguishes humans from bots using blink pattern detection.

## 🚀 Features

- Real-time blink detection using facial landmarks
- Dlib-based facial feature extraction
- Streamlit-powered interactive web interface
- Configurable blink threshold and count targets
- Time-limited verification session
- Visual feedback with live webcam feed

## Computer Vision Foundations

### Facial Landmark Detection
The system uses Dlib's 68-point facial landmark model:
## Facial Landmark Indices (68-point model)
### 📌 Key Regions and Point Ranges

| Facial Region       | Landmark Points |
|---------------------|-----------------|
| **Jawline**         | 0 - 16          |
| **Right Eyebrow**   | 17 - 21         |
| **Left Eyebrow**    | 22 - 26         |
| **Nose**            | 27 - 35         |
| **Right Eye**       | 36 - 41         |
| **Left Eye**        | 42 - 47         |
| **Mouth**           | 48 - 67         |

### Eye Aspect Ratio (EAR) Algorithm
The core blink detection uses:
```math
EAR = \frac{||p_2-p_6|| + ||p_3-p_5||}{2||p_1-p_4||}
