---
tags: [windows, wsl2, ollama, docker, local-llm]
---

# Local Windows AI Server

## Purpose
Use the Windows machine as a local server for:
- Docker
- Databases
- Private/local LLMs such as Ollama
- AI agents / Claude workers
- Local services accessed from Mac

## Current Preference
Keep Mac as the main development machine. Use Windows as a powerful local backend/server.

## Setup Notes
- Run heavy services on Windows or WSL2.
- Access services from Mac over LAN.
- Prefer wired Ethernet for Mac ↔ Windows.
- Consider 2.5GbE or 10GbE only if local file transfer / Parsec / local LLM workloads justify it.

## Services to Run
| Service | Where | Notes |
|---|---|---|
| Ollama | Windows native or WSL2 | Native may better access GPU |
| PostgreSQL | Docker / WSL2 | Good for apps and vector experiments |
| Docker workloads | WSL2 | Keep isolated |
| Whisper | Windows native if using GPU | Expose API to Mac if needed |

## Troubleshooting Notes
- Check whether port `11434` is listening.
- Confirm firewall allows LAN access.
- Test from Mac with `curl http://WINDOWS_IP:11434/api/tags`.
- Avoid binding conflicts when restarting Ollama.
