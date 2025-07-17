# Gesture-Controlled Virtual Mouse

A Python-based virtual mouse system that uses hand gestures detected via webcam to control mouse actions, system volume, and screen brightness. Built with OpenCV, MediaPipe, PyAutoGUI, and more.

## Features
- Move mouse pointer with hand gestures
- Left click, right click, double click, and drag
- Scroll vertically and horizontally
- Adjust system volume and screen brightness

## Setup Instructions
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Nolexx07/Gesture-control-virtual-mouse-.git
   cd Gesture-control-virtual-mouse-
   ```
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the application:**
   ```bash
   python src/Gesture_Controller.py
   ```

## Recognized Gestures
| Gesture Name         | How to Perform / Description         | Action in Code (Effect)                                  |
|----------------------|--------------------------------------|----------------------------------------------------------|
| **PALM**             | Open palm                            | No action (idle state)                                   |
| **FIST**             | All fingers curled                   | Mouse drag (hold left mouse button and move)             |
| **V_GEST**           | Index and middle finger up, spread   | Move mouse pointer (tracking mode)                       |
| **MID**              | Middle finger up                     | Single left click                                        |
| **INDEX**            | Index finger up                      | Right click                                              |
| **TWO_FINGER_CLOSED**| Index and middle finger up, close    | Double click                                             |
| **PINCH_MAJOR**      | Thumb and index finger pinch (major) | Adjust system brightness (horizontal) or volume (vertical)|
| **PINCH_MINOR**      | Thumb and index finger pinch (minor) | Scroll (vertical or horizontal)                          |

## Gesture Details
- **Move Mouse:** Show a "V" gesture (index and middle finger up, spread apart)
- **Left Click:** Show only the middle finger up
- **Right Click:** Show only the index finger up
- **Double Click:** Show index and middle finger up, close together
- **Drag:** Make a fist (all fingers curled)
- **Scroll:** Pinch with minor hand (thumb and index finger), move up/down or left/right
- **Adjust Volume/Brightness:** Pinch with major hand (thumb and index finger), move up/down (volume) or left/right (brightness)

## Requirements
- Python 3.7+
- Webcam
- Windows OS (for volume/brightness control)

## Dependencies
See `requirements.txt` for all Python dependencies.

## License
This project is licensed under the MIT License. 