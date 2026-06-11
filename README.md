# Hand Gesture Control

A Python-based real-time hand gesture recognition application that uses MediaPipe and OpenCV to detect finger gestures through a webcam and perform browser automation tasks.

The application tracks hand landmarks, identifies finger positions, and triggers predefined actions such as opening websites or closing browser windows.

## Features

- Real-time hand detection using MediaPipe
- Finger counting and gesture recognition
- Browser automation using hand gestures
- Automatic MediaPipe model download
- Lightweight and easy to use
- Webcam-based interaction without additional hardware

## Gesture Controls

| Gesture | Action |
|----------|----------|
| 1 Finger | Open Claude AI |
| 2 Fingers | Open ChatGPT |
| 3 Fingers | Open Gemini |
| 4 Fingers | Open LinkedIn |
| Fist | Close supported browsers |

## Technology Stack

- Python
- OpenCV
- MediaPipe
- WebBrowser Module
- PowerShell (Windows)

## Project Structure

```text
Hand-Gesture-Control/
│
├── td_gestures.py
├── hand_landmarker.task
└── README.md
```

### File Description

- `td_gestures.py` - Main application script responsible for gesture detection and browser automation.
- `hand_landmarker.task` - MediaPipe hand landmark model file downloaded automatically when required.
- `README.md` - Project documentation.

## Requirements

### Software Requirements

- Python 3.10 or later
- Windows Operating System (recommended)
- Internet connection for first-time model download

### Hardware Requirements

- Webcam

## Installation

### Clone the Repository

```bash
git clone https://github.com/kchaitralatha-bit/Hand-Gesture-Control.git
cd Hand-Gesture-Control
```

### Install Dependencies

```bash
pip install opencv-python mediapipe
```

## Usage

Run the application:

```bash
python td_gestures.py
```

### Steps

1. Launch the application.
2. Allow webcam access if prompted.
3. Show one of the supported hand gestures.
4. The corresponding browser action will be executed.
5. Press `q` to exit the application.

## How It Works

1. Captures video frames from the webcam.
2. Detects hand landmarks using MediaPipe.
3. Determines which fingers are raised.
4. Matches the detected gesture with predefined actions.
5. Executes browser automation commands.

## Supported Browser Actions

### Open Websites

- Claude AI
- ChatGPT
- Gemini
- LinkedIn

### Close Browsers

The fist gesture attempts to close:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Opera

## Automatic Model Download

If the MediaPipe model file is not available locally, the application automatically downloads:

```text
hand_landmarker.task
```

during startup.

## Notes

- Websites are opened using the system's default browser.
- Browser closing functionality uses PowerShell commands and is primarily designed for Windows.
- Good lighting conditions improve gesture detection accuracy.
- Ensure the webcam remains unobstructed and visible.

## Troubleshooting

### Webcam Not Detected

- Verify the webcam is connected properly.
- Close other applications currently using the camera.
- Check camera permissions.

### Gestures Not Recognized

- Improve lighting conditions.
- Keep your hand within the camera frame.
- Ensure fingers are clearly visible.

### Dependency Errors

Reinstall the required packages:

```bash
pip install --upgrade opencv-python mediapipe
```

## Future Enhancements

- Volume control using gestures
- Media playback control
- Custom gesture configuration
- Multi-hand gesture support
- Desktop GUI interface
- Cross-platform browser management

## Author

Chaitra Latha

GitHub Repository:
https://github.com/kchaitralatha-bit/Hand-Gesture-Control

## License
This project is intended for educational and learning purposes.
Feel free to use, modify, and enhance it for personal or academic projects.

This project is intended for educational and learning purposes.
Feel free to use, modify, and enhance it for personal or academic projects.
