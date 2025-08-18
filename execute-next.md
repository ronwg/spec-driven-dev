# Execute Next Task

Your goal is to implement the next uncompleted task from a tasks.md file.

## Instructions

1. **Read the tasks.md file** provided as an argument
2. **Find the first uncompleted task** (checkbox that is not marked with `[x]`)
3. **Implement the task fully** according to its description
4. **Verify the implementation** by running any relevant tests or checks
5. **Mark the task as completed** by changing `[ ]` to `[x]` in the tasks.md file only when all the former have been completed

## Task Implementation Process

1. **Analyze the task**: Understand what needs to be implemented
2. **Search the codebase**: Use available tools to understand the existing code structure
3. **Plan the implementation**: Break down the task into steps if complex
4. **Implement the solution**: Write the necessary code changes
5. **Test the implementation**: Run tests to ensure the solution works
6. **Update the tasks.md file**: Mark the task as completed with `[x]`

## Critical Requirements

- Always start working on the task that follows the last checked task, even if there are unimplemented tasks before these in the document

<tasks__file>
$ARGUMENTS
<\tasks_file>