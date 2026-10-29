# Final project
# Emotion Detector

An AI-based web application that detects emotions (anger, disgust, fear, joy, sadness) in text using the Watson NLP library, served with Flask.

## Project structure

```
oaqjp-final-project-emb-ai/
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
├── static/
│   └── mywebscript.js
├── templates/
│   └── index.html
├── server.py
├── test_emotion_detection.py
├── requirements.txt
└── README.md
```

## Setup

```
pip install -r requirements.txt
```

## Run the application

```
python3.11 server.py
```

Then open the app on port 5000.

## Run unit tests

```
python3.11 test_emotion_detection.py
```

## Static code analysis

```
pylint server.py
```

## Output format

The `emotion_detector` function returns a dictionary with `anger`, `disgust`, `fear`, `joy`, `sadness` and `dominant_emotion`. For blank input (HTTP 400), all values are `None` and the web app shows "Invalid text! Please try again!".
