

# 🧠 Agentic AI Chatbot — LangGraph + Groq + Streamlit

A simple and clean **Agentic AI Chatbot UI** built using **LangGraph**, **Groq**, and **Streamlit**.
The project demonstrates a basic chatbot workflow with a configurable UI, model selection, and a LangGraph-driven execution pipeline.

---

## 🚀 Features

* Built with **LangGraph StateGraph**
* Modular **BasicChatbotNode**
* Real-time streaming responses
* **Groq LLM** integration (llama-3.1, gemma models)
* Streamlit UI with:

  * LLM selector
  * Model selector
  * API key input
  * Use case selector
* Clean architecture, easy to extend into multi-agent systems

---

## 📦 Tech Stack

* Python 3.10+
* LangGraph
* Groq (ChatGroq)
* LangChain
* Streamlit

---

## 🏗️ Project Structure

```
src/langgraphagenticai/
│
├── graph/
│   └── graph_builder.py
│
├── nodes/
│   └── basic_chatbot_node.py
│
├── state/
│   └── state.py
│
├── LLMS/
│   └── groqllm.py
│
└── ui/streamlitui/
    ├── loadui.py
    └── display_result.py
```

---

## ⚙️ Installation

### 1. Clone the repo

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the app

```bash
streamlit run src/langgraphagenticai/main.py
```

---

## 🔑 Environment Variable (optional)

```
GROQ_API_KEY=your_api_key_here
```

(Or enter it directly in the Streamlit sidebar.)

---

## 💡 How It Works

* The app builds a LangGraph workflow:

```
START → chatbot → END
```

* `BasicChatbotNode` processes incoming messages using the selected Groq model
* LangGraph streams responses back
* Streamlit displays messages in a clean chat UI

---

## 📹 Demo

The video demo walks through:

* Sidebar controls
* Chat interface layout
* UI flow using a placeholder API key (intentionally)

---

## 🛠️ Future Enhancements

* Multi-agent workflows
* Memory node support
* Tool-calling
* Additional use-case templates

---

## 🤝 Contributions

Feel free to fork, improve, and submit pull requests.

---

## 🧑‍💻 Author

**Venkatesh Reddy**
AI Engineer & Full-Stack Developer

---

