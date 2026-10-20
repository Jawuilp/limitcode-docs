---
layout: default
title: Commands
nav_order: 6
---

# Commands

Limitcode adds these commands to Sublime Text's Command Palette:

- `Limitcode: Open Chat`
- `Limitcode: New Chat`
- `Limitcode: Chat History`
- `Limitcode: Rename Session`
- `Limitcode: Delete Session`
- `Limitcode: Send to Agent`
- `Limitcode: Change Provider`
- `Limitcode: Change Model`
- `Limitcode: Increase Chat Font Size`
- `Limitcode: Decrease Chat Font Size`
- `Limitcode: Reset Chat Font Size`
- `Limitcode: Set Reasoning Effort`
- `Limitcode: Toggle Show Thoughts`
- `Limitcode: Setup Provider API Key`
- `Limitcode: Open Settings`
- `Limitcode: Open Key Bindings`
- `Limitcode: Clear Chat`
- `Limitcode: Cancel Active Response`
- `Limitcode: Stop Agent`

## Keyboard shortcuts

Limitcode does not claim global shortcuts when installed. Inside the chat,
`Enter`, `Shift+Enter`, `Escape`, `Up`, and `Down` are context-specific controls.

To add global shortcuts, run **Limitcode: Open Key Bindings** and add bindings
in the user pane:

```json
[
    { "keys": ["ctrl+alt+l"], "command": "limitcode_open_chat" },
    { "keys": ["ctrl+alt+a"], "command": "limitcode_send_to_agent" },
    { "keys": ["ctrl+alt+x"], "command": "limitcode_cancel_request" }
]
```
