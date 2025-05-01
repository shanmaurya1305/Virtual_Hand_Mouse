# 🖐️ Hand Gesture Controlled Cursor (Virtual Mouse)

This project is a **Hand Gesture Controlled Virtual Mouse** system developed using Python, OpenCV, and MediaPipe. It allows the user to control the mouse cursor and perform click actions using hand gestures captured from a webcam.

> ⚠️ **Project Status:** Functional prototype — includes cursor movement, left/right/double clicks, and screenshot gesture.

## 🎯 Objective

To create a contactless virtual mouse system that simulates cursor movement and mouse clicks based on hand gestures, helping enhance human-computer interaction in a touch-free manner.

---

## 🧠 How It Works

- Uses **MediaPipe** to detect hand landmarks in real-time.
- Tracks the **index finger** to move the cursor.
- Detects specific gestures (like thumb touching fingers or a fist) to perform:
  - ✅ Cursor movement  
  - ✅ Left Click (Thumb + Index Tip)
  - ✅ Right Click (Thumb + Middle Tip)
  - ✅ Double Click (Thumb + Pinky Tip)
  - ✅ Screenshot (Fist gesture)

---

## 🔧 Features

| Feature                          | Status     |
|----------------------------------|------------|
| Cursor control via finger        | ✅ Working |
| Left click (Thumb + Index)       | ✅ Working |
| Right click (Thumb + Middle)     | ✅ Working |
| Double click (Thumb + Pinky)     | ✅ Working |
| Screenshot (Fist gesture)        | ✅ Working |
| Gesture priority control         | ✅ Implemented |
| Multi-hand support               | ❌ Not supported yet (only 1 hand) |

---

## 🛠️ Tech Stack

| Tool/Library     | Purpose                            |
|------------------|-------------------------------------|
| Python           | Programming Language                |
| OpenCV           | Video capture & drawing             |
| MediaPipe        | Hand landmark detection             |
| PyAutoGUI        | Mouse control & screenshots         |
| Pynput           | Mouse click simulation              |
| NumPy            | Gesture angle calculation           |

---

## 🧪 Gesture Mapping

| Gesture Description       | Detected As      |
|---------------------------|------------------|
| Only Index Finger Up      | Cursor Movement  |
| Thumb touching Index Tip  | Left Click       |
| Thumb touching Middle Tip | Right Click      |
| Thumb touching Pinky Tip  | Double Click     |
| All fingers down (fist)   | Screenshot       |

---

## 📁 Project Structure

```
hand-gesture-cursor/
│
├── hand1_FINAL.py           # Main Python script
├── README.md                # Project documentation
└── requirements.txt         # Python dependencies (recommended)
```

---

## 🚀 Getting Started

### 🔄 Prerequisites

- Python 3.7+
- Webcam-enabled system

### 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/hand-gesture-cursor.git
   cd hand-gesture-cursor
   ```

2. **Install dependencies**
   ```bash
   pip install opencv-python mediapipe pyautogui pynput numpy
   ```

3. **Run the project**
   ```bash
   python hand1_FINAL.py
   ```

4. **Exit**
   - Press `q` to close the webcam window.

---

## 📌 Notes & Limitations

- Works best in good lighting conditions.
- Currently supports **only one hand** at a time.
- Cursor may be jumpy — future improvement can include smoothing/filtering.
- Screenshot files are saved as `my_screenshot_<random>.png`.

---

## 🛣️ Future Improvements

- Add multi-hand support  
- Gesture smoothing using historical position data  
- UI for calibration and customization  
- Add scroll or drag gestures  

---

## 🙌 Acknowledgements

- [MediaPipe by Google](https://mediapipe.dev/)
- [OpenCV Library](https://opencv.org/)
- [PyAutoGUI Documentation](https://pyautogui.readthedocs.io/)
