# WingsCODE-Knowledge-Assistant
Guardrailed RAG-based AI Knowledge Assistant built with Botpress for the Barakah TechLabs AI &amp; Workflow Automation Internship.
# WingsCODE Knowledge Assistant

### Guardrailed RAG-Based AI Knowledge Assistant

A knowledge-grounded AI chatbot developed with **Botpress** as part of the **Barakah TechLabs AI & Workflow Automation Internship**.

The project demonstrates how a chatbot can retrieve information from an approved knowledge base while using strict guardrails to prevent unsupported or fabricated answers.

---

## 🚀 Project Overview

**WingsCODE Knowledge Assistant** is an AI-powered knowledge assistant designed to answer questions about WingsCODE using information provided through a dedicated knowledge base.

The primary objective is to demonstrate:

* Retrieval-Augmented Generation (RAG)
* Knowledge Base integration
* Grounded AI responses
* Anti-hallucination guardrails
* Controlled information retrieval
* Professional conversational responses

The assistant is instructed to use the connected knowledge base as its primary source and avoid presenting unsupported information as verified company information.

---

## 🧠 Key Features

### Knowledge-Based Q&A

The assistant retrieves relevant information from the connected WingsCODE knowledge base and uses it to answer user questions.

### RAG Workflow

The project follows the basic RAG pattern:

```text
User Question
      ↓
Knowledge Retrieval
      ↓
Relevant Information
      ↓
AI Response
```

### Anti-Hallucination Guardrails

The assistant is explicitly instructed not to invent:

* Prices
* Client information
* Employee information
* Refund policies
* Guarantees
* Company-specific dates
* Private company information
* Other unsupported claims

When requested information is unavailable, the assistant is instructed to clearly communicate that it does not have the information in its current knowledge base.

### Concise Professional Responses

Responses are designed to be:

* Clear
* Concise
* Professional
* Relevant to the user's question

---

## 📚 Knowledge Base

The assistant uses the following document as its approved knowledge source:

**WingsCODE Guardrailed RAG Knowledge Base**

The document contains information about:

* WingsCODE
* Core services
* Web development
* AI chatbot development
* AI workflow automation
* Knowledge-based AI
* Project development process
* Retrieval-Augmented Generation
* Guardrail policies
* Information boundaries
* Frequently asked questions
* RAG testing scenarios

The original knowledge-base document is available in the [`knowledge-base`](./knowledge-base/) directory.

---

## 🛡️ Guardrail Strategy

The assistant follows a strict grounding policy.

### Supported Information

If the requested information exists in the knowledge base, the assistant should provide an answer based on that information.

### Unsupported Information

If the requested information is not available, the assistant should not guess.

Example:

> "I don't have that information in my current knowledge base."

This prevents the chatbot from presenting unsupported information as verified WingsCODE information.

---

## 🧪 Testing

The assistant was tested using both supported and unsupported questions.

### Knowledge Retrieval Test

**Question:**

> What services does WingsCODE provide?

**Expected behavior:**

The assistant retrieves and summarizes the relevant services from the knowledge base.

### RAG Test

**Question:**

> What is RAG?

**Expected behavior:**

The assistant provides an explanation based on the information contained in the knowledge base.

### Guardrail Test

**Question:**

> What is the price of an AI chatbot?

**Expected behavior:**

The assistant should not invent a price because exact service pricing is not documented in the knowledge base.

### Unsupported Client Information Test

**Question:**

> Who are WingsCODE's clients?

**Expected behavior:**

The assistant should not fabricate client names or claim knowledge that is not present in the knowledge base.

---

## 📸 Project Evidence

### Knowledge Base

The WingsCODE knowledge-base document was uploaded and connected to the Botpress agent.

![Knowledge Base](./screenshots/knowledge-base.png)

### Agent Grounding Instructions

The agent was configured with grounding and anti-invention instructions.

![Agent Instructions](./screenshots/agent-instructions.png)

### RAG Response

Example of the assistant answering a question using the knowledge base.

![RAG Response](./screenshots/rag-response.png)

### Guardrail Response

Example of the assistant refusing to fabricate unavailable information.

![Guardrail Response](./screenshots/guardrail-response.png)

---

## 🛠️ Technology

* **Botpress**
* **Retrieval-Augmented Generation (RAG)**
* **Knowledge Bases**
* **Conversational AI**
* **AI Guardrails**

---

## 🎯 Internship Task

**Program:** Barakah TechLabs AI & Workflow Automation Internship

**Task:** Knowledge Base Integration (RAG)

**Project:** WingsCODE Knowledge Assistant

The project demonstrates the practical implementation of a knowledge-grounded conversational AI system with anti-hallucination safeguards.

---

## 📌 Project Status

**Status:** Completed

The assistant has been configured, tested, and published through Botpress.

---

## 👨‍💻 Developer

**Muhammad Nayyar Ameer**

Built as part of the AI & Workflow Automation internship learning and portfolio work.
