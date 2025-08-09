# 🦙 LLaMA Text Summarizer

A simple AI-powered web application that summarizes text using the **LLaMA** model (via [Ollama](https://ollama.com)), with a **FastAPI** backend and **Streamlit** frontend.  

---

## ✨ Features
- ⚡ **FastAPI Backend** – Handles text summarization requests and communicates with the LLaMA model.  
- 🎨 **Streamlit Frontend** – User-friendly web interface for entering text and viewing summaries.  
- 💻 **Runs Locally** – Uses Ollama to host the LLaMA model on your machine.  
- 🔗 **Git & GitHub** – Version control and project collaboration ready.  

---

## 📂 Project Structure
```
text-summarizer-llama/
│
├── backend/
│   └── main.py           # FastAPI backend
│
├── frontend/
│   └── app.py            # Streamlit frontend
│
├── venv/                 # Virtual environment (excluded in .gitignore)
├── requirements.txt      # Python dependencies
└── README.md             # Documentation
```

---

## 🚀 Installation & Setup

### **1. Install Python**
- Download & install Python from [python.org/downloads](https://www.python.org/downloads/).
- Ensure you check **"Add Python to PATH"** during installation.

### **2. Clone the Repository**
```bash
git clone https://github.com/iamdevlab/llama-text-summarizer.git
cd llama-text-summarizer
```

### **3. Create & Activate Virtual Environment**
**Windows (PowerShell)**:
```powershell
python -m venv venv
venv\Scripts\Activate.ps1
```
**Mac/Linux**:
```bash
python3 -m venv venv
source venv/bin/activate
```

### **4. Install Dependencies**
```bash
pip install -r requirements.txt
```

### **5. Install Ollama & LLaMA Model**
- Download Ollama from [ollama.com/download](https://ollama.com/download).  
- Pull the LLaMA model:
```bash
ollama pull llama2
```

---

## ▶️ Running the App

### **Run Backend (FastAPI)**
```bash
uvicorn backend.main:app --reload
```
Backend runs at: **http://localhost:8000**

### **Run Frontend (Streamlit)**
In a new terminal:
```bash
streamlit run frontend/app.py
```
Frontend runs at: **http://localhost:8501**

---

## 📊 Workflow Diagram
![Workflow Diagram](docs/workflow.png)  
*(User → Streamlit → FastAPI → Ollama (LLaMA) → Summary Output)*

---

## 🛠 Tech Stack
- **[Python](https://www.python.org/)** – Programming language
- **[FastAPI](https://fastapi.tiangolo.com/)** – Backend API
- **[Streamlit](https://streamlit.io/)** – Frontend UI
- **[Ollama](https://ollama.com/)** – Local LLaMA model hosting
- **[Git & GitHub](https://github.com/)** – Version control

---

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 💡 Author
Developed by **[Vernon Usigbe](https://github.com/iamdevlab)**.  
If you find this useful, ⭐ the repo and share it!
