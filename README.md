# __task.ai - A Personal Workflow Engine

## A lightweight, plain-text system for building and running your own automated workflows using natural language.

Inspired by: [this video on agentic workflows](http.googleusercontent.com/youtube.com/0)

You write the rules in plain English, and an AI assistant executes them. It's a way to create your own tools for any task, from simple daily planning to complex workflows. This system functions as a lightweight, self-hosted alternative to agentic frameworks like [LangChain](https://www.langchain.com/) or [Guidance](https://github.com/microsoft/guidance). Instead of defining chains and tools in code, you define them in plain text `__rules.md` files, using the file system itself as the environment for the AI agent to act upon.

## Getting Started - You can use any agent of your choice

1.  **Initialize the `__start.md`**: Write down a small description of yourself, your goals, and projects you're working on. This is the starting point for the AI to build your project structure.
2.  **Open `__memo.md`**: These are the daily unstructured notes that provide data for the `Project` and `Tasks` folders. This file is monitored in every run.
3.  **Run it with your agent**: Point your AI assistant to the workspace and give it a prompt.

**Example CLI Commands:**

```bash
# Claude
claude -p "For the Fuel Tracking project, perform a risk assessment on the new delivery data."

# OpenAI Codex CLI
codex "Based on the __memo.md, update the workspace according to the rules."

# Google Gemini CLI (non-interactive)
gemini --prompt "Run the task.ai workflow. Ingest the new memo and update all relevant project files."
```

## `__rules`
- `__rules` are found in every folder and can be nested to apply rules to their children. This allows for granular control over how information is processed and lets you build complex, chained logic for your workflows.

## Folders Included 
- **Daily Notes**
- **Projects**
- **Task**
- **Task Archive**
- **Performance Review**
- **Clients Management**

## Works Everywhere
This template works with any markdown editor (**Obsidian**, **Notion**, **Roam Research**, **Plain Text Files** etc.)
