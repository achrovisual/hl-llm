<div align="center">
  <h1>LLM Configuration</h1>
</div>

This is my **personal repository** for **System Prompts** and other configurations used with **Open WebUI** on my self-hosted Large Language Models (LLMs). The goal is to maintain a tested, consistent set of prompts for my specialized tasks and quick reference during setup.

---

## 🤖 System Prompts Reference

This repository organizes prompts based on their intended scope in Open WebUI:

* **General Prompt:** The system prompt located directly at `open-webui/system_prompt.txt` is intended for **general-purpose** use and can be set as the default across the entire user account or a non-specialized chat session. This prompt is currently the **Context-Aware, Time-Sensitive Assistant**.

* **Specific Prompts:** Prompts located inside the **`workspaces/`** directories are highly specialized for particular tasks (e.g., coding, translation, summarizing) and should be used within a dedicated Open WebUI Workspace or as a reusable slash command. The current workspace prompt is the **Development Documentation Assistant**.

---

## 🚀 Usage Guide

Use this as a quick reference when setting up a new Open WebUI container or updating a chat session's configuration.

### General Prompt Use:
Copy the content of the general prompt (`system_prompt.txt`) and paste it into the **System Prompt** field under your user **Settings** (for a global default) or the **Chat Controls** sidebar (for a single session).

### Workspace/Specific Prompt Use:
1.  **Create a Reusable Prompt:** Go to **Workspace** > **Prompts** in Open WebUI.
2.  **Paste Content:** Paste the content of the desired specific prompt (e.g., `workspaces/development/system_prompt.txt`) into the prompt template.
3.  **Set Command:** Set a command like `/dev-docs` or `/commit`.
4.  **Invoke:** In any chat, type the command (e.g., `/dev-docs`) to activate the specialized assistant's persona for that conversation.
