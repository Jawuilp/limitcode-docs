---
layout: default
title: Configuration
nav_order: 4
---

# Configuration

Open **Limitcode: Open Settings** to edit the user settings file. A minimal setup looks like this:

```json
{
    "default_provider": "openai",
    "default_model": "gpt-5.5",
    "api_keys": {
        "openai": ""
    },
    "temperature": "auto",
    "max_tokens": 8192,
    "max_iterations": 50,
    "chat_font_size": "auto",
    "reasoning_effort": "off",
    "show_thoughts": false,
    "auto_save_edits": false
}
```

## Common options

| Option | Values | Description |
|:-------|:-------|:------------|
| `default_provider` | Provider name | Provider used for new sessions |
| `default_model` | Model name | Model used for new sessions |
| `temperature` | `"auto"` or number | Controls response randomness |
| `max_tokens` | `"auto"` or positive integer | Maximum response length |
| `max_iterations` | Positive integer | Maximum tool loop iterations |
| `chat_font_size` | `"auto"` or positive number | Font size for the Limitcode chat view |
| `reasoning_effort` | `off`, `low`, `medium`, `high` | Reasoning level where supported |
| `show_thoughts` | `true` or `false` | Show model reasoning where supported |
| `auto_save_edits` | `true` or `false` | Save files automatically after edits |

Provider keys can also be configured through **Limitcode: Setup Provider API Key**. Never commit keys to the repository or paste them into issue reports.

`temperature` accepts `"auto"` or a number. `max_tokens` accepts `"auto"` or a
positive integer. Unsupported models ignore `reasoning_effort`.

## Chat appearance

The chat font follows Sublime Text's global font size by default. Set a fixed
size with `"chat_font_size": 11`. The chat status bar can also be customized
with `chat_style`, or with a user CSS override at
`Packages/User/Limitcode/chat.css`.
