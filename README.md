# Spec-driven Development Prompts - Claude Code Command Collection

A collection of specialized Claude Code commands inspired by the powerful Spec-driven workflow created by Amazon. These commands help transform project ideas into comprehensive technical specifications and actionable implementation plans.

## Commands Overview

This collection includes four sequential commands for complete project planning and execution:

1. **`/requirements`** - Generate comprehensive BDD-style requirements from project descriptions
2. **`/design`** - Create detailed technical design documents from requirements  
3. **`/tasks`** - Transform design documents into actionable implementation plans
4. **`/execute-next`** - Implement the next uncompleted task from a tasks.md file

## Installation

1. **Install the commands in Claude Code:**
   ```bash
   # Copy commands to Claude Code's commands directory
   # The exact path may vary based on your system
   cp requirements.md design.md tasks.md execute-next.md ~/.claude/commands   
   ```

2. **Verify installation:**
   ```bash
   claude-code --help
   # You should see the new commands listed
   ```

## Usage Workflow

### Step 1: Generate Requirements
In Claude Code, start with a project/feature idea or basic description:

```bash
> /requirements "Build a surfer travel tips website with AI-powered content generation"
```

**What it does:**
- Creates comprehensive BDD-style requirements
- Defines user stories with detailed acceptance criteria
- Outputs a `requirements.md` file in a new directory named after the feature/request

### Step 2: Create Technical Design
Use the generated requirements to create a technical design:

```bash
> /design @surfer-travel-tips-website/requirements.md
```

**What it does:**
- Analyzes the requirements document
- Creates comprehensive technical architecture
- Generates data models, API specifications, and system design
- Outputs a `design.md` file with complete technical specifications

**Optional:** Include additional requirements files:
```bash
> /design @surfer-travel-tips-website/requirements.md @additional-requirements.md
```

### Step 3: Generate Implementation Tasks
Transform the design into actionable tasks ordered by dependency:

```bash
> /tasks @surfer-travel-tips-website/design.md @surfer-travel-tips-website/requirements.md
```

**What it does:**
- Creates a detailed, sequenced implementation plan
- Breaks down complex features into manageable tasks
- Maps each task back to original requirements
- Outputs a `tasks.md` file with checkboxes for progress tracking

### Step 4: Execute Next Task
Implement the next uncompleted task from the generated tasks file:

```bash
> /execute-next @surfer-travel-tips-website/tasks.md
```

**What it does:**
- Finds the first uncompleted task in the tasks.md file (following the last completed task)
- Implements the task fully according to its description
- Runs tests and verification checks
- Marks the task as completed by updating the checkbox


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
