# LLM Code Generation Workflow Summary

This document summarizes Harper Reed's approach to using AI for code generation, as detailed in [his blog post](https://harper.blog/2025/02/16/my-llm-codegen-workflow-atm/).

## Greenfield Development Process (New Projects)

### 1. Idea Honing
- Use conversational LLMs like ChatGPT 4o/o3 to refine the idea
- Have the AI ask one question at a time to develop a thorough spec
- Save the output as `spec.md` in the repository

### 2. Planning
- Feed the spec to a reasoning model (Claude Opus, GPT-4o, etc.)
- Use specific prompts to break down the project into small, iterative steps
- Generate a prompt plan (`prompt_plan.md`) and a checklist (`todo.md`)

### 3. Execution
- Options include using GitHub Workspace, Aider, Cursor, Claude Engineer, etc.
- Two preferred approaches:
  - **Claude**: Manually set up repo boilerplate, paste prompts into Claude, and copy code into IDE
  - **Aider**: Set up repo, start Aider, and paste prompts to have it implement code automatically

## Non-Greenfield Process (Existing Codebases)

### 1. Get Context
- Use tools like [repomix](https://github.com/yamadashy/repomix) to grab source code efficiently
- Generate context files to feed to LLMs

### 2. Prompt Magic
- Use specific prompts for:
  - Code review
  - GitHub issue generation
  - Identifying missing tests

## Key Insights and Challenges

1. **Stay Organized**: Reed warns about getting "over his skis" - moving too fast without proper tracking
2. **Testing is Important**: Especially when using automated tools like Aider
3. **Loneliness**: Current workflows are primarily solo endeavors, lacking team collaboration features
4. **Productivity**: The approach has dramatically increased Reed's coding productivity
5. **Downtime Management**: Reed fills LLM processing time with brainstorming other projects or leisure activities

## Recommended Resources
- Book: "Co-Intelligence: Living and Working with AI" by Ethan Mollick - for balanced perspectives on working with LLMs
