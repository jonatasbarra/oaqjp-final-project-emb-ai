# Final project

## Emotion Detector

A web application built with Python and Flask that analyzes a text input and identifies the emotions expressed in it using IBM Watson NLP.

This project was developed as the final assignment for the **Developing AI Applications with Python and Flask** course by IBM on Coursera.

## Features

- Analyze natural language text using Watson NLP
- Detect five emotions:
  - Anger
  - Disgust
  - Fear
  - Joy
  - Sadness
- Identify the dominant emotion
- Display emotion scores through a Flask web interface
- Handle invalid or empty input
- Validate application behavior with unit tests
- Perform static code analysis using PyLint

## Technologies

- Python
- Flask
- IBM Watson NLP
- Requests
- unittest
- PyLint
- HTML
- JavaScript
- Git & GitHub

## Project Structure

```text
final_project/
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
├── static/
│   └── mywebscript.js
├── templates/
│   └── index.html
├── server.py
├── test_emotion_detection.py
└── README.md
```

## How It Works

The application receives text from the web interface and sends it to the Watson NLP Emotion Prediction API.

The API returns scores for five emotions:

- Anger
- Disgust
- Fear
- Joy
- Sadness

The application then determines which emotion has the highest score and returns it as the dominant emotion.

Example output:

```python
{
    "anger": 0.0043,
    "disgust": 0.0003,
    "fear": 0.0034,
    "joy": 0.9947,
    "sadness": 0.0127,
    "dominant_emotion": "joy"
}
```

## Running the Application

Install the required dependencies:

```bash
python3 -m pip install flask requests
```

Start the Flask server:

```bash
python3 server.py
```

The application runs on:

```text
http://localhost:5000
```

> Note: The Watson NLP endpoint used in this project is provided through the IBM Skills Network lab environment and may not be accessible outside that environment.

## Running the Tests

Run the unit tests with:

```bash
python3 test_emotion_detection.py
```

The test suite verifies that the application correctly identifies the dominant emotion for predefined statements representing joy, anger, disgust, sadness, and fear.

## Code Quality

Static code analysis was performed using PyLint:

```bash
pylint server.py
```

Final score:

```text
10.00/10
```

## What I Practiced

Through this project, I worked with:

- Python application development
- REST API integration
- JSON data processing
- Flask routing and web deployment
- Python package organization
- Unit testing
- Error handling
- Static code analysis
- Git and GitHub version control

## Author

**Jonatas Barra**

- GitHub: [jonatasbarra](https://github.com/jonatasbarra)
- LinkedIn: [Jonatas Barra](https://www.linkedin.com/in/jonatasbarra/)
