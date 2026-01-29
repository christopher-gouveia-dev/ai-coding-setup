# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains configuration and prompt files for AI-assisted development using Continue.dev and similar tools. The project establishes strict guidelines for how AI assistants should behave when working on development tasks.

## Key Files and Directories

- `AI.md`: Central configuration file defining mandatory rules for AI behavior
- `.continue/`: Directory containing Continue.dev configuration and custom prompts
- `.continue/prompts/`: Custom prompt templates for different roles (developer, architect, QA, business analyst)
- `output/`: Directory containing generated files and documentation

## AI Behavior Rules

All AI interactions must follow the strict rules defined in `AI.md`:

1. **No autonomous actions**: Do NOT act autonomously; always wait for explicit human validation
2. **No git operations**: Do NOT commit, push, tag, or modify git history
3. **Incremental changes**: Prefer small, incremental, testable changes
4. **Workflow compliance**: Follow the mandatory 6-step workflow (analyze, propose, validate, implement one task, provide tests, stop)

## Continue.dev Configuration

The project uses Continue.dev with custom role-based prompts:

- `dev.md`: Developer role focusing on implementing single tasks with minimal changes
- `arch.md`: Architect role for proposing designs and splitting work into small tasks
- `qa.md`: QA role for creating test strategies and validation checklists
- `ba.md`: Business Analyst role for translating ideas into user stories and acceptance criteria

## Development Approach

1. **Strict adherence to AI.md**: All interactions must comply with the rules in AI.md
2. **Single task focus**: Implement only one task at a time as validated by the human
3. **Minimal changes**: Keep code modifications small and focused
4. **Validation required**: Always provide tests or validation steps with implementations

## Common Tasks

- Creating or modifying prompt templates in `.continue/prompts/`
- Updating configuration in `.continue/config.yaml`
- Adding new AI behavior guidelines to `AI.md`
- Generating documentation in the `output/` directory

## Key Constraints

- Never commit or push code
- Never modify git history
- Always wait for human validation before proceeding
- Implement only one task at a time
- Follow existing conventions strictly
- Provide clear validation steps for all changes