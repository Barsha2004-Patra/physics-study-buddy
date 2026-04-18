# ⚛️ Physics Study Buddy

### Agentic AI Capstone Project (2026)

An intelligent **Physics chatbot** built using **Agentic AI architecture (LangGraph)** that helps B.Tech students understand core physics concepts, solve numerical problems, and interact through a conversational interface.

---

## 🚀 Project Overview

Physics Study Buddy is a **Retrieval-Augmented Generation (RAG) based AI system** that combines:

* 📚 Structured Physics knowledge base
* 🧠 Intelligent routing (Agent-based decision making)
* 🧮 Built-in calculator tool
* 🔍 Context-aware answering
* ✅ Faithfulness evaluation to reduce hallucinations

Unlike simple chatbots, this system **decides how to answer** — whether by retrieving knowledge, performing calculations, or using memory.

---

## 🧠 Key Features

### 🔀 Agentic Workflow (LangGraph)

* Smart routing between:

  * `retrieve` → concept-based questions
  * `tool` → numerical/calculation questions
  * `memory_only` → conversation & context

### 📖 Retrieval-Augmented Generation (RAG)

* Uses **ChromaDB vector database**
* Retrieves relevant physics concepts before answering

### 🧮 Built-in Physics Calculator

* Safely evaluates expressions like:

  * `F = ma`
  * Kinetic energy calculations
  * Basic math operations

### 📊 Faithfulness Evaluation Loop

* Automatically checks if answers are grounded in context
* Retries generation if hallucination is detected

### 💬 Streamlit Chat Interface

* Clean and interactive UI
* Maintains conversation history
* Shows sources + confidence score

---

## 📚 Topics Covered

* Newton’s Laws of Motion
* Work, Energy and Power
* Thermodynamics
* Electric Current & Ohm’s Law
* Capacitors and Capacitance
* Magnetism & Faraday’s Law
* Wave Motion and Sound
* Optics (Reflection & Refraction)
* Modern Physics (Photoelectric Effect)
* Gravitation & Kepler’s Laws

---

## 🏗️ Tech Stack

| Component  | Technology Used       |
| ---------- | --------------------- |
| LLM        | Groq (LLaMA 3)        |
| Framework  | LangGraph             |
| Vector DB  | ChromaDB              |
| Embeddings | Sentence Transformers |
| Frontend   | Streamlit             |
| Language   | Python                |

---

## 📂 Project Structure

```
.
├── agent.py                  # Core agent (LangGraph workflow)
├── capstone_streamlit.py     # Streamlit UI
├── day13_capstone.ipynb      # Development notebook
├── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/physics-study-buddy.git
cd physics-study-buddy
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Set API Key

Make sure you set your Groq API key:

```bash
export GROQ_API_KEY="your_api_key_here"
```

---

## ▶️ Run the Application

```bash
streamlit run capstone_streamlit.py
```

Then open the local URL shown in terminal.

---

## 🔄 How the System Works

1. User enters a question
2. Router decides the path:

   * Concept → Retrieval
   * Numerical → Calculator Tool
   * Casual → Memory
3. Relevant context is fetched from vector DB
4. LLM generates response
5. Evaluation checks answer quality
6. Final answer is displayed with sources

---

## 💡 Example Questions

* "Explain Newton's Second Law"
* "Calculate force if mass = 10kg and acceleration = 3 m/s²"
* "What is the first law of thermodynamics?"
* "What did I ask before?"

---

## 🎯 Learning Outcomes

This project demonstrates:

* Agentic AI system design
* RAG pipeline implementation
* Tool integration with LLMs
* Evaluation-driven generation
* Real-world AI application development

---

## 👨‍🏫 Instructor

**Dr. Kanthi Kiran Sirra**
Agentic AI Course — 2026

---

## 👨‍💻 Author

**Barsha Patra**

---

## 📌 Disclaimer

This project is developed as part of an academic capstone and is intended for educational purposes only.
