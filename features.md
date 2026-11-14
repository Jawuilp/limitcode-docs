---
layout: default
title: Features
nav_order: 3
permalink: /features/
---

# Features

Limitcode brings AI pair-programming directly into Sublime Text without forcing you into an unfamiliar browser view or separate AI IDE. Every feature is designed around editor-native speed, focused file control, and human review.

---

## Inline Assist (In-Buffer AI Transformation)

Generate, edit, refactor, and explain code directly inside your active buffer without switching to the chat view. Inspired by the inline assist workflows in Zed and GitHub Copilot, Limitcode renders an interactive minihtml block phantom right where your cursor or selection is.

<img src="{{ site.baseurl }}/assets/images/inline-assist.gif" alt="Limitcode Inline Assist Demo" class="docs-gif" />

### Key Highlights
* **In-buffer generation:** Select any function, block, or empty line, and prompt the model (`Limitcode: Inline Assist` or `ctrl+i`).
* **Interactive Visual Diff:** Review green additions and red deletions before touching your file.
* **One-Click Controls:**
  * **Accept (`Enter`):** Instantly replaces the selection with the clean replacement code.
  * **Reject / Cancel (`Esc`):** Closes the phantom without modifying a single character.
  * **Open in Chat:** Transfers your prompt, code context, and model output into the Chat panel to continue an extended conversation.
  * **Retry:** Re-runs the request with a single click if you want a different variation.
* **Adaptive Viewport Layout:** Automatically calculates your editor's column width so lines wrap cleanly and never clip horizontally.
* **Reasoning model support:** Cleanly parses `<think>...</think>` tags from models like DeepSeek-R1 and Nemotron, displaying real-time thought status without cluttering code.

---

## Editor-Native Streaming Chat

Chat with the agent side-by-side with your code in a dedicated Sublime Text view that feels like a native part of the editor.

<img src="{{ site.baseurl }}/assets/images/oss-session-1.gif" alt="Limitcode Chat Pair Programming" class="docs-gif" />

* **Zero Context Switching:** Keep your code on one side and the conversational agent on the other.
* **Independent Font Sizing:** Tune the chat font size separately from your editor font (`Limitcode: Increase/Decrease Chat Font Size`).
* **Image Attachment Support:** Paste images or UI mockups directly from your clipboard into the chat for multimodal models (e.g. GPT-4o, Claude 3.5 Sonnet, Gemini 1.5/2.0).
* **Theme-Aware Status Bar:** Displays the current provider, active model, and conversation token estimates matching your Sublime Text theme.

---

## Review Before Save (Zero-Risk Edits)

With Limitcode, the agent never overwrites your files on disk silently.

<img src="{{ site.baseurl }}/assets/images/oss-pomodoro-1.gif" alt="Limitcode Review Before Save Demo" class="docs-gif" />

* **Buffer-First Delivery:** When the agent modifies or creates code, the change lands directly in the active editor buffer as an unsaved modification.
* **Visual Gutter Diffs:** Sublime Text's native diff indicators show every addition and modification in real time.
* **You Stay in Control:** Inspect the edits, make manual adjustments, and save (`Ctrl+S`) only when you are satisfied. If you prefer automatic saving, enable `"auto_save_edits": true` in your settings.

---

## Focused File Access & Privacy

Limitcode deliberately constrains the agent's file access tools:

| Tool | Capability | Boundary |
|:-----|:-----------|:---------|
| `read_file` | Reads file content | **Only files open** in your active Sublime Text window |
| `write_to_file` | Replaces file content | **Only files open** in your active Sublime Text window |
| `edit_file` | Applies focused line replacements | **Only files open** in your active Sublime Text window |

* **No Blind Scans:** The agent cannot index your entire disk or traverse private folders behind your back.
* **No Shell Execution:** Limitcode OSS does not run terminal commands on your operating system without your oversight.

---

## Multi-Provider Flexibility

Connect Limitcode to your preferred model provider in seconds:

* **Cloud Providers:** OpenAI (GPT-4o, o1, o3-mini), Anthropic (Claude 3.5/3.7), Google Gemini (Gemini 2.0 Flash/Pro), DeepSeek, OpenRouter, and Moonshot AI (Kimi).
* **Local & Offline Models:** Full native compatibility with **Ollama**, **LM Studio**, and **Llamafile**. Run private open-source models (Llama 3, DeepSeek-R1, Qwen 2.5) with zero data leaving your machine.

---

## LSP Integration (Optional Diagnostics)

If you have the [Sublime Text LSP](https://packagecontrol.io/packages/LSP) package installed for your language, Limitcode automatically detects it. After applying an edit, the agent receives language server diagnostics to catch syntax mistakes, missing imports, or type errors immediately.

---

## Sessions, History, and Reasoning Controls

* **Persistent Sessions:** Name, switch, or resume past conversations at any time (`Limitcode: Chat History`).
* **`@`-File References:** Type `@filename` in chat to quickly point the agent's attention to a specific open file.
* **Configurable Reasoning Effort:** Adjust thinking intensity (`off`, `low`, `medium`, `high`) for models with reasoning architectures.
