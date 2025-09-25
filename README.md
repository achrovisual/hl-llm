<div align="center">
  <h1>LLM Configuration</h1>
</div>

This is my **personal repository** for **System Prompts** and other configurations used with **Open WebUI** on my self-hosted Large Language Models (LLMs). The goal is to maintain a tested, consistent set of prompts for my specialized tasks and quick reference during setup.

---

## 🤖 System Prompts Reference

This section contains the current collection of meta-prompts that define the AI's core behavior, rules, and persona.

### 📝 Prompt 1: Context-Aware, Time-Sensitive Assistant

**Purpose:** This is the default, general-purpose prompt. It explicitly forces the model to inject the current date and time into its context, which is crucial for making responses relevant for real-time questions, events, scheduling, or determining if information is outdated.

**Path:** `open-webui/system_prompt.txt`

**Content:**
```
You are a context-aware assistant. When responding, always consider the current date and time to provide the most relevant information.

**Current Date:** {{CURRENT_DATE}}
**Current Time:** {{CURRENT_TIME}}

**Your Task:**
Based on the user's request, provide a response that is timely and accurate. If the user asks about an event, check if it has already occurred or is upcoming based on the current date.
```

---

## ⚙️ Future Configurations & Tasks

This section tracks planned additions and specialized configurations for the repository:

* **Linux Shell Assistant:** A prompt focused on providing validated shell commands and scripting advice, strictly formatted in Markdown code blocks for easy copying.

---

## 🚀 Usage Guide

Use this as a quick reference when setting up a new Open WebUI container or starting a new chat session.

1.  **Locate:** Find the desired prompt content in the `/open-webui/` directory.
2.  **Copy/Paste:** Copy the content and paste it into the **System Prompt** field in Open WebUI.
    * **Note:** The Open WebUI environment is expected to automatically substitute the **`{{CURRENT_DATE}}`** and **`{{CURRENT_TIME}}`** variables with the actual values.