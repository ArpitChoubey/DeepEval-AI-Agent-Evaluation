# 🚀 DeepEval Agentic Testing Framework | LangChain • Claude • GPT-4o • DeepEval • AI Agent Evaluation

<p align="center">

![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![DeepEval](https://img.shields.io/badge/DeepEval-Agent%20Evaluation-blueviolet?style=for-the-badge)
![LangChain](https://img.shields.io/badge/LangChain-Agent-green?style=for-the-badge)
![Claude](https://img.shields.io/badge/Claude-AI-orange?style=for-the-badge)
![OpenAI](https://img.shields.io/badge/GPT--4o-Judge-black?style=for-the-badge&logo=openai)
![LLM Testing](https://img.shields.io/badge/LLM-Testing-red?style=for-the-badge)
![GenAI](https://img.shields.io/badge/Generative-AI-success?style=for-the-badge)
![AI Quality](https://img.shields.io/badge/AI-Quality-blue?style=for-the-badge)
![Agentic AI](https://img.shields.io/badge/Agentic-AI-purple?style=for-the-badge)
![Observability](https://img.shields.io/badge/LLM-Observability-teal?style=for-the-badge)
![QA Automation](https://img.shields.io/badge/QA-Automation-success?style=for-the-badge)
![GitHub](https://img.shields.io/badge/Open%20Source-GitHub-black?style=for-the-badge&logo=github)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

</p>

---

# 🌟 Project Overview

As AI Agents become increasingly common in enterprise software, traditional software testing is no longer sufficient.

This repository demonstrates **how to evaluate an AI Agent using DeepEval's Component-Level Evaluation**, measuring whether an agent:

- ✅ Completes the user's task
- ✅ Uses the correct tools
- ✅ Produces reliable responses
- ✅ Can be observed and evaluated like production AI systems

Unlike traditional unit testing, this project focuses on **LLM Quality Engineering**, an emerging discipline that combines AI, automation testing, observability, and evaluation.

---

# 🎯 Why This Project Matters

Modern companies are rapidly adopting:

- Agentic AI
- LangChain
- OpenAI
- Claude
- MCP Servers
- RAG Applications
- AI Assistants

Building AI applications is only half the challenge.

**The bigger challenge is knowing whether they actually work correctly.**

This repository demonstrates practical techniques for evaluating AI agents using production-style metrics instead of manual inspection.

---

# 🚀 Key Highlights

✔ DeepEval Component-Level Evaluation

✔ LangChain Agent Testing

✔ Claude as the Agent

✔ GPT-4o as the Judge

✔ Task Completion Metric

✔ Tool Correctness Metric

✔ Cross-Vendor AI Evaluation

✔ AI Agent Observability

✔ Golden Dataset Testing

✔ Trace Collection

✔ Component-Level AI Testing

✔ Real-world QA workflow

✔ Minimal Instrumentation (Only 4 additional lines)

---

# 🧠 Architecture

```
                    User Prompt
                          │
                          ▼
               LangChain AI Agent
                          │
                Claude (LLM Agent)
                          │
         -----------------------------
        │                             │
        ▼                             ▼

   Tool Execution               Final Response

        │                             │
         -------- Trace Collection ----

                    ▼

          DeepEval Callback Handler

                    ▼

        Task Completion Evaluation

                    +

        Tool Correctness Evaluation

                    ▼

             GPT-4o Judge Model

                    ▼

        Scores • Reasons • Evaluation
```

---

# 🔥 Why Recruiters & Hiring Managers Should Care

This project demonstrates experience beyond traditional automation testing.

It showcases knowledge of:

- AI Testing
- LLM Evaluation
- GenAI Quality Engineering
- AI Observability
- Agentic Systems
- LangChain
- Prompt Evaluation
- Cross-model validation
- Modern QA Engineering

These are rapidly growing skillsets for:

- Lead SDET
- AI Test Engineer
- AI QA Engineer
- GenAI Quality Engineer
- AI Automation Engineer
- LLM Evaluation Engineer

---

# 📂 Project Structure

```
deepeval-agent-project
│
├── agent_plain.py
├── agent_instrumented.py
├── chatbot.py
├── rag_agent.py
├── mcp_server.py
├── policies.txt
├── requirements.txt
├── README.md
│
├── evals
│   ├── test_TaskCompletion.py
│   ├── test_TracingComponentsTest.py
│   ├── test_agent_synthesized.py
│   ├── test_chatbot.py
│   ├── test_chatbot_customreqd.py
│   ├── test_customMetricEvals.py
│   ├── test_multipleEvalsTest.py
│   └── test_rag_agent.py
│
└── CLAUDE.md
```

---

# ⚙ Agent Flow

```
User Query

      │

      ▼

LangChain Agent

      │

Claude LLM

      │

Tool Execution

      │

DeepEval Callback

      │

Trace Collection

      │

Task Completion

      │

Tool Correctness

      │

GPT-4o Evaluation

      │

Final Scores
```

---

# 🔍 Minimal Instrumentation

One of the biggest strengths of DeepEval is that developers only need **4 additional lines** to make an existing LangChain agent observable.

```python
from deepeval.integrations.langchain import CallbackHandler

deepeval_callback = CallbackHandler()

config={"callbacks":[deepeval_callback]}

@observe(name="support_agent")
```

Everything else in the agent remains unchanged.

This makes AI evaluation practical for existing production systems.

---

# 🧪 Evaluation Metrics

## ✅ Task Completion

Measures whether the AI successfully completed the user's objective.

Example questions:

- Did the agent solve the task?
- Did it answer correctly?
- Was the reasoning complete?

---

## ✅ Tool Correctness

Measures whether the AI selected the appropriate tools.

Example questions:

- Did it call the right tool?
- Was the correct sequence followed?
- Were unnecessary tool calls avoided?

---

# 🏆 Features

- AI Agent Testing
- LangChain Integration
- DeepEval Evaluation
- Cross-Vendor LLM Testing
- GPT-4o Judge
- Claude Agent
- Golden Dataset Evaluation
- Trace Collection
- Component-Level Evaluation
- Custom Metrics
- Multiple Evaluations
- RAG Testing
- Chatbot Evaluation
- AI Observability
- Production-style AI QA

---

# 📚 Technologies Used

| Category | Technology |
|----------|------------|
| Language | Python |
| Agent Framework | LangChain |
| Evaluation | DeepEval |
| AI Model | Claude |
| Judge Model | GPT-4o |
| AI Platform | OpenAI |
| Testing | DeepEval Metrics |
| AI Quality | Task Completion |
| Tool Evaluation | Tool Correctness |
| Observability | CallbackHandler |

---

# 🚀 Installation

Clone repository

```bash
git clone https://github.com/ArpitChoubey/deepeval-agent-project.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Configure API Keys

```bash
export ANTHROPIC_API_KEY=YOUR_KEY

export OPENAI_API_KEY=YOUR_KEY
```

---

# 🔥 Login to DeepEval

```bash
deepeval login
```

---

# ▶ Run Agent

```bash
python agent_instrumented.py
```

---

# 🧪 Execute Evaluations

```bash
python test_agent.py
```

or

```bash
pytest
```

---

# 📊 What DeepEval Produces

After execution DeepEval automatically provides:

✅ Task Completion Score

✅ Tool Correctness Score

✅ Evaluation Reasons

✅ Trace Collection

✅ Component-level Insights

✅ Golden Dataset Validation

---

# 💡 Learning Outcomes

After completing this project you'll understand:

- AI Agent Testing
- DeepEval
- LangChain Evaluation
- LLM Observability
- AI Quality Engineering
- Agent Instrumentation
- Component-level Metrics
- Prompt Evaluation
- RAG Evaluation
- Tool Validation
- Production AI QA

---

# 🎯 Ideal For

- AI QA Engineers
- Lead SDETs
- QA Automation Engineers
- AI Automation Engineers
- LLM Evaluation Engineers
- GenAI Engineers
- QA Managers
- Engineering Managers
- Recruiters hiring AI Test Engineers

---

# 🌐 Repository

## GitHub

⭐ **Repository**

https://github.com/ArpitChoubey/deepeval-agent-project

---

# 👨‍💻 About Me

## Arpit Choubey

**Senior Software Development Engineer in Test (SDET)**

Specializing in:

- AI Testing
- Playwright
- Selenium
- Python
- Java
- LangChain
- DeepEval
- MCP
- REST API Testing
- CI/CD
- Docker
- Jenkins
- GitHub Actions

LinkedIn

https://www.linkedin.com/in/arpitchoubey/

Medium

https://medium.com/@ArpitChoubey9

GitHub

https://github.com/ArpitChoubey

---

# ⭐ Support

If you found this project useful:

⭐ Star the repository

🍴 Fork it

📢 Share it with the AI Testing community

🤝 Connect with me on LinkedIn

---

# 📈 Keywords

AI Testing • DeepEval • LangChain • Claude • GPT-4o • AI Agents • Agentic AI • LLM Evaluation • GenAI Testing • Python • AI Quality Engineering • Prompt Testing • Tool Correctness • Task Completion • Observability • AI Automation • QA Automation • Lead SDET • Open Source

---

## ⭐ If you're a Recruiter, Hiring Manager, QA Lead, or Engineering Manager evaluating AI Quality Engineering skills, this repository demonstrates practical experience with modern LLM evaluation techniques using production-oriented tooling and workflows.
