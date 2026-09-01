# AI Development Stack

## Subscriptions and API Infrastructure

| Provider | Access Method | Budget Layer | Target Workloads |
| :--- | :--- | :--- | :--- |
| Anthropic Claude Pro | Web UI / ClaudeCode CLI | 20 EUR / Mo Fixed | Complex system architecture, high-level prose, multi-file refactoring workflows |
| OpenRouter | API Endpoint | 50 EUR / Mo Metered | Inline text completions, uncensored generation, heavy programming loops |
| Ollama | Local Localhost | 0 EUR (Free) | Boilerplate generation, syntax checking, low-latency offline executions |

## Model Routing Matrix

| Model Identifier | Host Provider | Guardrail Status | Primary Engineering Use Case |
| :--- | :--- | :--- | :--- |
| anthropic/claude-3.5-sonnet | Claude Pro / OpenRouter | High Restriction | Complex logic, code generation, detailed technical writing |
| deepseek/deepseek-r1 | OpenRouter | Objective | Complex reasoning, mathematical validation, logic-heavy programming |
| nousresearch/hermes-3-llama-3.1-405b | OpenRouter | Uncensored | Raw generation, deep vulnerability testing, zero-refusal scenarios |
| qwen2.5-coder:7b-instruct-q8_0 | Local (Ollama) | Minimal | High-speed local code completion, background syntax checks |
| hermes3:8b | Local (Ollama) | Uncensored | Offline prototyping, localized script generation, raw text generation |

## Core Tooling and Runtime Layer

| Tool Name | Interface Type | Integration Hook | Functionality |
| :--- | :--- | :--- | :--- |
| Zed Editor | Desktop UI | OpenRouter API / Ollama | Rust-based GPU-accelerated editor for inline completions |
| Aider | Command Line | OpenRouter API | Terminal-first pair programmer with automated Git commit loops |
| ClaudeCode | Command Line | Anthropic Token / OpenRouter | Native Anthropic CLI agent for autonomous workspace debugging |
| OpenCode | Command Line | OpenRouter API | Model-agnostic terminal agent for custom workflow execution |
| Arize Phoenix | Web UI / Docker | Local Container Execution | Local-first trace visualization for LangGraph pipelines |
| Promptfoo | Command Line | Local Test Engine | Test-driven configuration verification for prompt payloads |
