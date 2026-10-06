# Final Project: Emotion Detection Web App

This repository contains the complete implementation of the Emotion Detection web application developed as part of the IBM Skills Network / Coursera course.

## Architecture

- **`EmotionDetection/`**: A Python package integrating Watson NLP Emotion Predict API.
  - `__init__.py`: Exposes `emotion_detector`.
  - `emotion_detection.py`: Core logic communicating with Watson NLP runtime with HTTP error handling (status code 400).
- **`server.py`**: A Flask server hosting the web application on port 5000, serving the web UI and `/emotionDetector` endpoint. Fully compliant with PEP8/pylint guidelines.
- **`test_emotion_detection.py`**: Unit tests verifying emotion classification for all basic emotions (joy, anger, disgust, sadness, fear).
- **`templates/index.html`**: User interface front-end.
- **`static/mywebscript.js`**: Client-side JavaScript handling asynchronous requests to the Flask server.

## Installation & Execution

```bash
pip install flask requests pylint
python server.py
```
