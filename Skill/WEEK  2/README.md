# Week 2 – Provider-Agnostic LLM Client

## 📌 Course Information
- **Course:** Generative AI
- **Experiment:** Week 2 – Provider-Agnostic LLM Client
- **Student:** Salihundam Svara Haasini

## 🎯 Objective

To develop a provider-agnostic Large Language Model (LLM) client that can interact with multiple LLM providers through a common interface.

This experiment explores abstraction, modular design, and integration of both hosted and locally running language models.

## 🛠️ Technologies & Tools
- **Python** – Programming language
- **Google Colab** – Development environment
- **Gemini API** – Hosted LLM provider
- **Ollama** – Running local language models
- **Llama 3.2** – Local language model
- **Object-Oriented Programming (OOP)** – Structuring the client using classes and abstraction

## 🧠 Concepts Explored

- Provider-agnostic architecture
- Abstract classes and methods
- Object-oriented programming
- API integration
- Local LLM execution
- Environment variable management
- Unit testing using a mock/fake provider

## ⚙️ Implementation

1. Set up the Google Colab environment.
2. Configured the Gemini API key securely using Colab Secrets.
3. Installed and configured Ollama to run locally within the Colab environment.
4. Pulled and executed the Llama 3.2 model using Ollama.
5. Created an abstract `LLMProvider` class to define a common interface.
6. Implemented `GeminiProvider` for hosted API-based interaction.
7. Implemented `Ollama
