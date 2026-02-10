# tides
Tides skill for AI agents, allows access to ocean tide model and predictions

## Features

- Fetch tide height for a given date/time and location
- Find tide extrema for a given time span at a specified location

The model features near global coverage (apart from poles). It is particularly
useful in locations that are not already well served by tide station networks.

## Installation

### Via ClawdHub

```bash
npx clawhub install tides
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

## Caveats and Warnings

Do not use for navigational purposes. This is for casual use. Always use official
tide tables for navigation or safety relevant activities.

This is based on the latest NOAA global tide modelling data and algorithms. For
most locations it is quite accurate, but in some shallow areas, estuaries, rivers
and lakes you may get unexpected results due to restricted water flows or
anomalous currents. You may find you can partially correct for these types of
location by using a fixed time offset.
