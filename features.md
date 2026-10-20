---
layout: default
title: Features
nav_order: 3
permalink: /features/
---

# Features

## Editor-native chat

Chat streams directly inside Sublime Text, next to the code you are working on. Sessions keep their own conversation history so you can return to a task later.

## Focused file access

The agent can only operate on files with paths that are open in the active window. This keeps context explicit and prevents accidental project-wide scans.

## Review before save

Agent edits land in the buffer first. Sublime Text's diff indicators show what changed, and you choose whether to save it. Set `auto_save_edits` to `true` only if you prefer automatic saves.

## Provider flexibility

Use hosted providers such as OpenAI, Anthropic, Gemini, DeepSeek, OpenRouter, and Moonshot AI, or connect to local models through Ollama and LM Studio.

## LSP feedback

When LSP is installed, diagnostics can be fed back after edits so the agent can catch syntax and type errors while working.

## Sessions and prompts

Limitcode includes persistent session history, prompt history, `@`-file references, configurable reasoning effort, and an option to show model thoughts where supported.
