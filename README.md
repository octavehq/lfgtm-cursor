# Octave Cursor Plugin

> Generated from [octavehq/lfgtm](https://github.com/octavehq/lfgtm). Do not edit directly — changes will be overwritten. File issues and PRs on the upstream repo.

GTM knowledge base integration for [Cursor](https://cursor.com). Provides grounded access to your Octave personas, Motions, messaging, positioning, and more — as skills, agents, and commands.

## Install

Add this plugin from the Cursor marketplace, or point Cursor at this repository:

```
https://github.com/octavehq/lfgtm-cursor
```

See Cursor's [plugins documentation](https://cursor.com/docs/reference/plugins) for installation details.

## Configure your Octave MCP server

This plugin ships no MCP config — add your workspace's Octave server (one per workspace) to Cursor's MCP settings:

```json
{
  "mcpServers": {
    "octave-acme": {
      "url": "https://mcp.octavehq.com/mcp?ctx=<context>"
    }
  }
}
```

Use any name starting with `octave-`. Skills detect the Octave server from the available tools.

## What's included

- **Skills** (`/octave:research`, `/octave:library`, `/octave:generate`, `/octave:battlecard`, …) — the full upstream skill set, invoked the same way as in Claude Code.
- **Agents** (`octave-assistant`, `pmm-strategist`, `sdr-coach`, `revenue-strategist`) — Octave's specialist GTM personas.
- **Workflows** — multi-step GTM playbooks (account-based research, competitive deal prep, full outbound pipeline, …) run via `/octave:workflow`.
- **Commands** — one shortcut per workflow, so each playbook is also directly invocable as a command.

See the [upstream README](https://github.com/octavehq/lfgtm#skills) for full descriptions.
