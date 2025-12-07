# 🔥 BlazeVeritas AI  
### AI-Powered Wildfire Detection & Explainability System

BlazeVeritas AI is a lightweight wildfire detection platform combining **deep learning**, **Grad-CAM explainability**, and a **RAG-based Copilot** for operational guidance. Built with **Streamlit + FastAPI**, it supports real-time image analysis and decision assistance.

---

## 🌍 Features
- 🔥 **Wildfire classification** (CNN, ResNet-18, DenseNet-121)  
- 🎯 **Explainability** with Grad-CAM heatmaps  
- 🌡 **Uncertainty calibration** (Temperature Scaling, ECE)  
- 🤖 **RAG Copilot** using LangChain + OpenAI  
- 🗺 **Geospatial-aware visualization**  
- ⚡ Fast, modular, deployment-ready architecture  

---

## ⚙️ Architecture
```

app/ (Streamlit UI)
├── Detect        → Fire prediction
├── Explain       → Grad-CAM
├── Calibration   → Reliability curves
└── Copilot       → RAG assistant

api/ (FastAPI)
├── inference.py  → Model prediction
├── explain.py    → Grad-CAM
└── rag/          → ChromaDB + OpenAI

````

---

## 🚀 Quick Start
```bash
git clone https://github.com/BlazeVeritas-AI/blazeveritas-project.git
cd blazeveritas-project

python -m venv .venv
source .venv/bin/activate      # macOS/Linux
.venv\Scripts\activate         # Windows

pip install -r requirements.txt

# Add to .env
OPENAI_API_KEY=your_api_key_here

uvicorn api.main:app --reload
streamlit run app.py
````

---

## 📁 Structure

```
blazeveritas/
├── api/         # Backend
├── app/         # Dashboard
├── models/      # Trained weights
├── scripts/     # Utilities
├── data/        # Sample inputs
└── reports/     # Metrics & Grad-CAM
```

---

## 👥 Project Team

* **Dilrabo Khidirova** — ML Development
* **Anna Surkova** — Deployment & QA

MSc in Software Engineering
**IT Park University**
Supported by **EPAM Engineering School**

---

## 📄 License

MIT License © 2025
**Dilrabo Khidirova & Anna Surkova**
