# tides
Tides skill for AI agents, allows access to ocean tide model and predictions

## Features

- Fetch tide height for a given date/time and location
- Find tide extrema for a given time span at a specified location

## Installation

### Via ClawdHub

```bash
clawdhub install evgyur/crypto-price
```

## Usage

### As a Skill

The skill is automatically triggered when users ask for tide information.

### Via MCP

This service is also available via MCP. Add the following to your
MCP definitions.

```
    "tides-mcp": {
      "command": "npx",
      "args": [
        "-y",
        "mcp-remote@latest",
        "https://hamandmore.net/api/harmonics/mcp"
      ]
    }

```
