# 🤖 Azure GPT-4o Chatbot

A modern web-based AI chatbot powered by **Azure OpenAI GPT-4o**. The backend is built with Flask (Python), and the frontend is a responsive HTML/CSS/JavaScript app.

---

## ✨ Features

- Conversational AI using Azure OpenAI GPT-4o
- Context-aware chat (remembers last 10 messages)
- Typing indicator and error handling
- Responsive, modern chat UI
- Easy configuration with `.env` file
- Health check and conversation reset endpoints

---

## 🚀 Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/Smiler54/ai-chatbot-gpt4o.git
cd ai-chatbot-gpt4o
```

### 2. Install dependencies
```bash
python3 -m venv venv
source venv/bin/activate
pip install flask flask-cors openai python-dotenv
```

### 3. Configure environment variables
Create a `.env` file in the project root:
```env
AZURE_OPENAI_API_KEY=your_actual_api_key
AZURE_OPENAI_ENDPOINT=https://your-resource-name.openai.azure.com/
AZURE_OPENAI_API_VERSION=2024-02-15-preview
DEPLOYMENT_NAME=gpt-4o
```

### 4. Start the backend
```bash
python app.py
```
The backend runs at `http://localhost:5000`.

### 5. Open the frontend
Open `index.html` in your browser. For best results, use a local server (e.g. VS Code Live Server extension).

---

## 🛠️ Project Structure

- `app.py` — Flask backend (API endpoints, Azure OpenAI integration)
- `index.html` — Frontend chat UI
- `.env` — Environment variables (not committed)

---

## ⚙️ Configuration

| Variable                  | Description                                 |
|--------------------------|---------------------------------------------|
| AZURE_OPENAI_API_KEY     | Your Azure OpenAI API key                   |
| AZURE_OPENAI_ENDPOINT    | Your Azure OpenAI resource endpoint         |
| AZURE_OPENAI_API_VERSION | API version (default: 2024-02-15-preview)   |
| DEPLOYMENT_NAME          | Your Azure OpenAI deployment name           |

---

## 📚 API Endpoints

- `POST /chat` — Send a message, get AI response
- `POST /clear` — Clear conversation history
- `GET /health` — Health check

---

## 🖼️ Screenshot

![Chatbot Output](screenshots/Output_Page.jpg)

---

## 👤 Authors & Credits

- Nandan Mishra
- Jyoti Kumari
- Juhi Kumari
- Prachi Singh

**Mentor:** Mr. Rohit Ranjan

---

## 📄 License

MIT License. See [LICENSE](LICENSE).
