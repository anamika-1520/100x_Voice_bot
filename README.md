# voice-bot
# 🎙️ 100x Voice AI Bot

A full-stack **Voice-based AI Assistant** that converts speech to text, processes it using an LLM, and responds back with intelligent answers and audio output.

🚀 **Live Demo:**

* 🌐 Frontend: https://100xvoicebot-cbzchkx2dyfpbmvoanuxx9.streamlit.app/
* ⚙️ Backend API: https://voice-bot-using-groq-model-2.onrender.com/ask

---

## 🌟 Features

* 🎤 Voice Input (Audio Processing)
* 🧠 AI Response using Groq LLM
* 🔊 Text-to-Speech Output
* ⚡ Clean Streamlit UI
* 🌐 Fully deployed (Frontend + Backend separated)

---

## 🏗️ System Architecture

```
User (Streamlit UI)
        ↓
Frontend (Streamlit Cloud)
        ↓
Backend API (Render)
        ↓
Groq LLM (AI Response)
        ↓
Text-to-Speech
        ↓
Audio Response to User
```

---

## 📂 Project Structure

```
100x_Voice_bot/
│── backend/
│   ├── main.py        # API logic
│   ├── persona.py     # AI personality / prompt
│
│── frontend/
│   ├── app.py         # Streamlit UI
│   ├── reply.mp3      # Generated audio output
│   ├── runtime.txt    # Python version config
│
│── requirements.txt
│── README.md
```

---

## ⚙️ Tech Stack

| Layer      | Technology Used          |
| ---------- | ------------------------ |
| Frontend   | Streamlit                |
| Backend    | FastAPI / Python         |
| LLM        | Groq API                 |
| Speech     | Speech-to-Text + gTTS    |
| Deployment | Render + Streamlit Cloud |

---

## 🔗 API Endpoint

**POST** `/ask`

👉 https://voice-bot-using-groq-model-2.onrender.com/ask

### Request:

```json
{
  "text": "Your question here"
}
```

### Response:

```json
{
  "response": "AI generated answer"
}
```

---

## ▶️ Run Locally

### 1️⃣ Clone repo

```bash
git clone https://github.com/your-username/100x_Voice_bot.git
cd 100x_Voice_bot
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run Backend

```bash
cd backend
python main.py
```

### 4️⃣ Run Frontend

```bash
cd frontend
streamlit run app.py
```

---

## 🔑 Environment Variables

Create `.env` file:

```
GROQ_API_KEY=your_api_key
```

---

## 🚧 Challenges & Solutions

### ❌ Problem:

* WebRTC audio streaming failed on cloud (Render)

### ✅ Solution:

* Switched to **file-based audio processing**
* Separated frontend and backend for scalability

---

## 🚀 Future Improvements

* 🎯 Real-time voice streaming (WebRTC local support)
* 🧠 Conversation memory
* 🌍 Multi-language support
* 📱 Mobile optimization

---

## 📸 Screenshots

(Add your project screenshots here)

---

## 🤝 Contributing

Feel free to fork and improve this project!

---

## 👩‍💻 Author

**Anamika**

* GitHub: https://github.com/anamika-1520

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!

<img width="1920" height="1080" alt="Screenshot 2026-02-02 025935" src="https://github.com/user-attachments/assets/1dd85662-f1be-4576-bc8e-824004b28bbd" />
<img width="1920" height="1080" alt="Screenshot 2026-02-02 025946" src="https://github.com/user-attachments/assets/c0674ef9-6461-46e0-b310-46c7897cdb82" />


