
# 🦖 Dino Game – Hand Gesture Controlled Automation

This project implements a gesture-controlled version of the Chrome **Dino Game**, where the player's movements are captured via webcam and translated into game controls using computer vision and automation libraries.

## 📹 How It Works

- Uses a webcam feed to detect hand gestures inside a defined region of interest (ROI).
- Processes video frames in real-time using OpenCV: converts to HSV, applies blurring and morphological operations, and extracts contours.
- Analyzes hand geometry to detect gestures (like the number of fingers shown).
- Sends keyboard commands (e.g., jump) to the game using PyAutoGUI based on recognized gestures.

## 📁 Files

- `dino_game.ipynb`: Main notebook containing the code and logic for gesture detection and game automation.

## 🛠️ Requirements

Install the dependencies with:

```bash
pip install opencv-python numpy pyautogui
```

You also need:

- A working webcam
- Google Chrome's Dino Game open (`chrome://dino` or just turn off Wi-Fi and hit space in Chrome)

## 🚀 Running the Project

1. **Clone the repo:**

```bash
git clone https://github.com/jithin06/dino_game.git
cd dino_game
```

2. **Launch the notebook:**

```bash
jupyter notebook dino_game.ipynb
```

3. **Follow the in-notebook instructions:**
   - A red rectangle appears on the screen — show hand gestures inside it.
   - Press `q` to quit the live video feed.

## ✨ Features

- Real-time gesture recognition using contour analysis
- Automation of keypresses using PyAutoGUI
- Clean ROI for hand tracking
- Thresholding and blurring to improve accuracy

