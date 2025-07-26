# Game Automation using Mediapipe

Automate game interactions using your body movements and computer vision! This project leverages [Mediapipe](https://google.github.io/mediapipe/) for real-time pose detection and [PyAutoGUI](https://pyautogui.readthedocs.io/en/latest/) to control keyboard inputs, enabling you to play simple games hands-free using your webcam.

## Features
- **Real-time Pose Detection:** Uses Mediapipe to track your body pose from webcam video.
- **Game Control:** Move left, right, jump, crouch, or start the game using specific body poses and gestures.
- **Hands-Free Automation:** No need for physical controllers—just use your body!
- **Visual Feedback:** See your pose and detected actions overlaid on the webcam feed.

## How It Works
- **Start Game:** Join both hands in front of you to start.
- **Move Left/Right:** Move your body to the left or right of the camera frame.
- **Jump/Crouch:** Jump or crouch to trigger up/down actions.
- **In-Game Actions:** The script sends keyboard events (left, right, up, down, space) to control the game window.

## Requirements
- Python 3.7+
- Webcam
- Supported OS: macOS, Windows, Linux

### Python Dependencies
Install all dependencies with:
```bash
pip install -r requirements.txt
```

- `mediapipe`
- `pyautogui`
- `opencv-python`
- `numpy`

## Usage
1. **Connect your webcam.**
2. **Run the script:**
   ```bash
   python main.py
   ```
3. **Follow on-screen instructions:**
   - Join both hands to start the game.
   - Move left/right, jump, or crouch to control the game.
   - Press `Esc` or `q` to exit.

> **Note:** The script simulates keyboard presses. Make sure your game window is focused and supports keyboard controls.

## Customization
- You can adjust pose detection thresholds and key mappings in `main.py` to fit your needs or specific games.

## License
This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## Credits
- Developed by Jay Dobariya
- Powered by [Mediapipe](https://google.github.io/mediapipe/) and [PyAutoGUI](https://pyautogui.readthedocs.io/en/latest/)
