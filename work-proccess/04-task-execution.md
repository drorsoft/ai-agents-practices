# Task Execution

## Asking the AI to Execute the Task

Once the task is defined and edited, you can ask the AI agent to execute the task. The AI agent will follow the plan and complete the task as specified.

use the following prompt to ask the AI agent to execute the task:
```prompt
I would like you to execute the task. In the task file `<task_file_name>`.
before executing the task, please refer to the file
`repo_spec-for-agents.md` in the docs folder.
```
## Inspection results - part 1
The first part of the inspection results will mean to check if the code is working as expected. The AI agent will run the code and check for any errors or issues. If there are any errors, the AI agent will fix them and re-run the code.

## Inspection results - part 2
> This is in most cases the more important part of the inspection!

Check for code quality, readability, and maintainability. The AI agent will check for any code smells, anti-patterns, or other issues that may affect the quality of the code. The AI agent will also check for any best practices that are not being followed.

```prompt
The task is executed, but I would like you to check the code quality, readability, and maintainability. Please check for any code smells, anti-patterns, or other issues that may affect the quality of the code. Also check for any best practices that are not being followed.

*Please improve the code quality, readability, and maintainability.* 
```

If the code is not readable or not easy to understand, ask the AI agent to improve the code quality, suggest better variable names, change control flow, and improve the overall readability of the code.

  

## Adding tests to the Task

You can use the following prompt to add tests to the task:
```prompt
Please add the following tests to the task:
<test cases>
```

