# 🧠 AI Research Intelligence Agent

An autonomous AI research assistant built with Python, Streamlit, Ollama, and web-search tools.

The system accepts a research topic, creates a structured research plan, performs web-based information gathering, and uses a locally hosted Large Language Model to generate research-oriented responses.

The project demonstrates how agentic AI concepts can be combined with local LLM inference and external tools to build an AI-powered research workflow.

---

## 🚀 Project Overview

The AI Research Intelligence Agent is designed to automate multiple stages of a research workflow.

Instead of simply generating an answer from a language model, the system follows an agent-based process:

- Understand the research query
- Break the query into actionable tasks
- Perform information retrieval
- Collect relevant research information
- Process the gathered information
- Generate a structured response

The system uses **Ollama** for local LLM inference, reducing dependency on paid external LLM APIs.

---

## 🧠 Agent Architecture

The application follows a modular agent-based architecture:

```text
                  User Research Query
                          |
                          v
                    Streamlit UI
                          |
                          v
                   Planner Agent
                          |
                          v
                  Research Plan
                          |
                          v
                  Executor Agent
                          |
              +-----------+-----------+
              |                       |
              v                       v
        Web Search Tool        PDF Downloader
              |                       |
              +-----------+-----------+
                          |
                          v
                   Research Agent
                          |
                          v
                    Ollama / Qwen
                          |
                          v
              Structured Research Response

This modular design separates planning, execution, information retrieval, and response generation.

🔥 Key Features
✅ Autonomous Research Planning

The Planner Agent analyzes the user's research question and decomposes it into smaller research tasks.

✅ Tool-Augmented Research

The Executor Agent can interact with external tools such as web search to retrieve information relevant to the research topic.

✅ Local LLM Inference

The system uses Ollama to run the language model locally instead of relying on paid external LLM APIs.

✅ Agent-Based Workflow

Different components are responsible for planning, research execution, and response generation, creating a modular agentic workflow.

✅ Interactive Web Interface

The application provides a Streamlit-based interface through which users can submit research queries and interact with the system.

✅ PDF Resource Support

The project includes functionality for downloading PDF resources when required during the research process.

✅ Conversation Memory

A modular conversation-memory component allows the system to maintain information from the interaction.

🛠️ Technology Stack
Programming
Python
Streamlit
AI / LLM
Ollama
Qwen3:4B
Local Large Language Model inference
Prompt Engineering
Agentic AI
Research & Tools
DDGS Web Search
Requests
PDF Downloader
Conversation Memory
Architecture
Multi-agent workflow
Task decomposition
Tool integration
Modular AI system design
🤖 Local LLM

The current implementation is configured to use:

qwen3:4b

through Ollama.

The model performs the language-generation and reasoning tasks required by the research workflow.

Using a local model provides:

No external LLM API dependency
Local inference
Greater control over model configuration
Reduced API usage costs

⚙️ Installation
1. Clone the Repository
git clone https://github.com/JeetMakadiya9/AI-Research-Agent.git
cd AI-Research-Agent
2. Create a Virtual Environment
python -m venv venv

Activate the environment on Windows:

venv\Scripts\activate

For Linux/macOS:

source venv/bin/activate
3. Install Dependencies

Install the required Python packages:

pip install streamlit ollama requests ddgs
🧠 Ollama Setup

Install Ollama on your system and make sure the Ollama service is running.

Pull the required model:

ollama pull qwen3:4b

Verify the installed model:

ollama list

The output should contain:

qwen3:4b
▶️ Running the Application


Open the address in your browser to interact with the research agent.

🧪 Example Research Queries

The system can be used for topics such as:

Impact of artificial intelligence on healthcare
Applications of generative AI in software engineering
Future of autonomous AI agents
Applications of AI in cybersecurity
Quantum computing applications in cryptography

The agent converts the research question into smaller tasks and performs the corresponding research workflow.

🔄 Research Workflow

The overall workflow is:

1. User Input

The user enters a research question through the Streamlit interface.

2. Planning

The Planner Agent analyzes the query and generates a structured research plan.

3. Task Execution

The Executor Agent processes the planned research tasks.

4. Information Retrieval

The system uses web-search tools to retrieve relevant information.

5. Resource Processing

Relevant resources, including PDF resources when required, can be collected for further processing.

6. Local LLM Processing

The collected research information is processed using the locally hosted Qwen3:4B model through Ollama.

7. Response Generation

The Research Agent generates a structured research-oriented response for the user.

👨‍💻 Author

Jeet Makadiya

M.Tech Computer Science & Engineering
Artificial Intelligence & Machine Learning

GitHub:

https://github.com/JeetMakadiya9
