# 🐔 PoultryVision AI
### Hierarchical Deep Learning & Grounded Generative AI for Poultry Disease Diagnosis

AI-powered veterinary web platform that detects poultry diseases from images and generates actionable, medically grounded consultation reports using Computer Vision, Explainable AI, and Generative AI.

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green)
![React](https://img.shields.io/badge/React-Frontend-61DAFB)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-FF6F00)
![Gemini](https://img.shields.io/badge/Gemini-2.5_Flash-purple)
![Netlify](https://img.shields.io/badge/Frontend-Netlify-success)
![Render](https://img.shields.io/badge/Backend-Render-blue)

---

## 🌐 Live Deployment

### Frontend
https://poultryvisionai.netlify.app

### Backend API
https://poultryvision-ai.onrender.com

---

## 📖 Executive Summary

PoultryVision AI is an end-to-end intelligent veterinary assistant designed to identify poultry diseases from images and provide grounded treatment recommendations.

Unlike traditional flat multi-class classification systems, PoultryVision AI employs a **Hierarchical CNN Architecture** that separates disease detection into two specialized stages:

1. **Bouncer Model**
   - Healthy vs Sick Triage
   - Optimized to reduce false negatives

2. **Doctor Model**
   - Disease-specific diagnosis
   - Bumblefoot
   - Chronic Respiratory Disease (CRD)
   - Fowl Pox
   - Infectious Coryza

The diagnostic results are then combined with Explainable AI visualizations and passed through a constrained Gemini-powered reasoning pipeline that generates structured veterinary consultation reports.

---

# 🚀 Features

### Computer Vision
- Poultry disease detection from images
- Hierarchical CNN architecture
- Binary triage + disease classification
- Confidence scoring

### Explainable AI
- Grad-CAM heatmaps
- Visual disease localization
- CNN decision transparency

### Generative AI
- Gemini 2.5 Flash integration
- Grounded generation framework
- Hallucination-reduced consultation reports
- Structured action plans

### Web Platform
- Responsive React frontend
- FastAPI backend
- REST API architecture
- Cloud deployment

---

# 🏗️ System Architecture

```text
Image Upload
      │
      ▼
┌─────────────────┐
│ Bouncer Model   │
│ Healthy / Sick  │
└─────────────────┘
      │
      ▼
┌─────────────────┐
│ Doctor Model    │
│ Disease Class   │
└─────────────────┘
      │
      ▼
┌─────────────────┐
│ Grad-CAM Engine │
└─────────────────┘
      │
      ▼
┌─────────────────┐
│ Gemini 2.5      │
│ Grounded AI     │
└─────────────────┘
      │
      ▼
Veterinary Consultation Report
```

---

# 🧹 Data Engineering Pipeline

The training dataset was constructed using:

- Original poultry disease datasets
- Roboflow-translated datasets
- Augmented image collections

### Data Cleaning

A custom TensorFlow-based silent cleaner was implemented to:

- Remove corrupt images
- Remove unreadable files
- Prevent training instability
- Improve gradient convergence

---

# 🧠 Hierarchical Deep Learning Models

## Phase 1 — Bouncer Model

Binary classification model responsible for determining:

```text
Healthy
or
Sick
```

### Objective

Reduce false negatives and ensure potentially sick birds are not ignored.

### Performance

| Metric | Score |
|----------|----------|
| Accuracy | 82% |
| Precision (Sick) | 90% |
| Recall (Sick) | 82% |
| F1 Score | 81% |

### Analysis

The Bouncer model demonstrates strong reliability for disease screening and prioritizes disease detection over risky healthy classifications.

---

## Phase 2 — Doctor Model

Multi-class disease classifier responsible for identifying:

- Bumblefoot
- Chronic Respiratory Disease (CRD)
- Fowl Pox
- Infectious Coryza

### Performance

| Metric | Score |
|----------|----------|
| Accuracy | 72% |

### CRD

| Metric | Score |
|----------|----------|
| Precision | 80% |
| Recall | 82% |
| F1 Score | 81% |

### Fowl Pox

| Metric | Score |
|----------|----------|
| Precision | 53% |
| Recall | 90% |

### Analysis

Confidence distributions cluster between 50% and 80%, indicating informed classifications rather than random or overconfident predictions.

---

# 🔍 Explainable AI

To improve trust and interpretability:

### Grad-CAM Heatmaps

The system generates visual explanations showing:

- Disease-specific regions
- Anatomical focus points
- CNN attention areas

This allows users to understand why a prediction was made.

---

# 🤖 Grounded AI Consultation Engine

After disease classification:

1. Model probabilities are extracted.
2. Grad-CAM explanations are generated.
3. Diagnostic information is passed to Gemini 2.5 Flash.
4. Gemini is constrained using veterinary dictionaries and structured prompts.

### Generated Output

- Diagnostic Summary
- Confidence Analysis
- Immediate Action Plan
- Isolation Recommendations
- Ongoing Care Guidance

This reduces hallucinations and ensures medically grounded responses.

---

# 💻 Technology Stack

## Frontend

- React
- Vite
- React Router
- Tailwind CSS

## Backend

- FastAPI
- Python
- TensorFlow
- Keras
- Gemini API

## AI & ML

- CNN Models
- Grad-CAM
- Explainable AI
- Grounded LLM Generation

## Deployment

- Netlify
- Render

---

# 📂 Project Structure

```text
PoultryVision_AI
│
├── poultry_frontend
│   ├── apps
│   │   └── web
│   ├── src
│   └── public
│
├── backend
│   ├── models
│   ├── routes
│   ├── services
│   └── main.py
│
└── README.md
```

---

# ⚙️ Local Development

## Clone Repository

```bash
git clone https://github.com/AYUSHMSINGH2004/PoultryVision_AI.git
cd PoultryVision_AI
```

## Frontend

```bash
cd poultry_frontend
npm install
npm run dev
```

## Backend

```bash
pip install -r requirements.txt
uvicorn main:app --reload
```

---

# 🌍 Deployment

## Netlify

```text
Base Directory:
poultry_frontend

Build Command:
npm run build

Publish Directory:
dist/apps/web
```

### Environment Variables

```env
VITE_API_BASE_URL=https://poultryvision-ai.onrender.com
VITE_BACKEND_URL=https://poultryvision-ai.onrender.com
```

---

# 📸 Screenshots

Add screenshots here:

- Home Page
- Disease Detection Interface
- Prediction Results
- Grad-CAM Visualization
- AI Consultation Report

---

# 🔮 Future Roadmap

- Mobile Application
- Real-Time Farm Monitoring
- Additional Disease Classes
- Disease History Tracking
- Multilingual Support
- Veterinary Dashboard
- Offline Inference Support

---

# 👥 Contributors

| Name | Registration Number | Role |
|--------|--------|--------|
| Ayush M Singh | 23BDS0033 | Project Lead, Full Stack Development, AI Integration |
| Venkata Sriram Topalli | 23BCE0441 | Contributor, Research, Testing & Development |

---

# ⭐ Support

If you found this project useful:

⭐ Star the repository

🍴 Fork the project

🤝 Contribute improvements

---

## 📜 License

This project is intended for educational, research, and academic purposes.
