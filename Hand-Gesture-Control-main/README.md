# Hand Gesture Control

A Python webcam-based gesture control app that uses MediaPipe and OpenCV to detect finger poses and automate browser actions.
This project uses your webcam to detect simple finger gestures and open browser tabs or close browser processes.

## Gesture Controls

- `1` finger → Open Claude AI
- `2` fingers → Open ChatGPT
- `3` fingers → Open Gemini
- `4` fingers → Open LinkedIn
- `Fist` → Close supported browsers

## Requirements

- Python 3.10 or newer
- Webcam
- Windows (browser closing uses PowerShell commands)

## Dependencies

Install the required packages:

```bash
pip install opencv-python mediapipe
```

## Usage

Run the script from the project directory:

```bash
python td_gestures.py
```

On first run, the script will download the MediaPipe hand landmarker model file `hand_landmarker.task` automatically.

## Notes

- The script opens browser tabs using the default browser.
- For the `Fist` gesture, the script attempts to close Chrome, Edge, Firefox, and Opera using PowerShell.
- Press `q` to quit the application window.

## Files

- `td_gestures.py` — main Python script for gesture detection and browser control
- `hand_landmarker.task` — MediaPipe hand detection model (downloaded automatically if missing)

## License

No license is specified. Use the project responsibly.
