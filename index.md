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

## The small tool surface is the feature

Limitcode deliberately gives the agent only three tools:

| Tool | Purpose |
|:-----|:--------|
| `read_file` | Read a file that is open in Sublime Text |
| `write_to_file` | Replace the contents of an open file |
| `edit_file` | Apply a focused edit to an open file |

No hidden filesystem scans. No shell access. No autopilot. You steer the session and save the changes when they are ready.

## Built for a reviewable workflow

1. **Open** the files you want the agent to understand.
2. **Ask** for a change or send a selection to the agent.
3. **Review** the edit directly in Sublime Text.
4. **Save** only when the result looks right.

## What is included

- Streaming chat inside Sublime Text
- Persistent conversation history per session
- Multiple model providers with per-session control
- Optional LSP diagnostics after edits
- Prompt history and `@`-file references
- Configurable reasoning effort and visible thinking

> Want the autonomous version? [Limitcode Pro](https://limitcode.jawuil.dev/) adds project-wide tools, shell commands, web access, skills, and MCP connections.

## Next steps

- [Install and start using Limitcode]({{ site.baseurl }}/getting-started/)
- [Explore the feature set]({{ site.baseurl }}/features/)
- [Configure providers and models]({{ site.baseurl }}/configuration/)
- [See all supported providers]({{ site.baseurl }}/providers/)
- [Compare with Limitcode Pro]({{ site.baseurl }}/limitcode-pro/)
