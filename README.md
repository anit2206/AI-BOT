A full-stack AI study assistant built with React (frontend) and Flask (backend), integrating GPT-4, speech-to-text, file upload, and email functionality.

---

## 🔹 Section 1: Frontend

### 🧱 Folder Structure

```
ai/
└── frontend/
    ├── public/
    └── src/
        ├── App.js
        ├── components/
        │   └── ChatBox.js
        ├── index.js
        └── App.css
```

### 🔄 Code Flow

```
📄 public/index.html
    ↓
📄 src/index.js
    → ReactDOM renders <App />

📄 src/App.js
    → Renders <ChatBox /> component
    → Imports global styles from App.css

📄 src/components/ChatBox.js
    → Handles:
        - User input
        - Speech-to-text (Web Speech API)
        - File upload (PDF)
        - GPT-4 API call via POST to `/ask`
        - Text-to-speech for responses
        - Email POST to `/send-email`
```

## 🔹 Section 2: Backend

### 🧱 Folder Structure

```
ai/
├── backend/
│   ├── app.py
│   ├── requirements.txt
│   └── .env
└── frontend/
    ├── public/
    └── src/
        ├── App.js
        ├── components/
        │   └── ChatBox.js
        ├── index.js
        └── App.css
```



## 🔁 Final Flow Overview

```
index.html
   ↓
index.js
   ↓
App.js
   ↓
ChatBox.js
   ↓
→ POST /ask → app.py → GPT-4 → Response
→ POST /send-email → app.py → SMTP → Email sent
```

---

## 📌 Notes

- Ensure environment variables are securely stored in `.env`
- You need an OpenAI API key and SMTP credentials for full functionality
- CORS is enabled to allow frontend-backend communication locally

---

Feel free to customize, fork, and improve!

---

