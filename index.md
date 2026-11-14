---
layout: home
title: Limitcode OSS
nav_order: 1
description: "An AI pair programming agent that stays inside Sublime Text."
permalink: /
---

<div class="hero">
  <p class="eyebrow">OPEN SOURCE · SUBLIME TEXT</p>
  <h1>AI pair programming,<br><span>inside your editor.</span></h1>
  <p class="hero-copy">Limitcode is an AI coding agent for Sublime Text. You decide what it can see, it makes focused edits, and every change stays reviewable in your buffer.</p>
  <div class="hero-actions">
    <a class="btn btn-primary" href="{{ site.baseurl }}/getting-started/">Get started</a>
    <a class="btn btn-secondary" href="https://github.com/Jawuilp/Limitcode">View on GitHub</a>
  </div>
</div>

<div class="docs-note">
  <strong>New in v1.2.0:</strong> <strong>Inline Assist</strong> is now live! Generate, edit, and refactor code directly inside your buffer with real-time diff previews inspired by Zed and GitHub Copilot. <a href="{{ site.baseurl }}/features/#inline-assist-in-buffer-ai-transformation">Explore Inline Assist &rarr;</a>
</div>

## The small tool surface is the feature

Limitcode deliberately gives the agent only three tools:

| Tool | Purpose | Scope |
|:-----|:--------|:------|
| `read_file` | Read an open file's buffer content | Only files active/open in Sublime Text |
| `write_to_file` | Replace an open file's buffer content | Only files active/open in Sublime Text |
| `edit_file` | Apply focused line edits | Only files active/open in Sublime Text |

No hidden filesystem scans. No unauthorized shell access. No autopilot. You steer the session and save the changes when they are ready.

---

## Built for a reviewable workflow

1. **Open** the files you want the agent to understand.
2. **Transform** code in-buffer with Inline Assist (`ctrl+i`) or ask questions in the side-by-side chat view.
3. **Review** the live diff indicators directly in Sublime Text before saving.
4. **Save** (`Ctrl+S`) only when the result looks right.

---

## What is included

* **Inline Assist:** In-buffer code transformation, real-time diff preview, and one-click Accept/Reject.
* **Editor-Native Chat:** Streaming conversation view that matches your editor theme and font preferences.
* **Review Before Save:** Unsaved buffer-first deliveries; your disk remains untouched until you save.
* **Broad Provider Support:** OpenAI, Anthropic, Gemini, DeepSeek, OpenRouter, Moonshot AI, plus local Ollama, LM Studio, and Llamafile.
* **Persistent Sessions:** Multi-session history, `@`-file references, and reasoning controls.
* **LSP Integration:** Automated post-edit diagnostics when the Sublime LSP package is active.

> Want an autonomous agent with project-wide search, terminal commands, web search, skills, and MCP tools? Check out [Limitcode Pro](https://limitcode.jawuil.dev/).

---

## Community, Support & Feedback

Limitcode is an open-source project created for the Sublime Text community. We welcome all bug reports, questions, and feature suggestions:

* **Report a Bug or Suggest a Feature:** Open an issue on GitHub at [Jawuilp/Limitcode Issues](https://github.com/Jawuilp/Limitcode/issues).
* **Ask Questions or Give Feedback:** Join the discussion on the official [Sublime Text Forum](https://forum.sublimetext.com/t/limitcode-ai-pair-programming-for-sublime-text/79034).
* **Direct Contact:** You can reach the creator via email at [contact@jawuil.dev](mailto:contact@jawuil.dev) or on X/Twitter [@Jawuil_p](https://x.com/Jawuil_p).

---

## Next steps

* [Install and start using Limitcode]({{ site.baseurl }}/getting-started/)
* [Explore all features with visual demos]({{ site.baseurl }}/features/)
* [View available commands and shortcuts]({{ site.baseurl }}/commands/)
* [Configure providers and models]({{ site.baseurl }}/configuration/)
* [Compare with Limitcode Pro]({{ site.baseurl }}/limitcode-pro/)
