---
layout: default
title: Features
nav_order: 3
permalink: /features/
---

# Features

## Inline Assist (in-buffer AI coding)

Generate, edit, and refactor code directly inside your active buffer without switching to the chat panel. Inspired by the inline assist workflows in Zed and GitHub Copilot, Limitcode renders an adaptive diff preview directly under your code inside a native minihtml block phantom.

* **In-buffer edits:** Select any code block (or place your cursor anywhere) and prompt the model.
* **Visual Diff preview:** Review added and removed lines before applying them to your buffer.
* **One-click controls:** Instantly Accept edits (`Enter`), Reject them (`Esc`), or hand off the prompt and response to the Chat view to continue an extended conversation.
* **Adaptive layout:** Dynamically adjusts to your editor viewport width so explanations and code previews never clip or horizontally overflow.

## Editor-native chat

Chat streams directly inside Sublime Text, next to the code you are working on. Sessions keep their own conversation history so you can return to a task later.

## Focused file access

The agent can only operate on files with paths that are open in the active window. This keeps context explicit and prevents accidental project-wide scans.

## Review before save

Agent edits land in the buffer first. Sublime Text's diff indicators show what changed, and you choose whether to save it. Set `auto_save_edits` to `true` only if you prefer automatic saves.

## Provider flexibility

Use hosted providers such as OpenAI, Anthropic, Gemini, DeepSeek, OpenRouter, and Moonshot AI, or connect to local models through Ollama, LM Studio, and Llamafile.

## LSP feedback

When LSP is installed, diagnostics can be fed back after edits so the agent can catch syntax and type errors while working.

## Sessions and prompts

Limitcode includes persistent session history, prompt history, `@`-file references, configurable reasoning effort, and an option to show model thoughts where supported.
