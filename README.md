# FingerPaintCV – Draw with Your Finger in the Air 🎨

**FingerPaintCV** is an advanced AI-powered virtual painter that lets you draw on the screen using nothing but your finger, tracked in real-time through a webcam. Built using **OpenCV** and **MediaPipe**, it transforms your index finger into a brush and detects simple hand gestures to toggle drawing modes, adjust brush/eraser size, and switch colors — all without touching the screen.

---

## ✨ Features

* 🖐️ Hand tracking using MediaPipe
* 🖊️ Real-time drawing with your index finger
* ✊ Fist gesture to toggle brush/eraser size sliders
* 🎨 Dynamic color palette for easy selection
* 🧽 Eraser mode when black is selected
* 📏 Adjustable brush and eraser thickness using sliders
* 🖼️ On-screen UI for instructions and feedback
* 📎 Save and clear your canvas with keyboard shortcuts
* ⚡ Smoothing for gestures and drawing paths to reduce jitter
* 📊 Real-time FPS display

---

## 📷 Demo

*Coming soon*
You can add a `.gif` or video here showing live finger drawing and gesture control.

---

## 🛠️ Installation

1. **Clone the repository:**

```bash
git clone https://github.com/yourusername/FingerPaintCV.git
cd FingerPaintCV
```

2. **Install dependencies:**

Make sure you have Python 3.8+ installed, then run:

```bash
pip install -r requirements.txt
```

3. **Run the application:**

Make sure the script file is named `draw_with_finger.py`, then:

```bash
python3 draw_with_finger.py
```

---

## 📆 Requirements

Your `requirements.txt` should include:

```
opencv-python
mediapipe
numpy
```

No additional hardware or depth sensor is needed — just a webcam.

---

## 🎮 Controls

| Action                    | Input / Gesture        |
| ------------------------- | ---------------------- |
| Start Drawing             | Raise index finger     |
| Show Brush/Eraser Sliders | Make a Fist            |
| Select Color              | Hover over palette     |
| Adjust Thickness          | Move hand over sliders |
| Save Drawing              | Press `S` key          |
| Clear Canvas              | Press `C` key          |
| Quit Application          | Press `Q` key          |

---

## 🧠 How It Works

* **MediaPipe Hands** detects 21 hand landmarks in real-time.
* The app distinguishes between gestures like pointing (index up) and fist (all fingers closed).
* When pointing, drawing is enabled — when over the palette, the color is changed.
* A fist gesture activates brush and eraser sliders, controlled by hand position.
* All UI overlays, drawing logic, and gesture classification are handled in real-time with OpenCV.
* Gestures and positions are **smoothed** using weighted averages for better visual experience.

---

## 📄 License

This project is open-source and available under the **MIT License**. See the `LICENSE` file for details.

---

## 👨‍💻 Author

**Karim Dwikat**
AI & Computer Vision Developer
Built with ❤️ using Python, OpenCV, and MediaPipe.
