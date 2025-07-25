# 🧠 ResQ.AI – Backend (Flask + AI)

An intelligent, lightweight backend API service for **ResQ.AI**, the AI-powered emergency assistant. This component classifies incoming emergency reports and returns relevant metadata to guide the frontend's behavior.

> “Help will always be given at Hogwarts to those who ask for it.”  
> — *Albus Dumbledore*

---

## 🔗 Frontend Repository  
👉 [ResQ.AI Frontend](https://github.com/18Prachi/resq-ai)

---

## 💡 What It Does

This backend handles:

- 🧾 Accepting input from the user (text, and location optionally)
- 🧠 Using **HuggingFace Transformers** to classify emergencies  
  (`Medical`, `Fire`, `Accident`, `Crime`, etc.)
- 📊 Returning:
  - Emergency type
  - Confidence score
  - Location status
- ✨ Planned: Gemini / GPT integration for dynamic, real-time guidance

---

## ⚙️ Tech Stack

| Layer        | Technology                    |
|--------------|-------------------------------|
| Web Server   | Flask (Python)                |
| AI Model     | HuggingFace Transformers      |
| API Type     | REST (JSON)                   |
| CORS Support | `flask-cors`                  |
| Deployment   | Render.com / Python-compatible hosts |

---

## 🗂️ Project Structure

```bash
resq-ai-backend/
├── venv/                   # Virtual environment
├── app.py                  # Main API server
├── requirements.txt        # Python dependencies
├── package.json            # (Optional, for client bundling)
├── package-lock.json       # Lockfile
├── .gitignore              # Git exclusions
└── README.md               # You're here!
```

## 🚀 How to Run (Locally)

### 🧰 Prerequisites
- Python 3.8+
- `pip` installed

### 🛠️ Setup

```bash
# Clone the repo
git clone https://github.com/18Prachi/resq-ai-backend.git
cd resq-ai-backend

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # For Windows use: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the server
python app.py

```
🖥️ The API will be live at: `http://localhost:5000`

