
# 🎓 AI Learning Buddy

AI Learning Buddy is a streamlined, web-based educational assistant built with Python. Powered by Google's Gemini generative AI model, this application provides an interactive interface for students and lifelong learners to break down complex topics, explore real-world scenarios, test their knowledge, or get quick answers to custom queries.

---

## 🚀 Features

The application offers four core learning activities tailored to any topic you input:

1. **Explain Concept:** Breaks down the input topic into simple, easy-to-understand language perfect for beginners.
2. **Real-Life Example:** Connects abstract concepts to daily life with a practical, simplified real-world scenario.
3. **Generate Quiz:** Automatically builds a custom quiz featuring 5 Multiple Choice Questions (MCQs) complete with answers.
4. **Ask Anything:** Serves as an open dialogue interface where the model responds directly to custom prompts or complex questions regarding the topic.

---

## 🛠️ Technology Stack

* **Frontend Framework:** [Streamlit](https://streamlit.io/) for creating a responsive, interactive UI.
* **LLM Engine:** [Google Generative AI SDK](https://github.com/google/generative-ai-python) utilizing the fast and capable `gemini-2.5-flash` model.
* **Development Environment:** Full devcontainer configuration optimized for GitHub Codespaces or Docker-based VS Code development.

---

## ⚙️ Setup & Installation

### Local Prerequisites
* Python 3.9 or higher installed on your system.
* A valid Google Gemini API Key.

### Step-by-Step Installation

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/manasvigit2415/ai-learning-buddy.git](https://github.com/manasvigit2415/ai-learning-buddy.git)
   cd ai-learning-buddy

```

2. **Install Dependencies:**
Install the required core packages using `pip`:
```bash
pip install -r requirements.txt

```


3. **Configure API Secrets:**
Streamlit looks for configuration secrets locally in a `.streamlit/secrets.toml` file. Create this file in your root folder:
```toml
# .streamlit/secrets.toml
GEMINI_API_KEY = "your_actual_gemini_api_key_here"

```


4. **Run the Application:**
```bash
streamlit run app.py

```


Open `http://localhost:8501` in your browser to start learning.

---

## 📦 Container Development (GitHub Codespaces / VS Code)

This repository includes a ready-to-use `.devcontainer` directory. If you open this project in a VS Code Dev Container or launch it on GitHub Codespaces:

* It automatically provisions a Python 3.11 pre-configured environment.
* Installs dependencies via `requirements.txt` instantly.
* Automatically runs and exposes the Streamlit web server on port 8501.

*(Note: You will still need to supply the `GEMINI_API_KEY` environmental variable or configuration secret inside the Codespace repository secrets settings to properly authenticate the AI model).*

---

## 📂 File Structure

```text
├── .devcontainer/
│   └── devcontainer.json   # Containerized workspace setup details
├── app.py                  # Core application logic and Streamlit UI
├── requirements.txt        # Third-party Python dependencies
└── README.md               # Documentation

```

```

```
