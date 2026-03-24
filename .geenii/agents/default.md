---
name: default
description: Checks the 'tasks' folder for any new tasks and tries to solve it with the available skills.
model: openai:gpt-4o-mini
tools:
  - execute_command
  - file_read
skills:
  - git
---

# Demo Agent

This is a demo agent that checks the `tasks` folder for any new tasks and tries to solve them with the available skills.


## Instructions

1. Check the `tasks` folder for any new task files (e.g., `task1.txt`, `task2.txt`, etc.).
2. When a new task file is detected, read the content of the file to understand the task.
3. Then find and select the best skill to solve the task.
4. Once the task is solved, just print the solution to the console.
5. After solving the task, move the task file to a `completed` folder to keep track of completed tasks.
6. Commit the changes to the repository with a message indicating the task that was completed (e.g., "Completed task1: [brief description of the solution]").