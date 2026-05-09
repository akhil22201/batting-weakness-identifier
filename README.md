# Batting Weakness Identifier for Amateur Cricketers

## Overview

The **Batting Weakness Identifier for Amateur Cricketers** is an AI-powered cricket batting analysis system developed using computer vision and deep learning techniques. The application analyzes batting videos to evaluate player posture, stance, balance, alignment, and shot execution. It provides automated performance scoring, visual overlays, and actionable coaching recommendations to help players improve their batting technique.

---

## Features

- Real-time cricket batting pose analysis
- MediaPipe-based 33-point body landmark detection
- Automated performance scoring system
- Detection of stance, balance, and alignment issues
- Annotated output videos with visual overlays
- AI-generated coaching recommendations
- Browser-based interactive interface

---

## Tech Stack

**Languages:** Python 3.12, HTML5, CSS3, JavaScript  

**Frameworks & Tools:** FastAPI, MediaPipe, OpenCV, YOLOv8, TensorFlow Lite  

**Concepts:** Computer Vision, Pose Estimation, Deep Learning, Video Analysis

---

## Installation

### Step 1: Clone the Repository

```bash
git clone https://github.com/akhil22201/batting-weakness-identifier.git
cd batting-weakness-identifier
```

---

### Step 2: Create Virtual Environment

```bash
python -m venv cricket-env
```

---

### Step 3: Activate Virtual Environment

#### Windows

```bash
cricket-env\Scripts\activate
```

#### Linux/Mac

```bash
source cricket-env/bin/activate
```

---

### Step 4: Install Dependencies

```bash
pip install -r requirements.txt
```

---

### Step 5: Download YOLO Model

The YOLOv8 nano model will automatically download during the first run.

---

## Running the Application

### Run using Python

```bash
python app.py
```

---

### Run using Uvicorn

```bash
uvicorn app:app --host 0.0.0.0 --port 8000 --reload
```

---

## Access the Application

- Web Interface: `http://localhost:8000`
- API Documentation: `http://localhost:8000/docs`
- Health Check Endpoint: `http://localhost:8000/health`

---

## Project Workflow

1. Video Upload  
2. Pose Detection  
3. Landmark Extraction  
4. Movement Analysis  
5. Performance Scoring  
6. Technique Recommendation Generation

---

## API Endpoints

- `POST /analyze` → Upload and analyze batting videos
- `GET /processed/{filename}` → Retrieve processed videos
- `GET /health` → Health check endpoint
- `GET /stats` → Analysis statistics

---

## Performance Optimization

- Frame skipping for faster processing
- GPU acceleration support for YOLO detection
- Browser-compatible H.264 video output

---

## Future Improvements

- Real-time live camera analysis
- Advanced shot classification
- Cloud deployment support
- Player performance history tracking

---

## Project Structure

```bash
batting-weakness-identifier/
│
├── backend/
├── frontend/
├── uploads/
├── processed/
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

---

## License

This project is licensed under the MIT License.

---

## Acknowledgements

- MediaPipe
- OpenCV
- Ultralytics YOLO
- FastAPI

---

## Author

Akhil
