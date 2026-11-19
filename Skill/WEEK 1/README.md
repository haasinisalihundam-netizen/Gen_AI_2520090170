# Week 1 – First LLM API Call Using OpenAI

## 📌 Course Information
- **Course:** Generative AI
- **Experiment:** Week 1 – First LLM API Call Using OpenAI
- **Student:** Salihundam Svara Haasini

## 🎯 Objective
To understand how to interact with a Large Language Model (LLM) programmatically by making the first API call using Python and the OpenAI API.

This experiment introduces the fundamentals of API integration, environment configuration, and secure API key management.

## 🛠️ Technologies & Tools
- **Python** – Programming language
- **OpenAI API** – Accessing Large Language Models
- **Visual Studio Code** – Development environment
- **python-dotenv** – Managing environment variables
- **Virtual Environment (venv)** – Managing project dependencies

## 📂 Project Structure

```text
Week-1/
│
├── main.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

## ⚙️ Implementation

1. Set up a Python development environment using a virtual environment.
2. Installed the required Python libraries.
3. Configured the OpenAI API key using a `.env` file.
4. Used `python-dotenv` to securely load environment variables.
5. Implemented a Python program to send a request to the OpenAI API.
6. Retrieved and displayed the LLM-generated response.

## ▶️ How to Run

**1. Clone the repository**
```bash
git clone <your-repository-url>
```

**2. Navigate to the Week 1 folder**
```bash
cd Week-1
```

**3. Install dependencies**
```bash
pip install -r requirements.txt
```

**4. Configure your API key**

Create a `.env` file in the project directory:

```env
OPENAI_API_KEY=your_api_key_here
```

**5. Run the program**
```bash
python main.py
```

## 🔐 Security
- API keys are stored in environment variables instead of being hardcoded.
- The `.env` file is excluded from version control using `.gitignore`.
- Sensitive credentials should never be uploaded to a public GitHub repository.

## 📚 Key Learnings
- Understanding the basics of Large Language Models.
- Learning how API requests and responses work.
- Connecting Python applications with an LLM.
- Managing API keys securely using environment variables.
- Setting up and working with Python virtual environments.

## 🚀 Outcome
Successfully configured a Python environment and executed the first LLM API call using the OpenAI API, gaining practical experience with Python-based LLM integration.

---

**Part of my Generative AI coursework – exploring LLMs, API integration, and practical AI development.**
