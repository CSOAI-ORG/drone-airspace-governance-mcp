<div align="center">

# Drone Airspace Governance MCP

**MCP server for drone airspace governance mcp operations**

[![PyPI](https://img.shields.io/pypi/v/meok-drone-airspace-governance-mcp)](https://pypi.org/project/meok-drone-airspace-governance-mcp/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![MEOK AI Labs](https://img.shields.io/badge/MEOK_AI_Labs-MCP_Server-purple)](https://meok.ai)

</div>

## Overview

Drone Airspace Governance MCP provides AI-powered tools via the Model Context Protocol (MCP).

## Tools

| Tool | Description |
|------|-------------|
| `classify_operation` | Classify drone operation category per EASA/FAA regulations. |
| `bvlos_risk_assessment` | SORA 2.5 risk assessment for Beyond Visual Line of Sight operations. |
| `remote_id_compliance` | Check FAA Remote ID compliance for drone operations. |
| `autonomous_decision_governance` | Governance check for autonomous drone AI decisions (EU AI Act + aviation safety) |

## Installation

```bash
pip install meok-drone-airspace-governance-mcp
```

## Usage with Claude Desktop

Add to your Claude Desktop MCP config (`claude_desktop_config.json`):

```json
{
  "mcpServers": {
    "drone-airspace-governance": {
      "command": "python",
      "args": ["-m", "meok_drone_airspace_governance_mcp.server"]
    }
  }
}
```

## Usage with FastMCP

```python
from mcp.server.fastmcp import FastMCP

# This server exposes 4 tool(s) via MCP
# See server.py for full implementation
```

## License

MIT © [MEOK AI Labs](https://meok.ai)
