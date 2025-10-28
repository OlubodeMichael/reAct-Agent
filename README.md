# ReAct-LangChain

A demonstration of the ReAct (Reasoning and Acting) pattern using LangChain agents.

## Overview

This project implements a ReAct agent that can reason about problems and take actions using tools. The example includes a text length calculator tool that demonstrates how the agent can perform calculations and reasoning.

## Features

- ReAct agent implementation using LangChain
- Custom text length calculation tool
- OpenAI GPT integration
- Manual ReAct loop implementation showing the reasoning and acting process

## Setup

1. Install dependencies:

   ```bash
   pip install -e .
   ```

2. Create a `.env` file with your OpenAI API key:
   ```bash
   echo "OPENAI_API_KEY=your_api_key_here" > .env
   ```

## Usage

Run the main script:

```bash
python main.py
```

The agent will demonstrate its reasoning and acting capabilities by calculating the length of a text string.

## Requirements

- Python >= 3.14
- OpenAI API key
- LangChain and related packages (see pyproject.toml)

## How ReAct Works

The ReAct pattern combines reasoning and acting in a loop:

1. **Reason**: The agent thinks about what to do next
2. **Act**: The agent takes an action using available tools
3. **Observe**: The agent observes the result of the action
4. Repeat until the task is complete

This allows the agent to break down complex problems into smaller, manageable steps.

## Project Structure

- `main.py`: Contains the ReAct agent implementation with a text length calculation tool
- `pyproject.toml`: Project dependencies and configuration
- `.env`: Environment variables (create this file with your OpenAI API key)
