# Ionosphere Radar Target Classifier (v0 Full-Stack Edition)

A high-frequency phased-array radar return classifier built with **Next.js 16 (Turbopack)**, **React 19**, **TailwindCSS v4**, and **FastAPI**.

---

## 🎯 Architecture

* **Frontend**: Next.js 16 + React 19 + TailwindCSS v4 (pp/, components/, lib/)
  * Interactive 360-degree radar canvas with targets & sweeping beam
  * 2D PCA dataset projection explorer & feature variance inspector
  * 5-model benchmark suite (SVM, Random Forest, Neural Network, k-NN, Logistic Regression)
  * Viva Testing Lab (radar presets, 34-feature copy-paste box, batch CSV dropzone)
* **Backend**: FastAPI (ackend/main.py + ackend/ml.py)
  * Signal telemetry & real-time prediction dispatcher
  * Pre-trained 5-model pipeline artifact (rtifacts/bundle.joblib)
  * Dataset: UCI Ionosphere radar dataset (ackend/data/ionosphere.csv)

---

## 🚀 Running the Project

### 1. Start the FastAPI Backend (Port 8000)
Open a terminal in the ackend/ directory:
`ash
cd backend
python -m uvicorn main:app --port 8000
`
API docs available at: http://localhost:8000/docs

### 2. Start the Next.js Frontend (Port 3000)
In the project root directory:
`ash
npx pnpm dev
`
Open http://localhost:3000 in your browser.

---

## 📄 Codebase Documentation
All source code is consolidated in PROJECT_CODE.md for code review with Claude or examiners.
