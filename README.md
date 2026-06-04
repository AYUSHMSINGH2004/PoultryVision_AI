# 🐔 PoultryVision AI

An AI-powered poultry disease detection and analysis platform that helps farmers, veterinarians, and poultry researchers identify diseases from poultry images using computer vision and machine learning.

## 🚀 Live Demo

### Frontend
https://poultryvisionai.netlify.app

### Backend API
https://poultryvision-ai.onrender.com

---

## 📌 Features

- 🔍 Poultry disease detection from uploaded images
- 🤖 AI-powered disease analysis
- 📊 Disease confidence scores
- 📖 Poultry disease information library
- 🌐 Modern responsive user interface
- ⚡ Fast API-powered predictions
- ☁️ Cloud deployment with Netlify and Render

---

## 🛠️ Tech Stack

### Frontend
- React
- Vite
- React Router
- Tailwind CSS
- JavaScript

### Backend
- Python
- FastAPI
- Machine Learning / Deep Learning Models
- Uvicorn

### Deployment
- Netlify (Frontend)
- Render (Backend)

---

## 📂 Project Structure

```text
PoultryVision_AI/
│
├── poultry_frontend/
│   ├── apps/
│   │   └── web/
│   ├── src/
│   └── public/
│
├── backend/
│   ├── models/
│   ├── routes/
│   ├── services/
│   └── main.py
│
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/AYUSHMSINGH2004/PoultryVision_AI.git
cd PoultryVision_AI
```

---

## Frontend Setup

Navigate to frontend directory:

```bash
cd poultry_frontend
```

Install dependencies:

```bash
npm install
```

Create a `.env.local` file:

```env
VITE_API_BASE_URL=http://localhost:8000
VITE_BACKEND_URL=http://localhost:8000
```

Run development server:

```bash
npm run dev
```

---

## Backend Setup

Create virtual environment:

```bash
python -m venv venv
```

Activate virtual environment:

### Windows

```bash
venv\Scripts\activate
```

### Linux / Mac

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run backend server:

```bash
uvicorn main:app --reload
```

Backend will be available at:

```text
http://localhost:8000
```

---

## 🌍 Environment Variables

### Frontend

```env
VITE_API_BASE_URL=https://poultryvision-ai.onrender.com
VITE_BACKEND_URL=https://poultryvision-ai.onrender.com
```

---

## 🚀 Deployment

### Frontend (Netlify)

Build Settings:

```text
Base Directory: poultry_frontend
Build Command: npm run build
Publish Directory: dist/apps/web
```

Environment Variables:

```env
VITE_API_BASE_URL=https://poultryvision-ai.onrender.com
VITE_BACKEND_URL=https://poultryvision-ai.onrender.com
```

---

### Backend (Render)

Start Command:

```bash
uvicorn main:app --host 0.0.0.0 --port $PORT
```

---

## 📸 Screenshots

Add screenshots of:

- Home Page
- Disease Detection Page
- Prediction Results
- Poultry Information Page

---

## 🎯 Use Cases

- Poultry Farmers
- Veterinary Professionals
- Agricultural Researchers
- Poultry Farm Management Systems
- Educational Projects

---

## 🔮 Future Improvements

- Mobile application support
- Real-time disease monitoring
- Multi-language support
- Farm analytics dashboard
- Disease history tracking
- Offline prediction support

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a feature branch

```bash
git checkout -b feature-name
```

3. Commit changes

```bash
git commit -m "Added new feature"
```

4. Push branch

```bash
git push origin feature-name
```

5. Open a Pull Request

---

## 👨‍💻 Author

**Ayush M Singh**

GitHub:
https://github.com/AYUSHMSINGH2004

---

## 📄 License

This project is licensed under the MIT License.

---

⭐ If you found this project useful, consider giving it a star on GitHub.
