---
layout: default
title: Getting started
nav_order: 2
has_children: false
permalink: /getting-started/
---

# Getting started

## Requirements

- Sublime Text 4 or newer
- An API key for a cloud provider, or a local Ollama/LM Studio/Llamafile installation

## Install from source

### Recommended: Package Control

1. Open the Command Palette in Sublime Text.
2. Run **Package Control: Install Package**.
3. Search for **Limitcode** and install it.

Limitcode OSS is published in the [Sublime Package Control
catalog](https://packagecontrol.io/packages/Limitcode), so Package Control
will handle the installation and updates.

### Install from source

Clone the repository into Sublime Text's `Packages` directory when you want to
work from the source tree:

```powershell
cd "$env:APPDATA\Sublime Text\Packages"
git clone https://github.com/Jawuilp/Limitcode.git Limitcode
```

Restart Sublime Text after cloning.

## Open your first chat

1. Open the Command Palette.
2. Run **Limitcode: Setup Provider API Key**.
3. Run **Limitcode: Open Chat**.
4. Open the files you want Limitcode to read or edit.
5. Describe the task in the chat.

Limitcode only works with files that are already open in the active Sublime Text window.

## Send code to the agent

Select the code you want to discuss and run **Limitcode: Send to Agent**, or describe the task directly in the chat. Edits are applied to the editor buffer for review. By default, they are not saved to disk until you save the file.

## Optional: install LSP

If the [LSP package](https://packagecontrol.io/packages/LSP) is installed, Limitcode can use its diagnostics after an edit. This is optional and activates automatically when available.
