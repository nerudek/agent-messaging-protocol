# Agent Messaging Protocol (AMP)

> **Previously:** acp-bridge / skill-acp-bridge (DEPRECATED)

Agent-to-agent communication protocol built on the Agent Client Protocol (ACP). Enables cross-agent messaging between Claude, Kimi, OpenClaw, and Hermes agents with a unified command interface.

## Overview

AMP provides a standardized messaging layer for multi-agent AI ecosystems. Each agent communicates via acpx-style commands over a shared protocol, with Hermes using an MCP/filesystem workaround for compatibility.

**Key features:**
- Cross-agent message routing (Claude, Kimi, OpenClaw, Hermes)
- acpx command syntax for all agents
- Hermes compatibility layer (MCP bridge / file-based relay)
- Lightweight, skill-based architecture
- MIT licensed

## Installation

```bash
# Clone to your OpenClaw skills directory
git clone https://github.com/nerudek/agent-messaging-protocol.git ~/.openclaw/skills/agent-messaging-protocol

# Or symlink if you keep skills elsewhere
ln -s /path/to/agent-messaging-protocol ~/.openclaw/skills/agent-messaging-protocol
```

## Usage

Full documentation is in [SKILL.md](SKILL.md).

Quick start:
- See `SKILL.md` for protocol commands and agent addressing
- Each agent registers its identity via the protocol header
- Messages are routed through the ACP bridge layer

## Requirements

- OpenClaw >= 2026.4.0 (or compatible agent runtime)
- Network access for cross-agent communication
- MCP client or filesystem access for Hermes agents

## Repository

- **GitHub:** [github.com/nerudek/agent-messaging-protocol](https://github.com/nerudek/agent-messaging-protocol)
- **Issues:** [github.com/nerudek/agent-messaging-protocol/issues](https://github.com/nerudek/agent-messaging-protocol/issues)
- **Package:** `nerudek/agent-messaging-protocol`

## Version

Current version: `1.2.0`

## License

MIT — see [package.json](package.json) for details.

---

Built by [nerudek](https://github.com/nerudek). Support: [PayPal.me/nerudek](https://www.paypal.me/nerudek)
