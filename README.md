<div align="center">

# Encoder Ai MCP

**MCP server for encoder ai mcp operations**

[![PyPI](https://img.shields.io/pypi/v/meok-encoder-ai-mcp)](https://pypi.org/project/meok-encoder-ai-mcp/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![MEOK AI Labs](https://img.shields.io/badge/MEOK_AI_Labs-MCP_Server-purple)](https://meok.ai)

</div>

## Overview

Encoder Ai MCP provides AI-powered tools via the Model Context Protocol (MCP).

## Tools

| Tool | Description |
|------|-------------|
| `encode_base64` | Encode text to Base64. |
| `decode_base64` | Decode Base64 to text. |
| `encode_url` | URL-encode a string. |
| `encode_html` | HTML-encode special characters. |
| `to_hex` | Convert text to hexadecimal. |

## Installation

```bash
pip install meok-encoder-ai-mcp
```

## Usage with Claude Desktop

Add to your Claude Desktop MCP config (`claude_desktop_config.json`):

```json
{
  "mcpServers": {
    "encoder-ai": {
      "command": "python",
      "args": ["-m", "meok_encoder_ai_mcp.server"]
    }
  }
}
```

## Usage with FastMCP

```python
from mcp.server.fastmcp import FastMCP

# This server exposes 5 tool(s) via MCP
# See server.py for full implementation
```

## License

MIT © [MEOK AI Labs](https://meok.ai)
