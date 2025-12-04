# 🚀 Local AI Chatbot — Chainlit + Ollama (llama3.2)

This project is a fully local AI chatbot built using **Chainlit** for the UI and **Ollama** for running the `llama3.2:latest` model.  
It provides a simple, fast, and private alternative to ChatGPT — all running on your own machine.

---

## ✨ Features

- 💬 **Interactive chat UI** powered by Chainlit  
- ⚡ **Streaming responses** for a smooth chat experience  
- 🔐 **100% local** — no API keys or cloud services  
- 🦙 Uses **Ollama** to run `llama3.2:latest` locally  
- 📚 Session-based message handling  
- 🎯 Very simple to run and extend

---

## 📁 Project Structure

.
├── app.py # Main application file
├── requirements.txt # Python dependencies
└── README.md # Project documentation

yaml
Copy code

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
cd YOUR_REPOSITORY_NAME
2️⃣ Create & activate a virtual environment (optional but recommended)
bash
Copy code
python -m venv venv
source venv/bin/activate      # Linux / macOS
venv\Scripts\activate         # Windows
3️⃣ Install dependencies
bash
Copy code
pip install -r requirements.txt
4️⃣ Install Ollama
Download from:
https://ollama.com/download

Then pull the required model:

bash
Copy code
ollama pull llama3.2:latest
▶️ Running the App
Start the Chainlit app using:

bash
Copy code
chainlit run app.py -w
Your local chatbot UI will now run at:

👉 http://localhost:8000

🧠 How It Works
When the chat starts, a greeting message is streamed character-by-character.

Messages are stored in a user_session list.

Each user message is sent to Ollama using the llama3.2:latest model.

Responses are streamed back to the UI.

Chainlit handles the interface and step execution.

🤝 Contributing
Feel free to open issues or submit pull requests to improve the app!

📜 License
This project is released under the MIT License.
