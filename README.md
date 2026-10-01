# Gesture Music

A small webcam-controlled piano. The notebook uses MediaPipe to track one hand, OpenCV to display seven piano keys, and Pygame to play a note when your index fingertip enters a key.

## Requirements

- Python
- A webcam
- Speakers or headphones

## Setup

From the project directory, install the notebook's dependencies:

```powershell
python -m pip install opencv-python mediapipe pygame numpy
```

Keep the `sounds/` directory next to `project.ipynb`; it contains the WAV samples used by the notebook.

## Run

1. Open `project.ipynb` in VS Code or Jupyter and select a Python kernel with the dependencies installed.
2. Run the main piano code cell. Allow the application to access your webcam.
3. Move your index fingertip over one of the seven keys along the bottom of the camera window to play a note.
4. Press `q` while the camera window is focused to quit.

The notebook uses `cv2.CAP_DSHOW`, which is intended for Windows webcam capture.
