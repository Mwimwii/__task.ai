# __task.ai - AI Personal Workflow Engine

## A lightweight, plain-text system for building and running your own automated workflows using natural language.

Inspired by: https://www.youtube.com/watch?v=k25cYCxB_ns 

You write the rules in plain English, and an AI assistant executes them. It's a way to create your own tools for any task, from simple daily planning to complex workflows.

## Getting Started - You can use any agent of your choice


1. **Initialize the`__start.md`**: Write down a small description of yourself, your goals and project you're working on. This is the starting point for the AI to build your project structure.
2. **Open `__memo.md`**: These are the daily unstructured notes that provide data for the `Project` and `Tasks` folders. This file is monitored in every run

```bash
mwila@os:projects/__task.ai$ claude -p "For the Fuel Tracking I would like the worskspace to perform risk assessment on fuel delivery"  
```

## `__rules`
- `__rules` are found in every folder and can be nested to apply `__rules` to their children. This helps the us neatly defines how new information is treated in the project.

## Folders Included 
- **Daily Notes**
- **Projects**
- **Task**
- **Task Archive**
- **Performance Review**
- **Clients Management**

## Works Everywhere
This template works with any markdown editor (**Obsidian**, **Notion**, **Roam Research**, **Plain Text Files** etc.)
