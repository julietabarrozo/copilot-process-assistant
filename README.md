# 🤖 Copilot Studio: Process Support Agent

## 📌 Overview
An AI-powered conversational agent built in **Microsoft Copilot Studio** designed to assist users with an operational process. 

The agent acts as a centralized knowledge assistant, leveraging organizational documents and SOPs (Standard Operating Procedures) to deliver concise answers without requiring manual searches through presentations or emails.

---

## 🛠️ Key Technical Specifications
- **Platform:** Microsoft Copilot Studio
- **Base LLM Model:** GPT-4.1
- **Architecture Pattern:** RAG (Retrieval-Augmented Generation)
- **Knowledge Sources:** Internal documentation, SOPs, and process guidelines.

---

## 💡 Capabilities & Features
- **Instant SOP Querying:** Synthesizes complex operational procedures into clear, actionable responses.
- **Knowledge Base Integration:** Retrieves real-time answers from connected organizational repositories.
- **Time Reduction:** Eliminates manual document searching for operational team members.
- **Interactive CSAT:** Uses Microsoft Teams Adaptive Cards to collect user feedback directly within the chat stream. 

---

## 📁 Repository Structure

```text
copilot-process-assistant/
│
└── src/
    ├── bots/
    │   └── configuration.json        # Global agent setup, channels (Teams/M365), and AI settings
    └── botcomponents/
        ├── system_instructions.yaml  # System prompts, strict guardrails, and model selection
        ├── conversation_start.yaml   # Initial greeting and trigger queries
        ├── search.yaml               # RAG logic, knowledge search, and team fallback
        ├── thank_you.yaml            # Adaptive Card schema for user feedback capture
        └── end_of_conversation.yaml  # Session closure and survey trigger

