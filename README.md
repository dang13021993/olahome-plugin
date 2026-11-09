# OlaHome

Public listings of homes in Japan for foreign residents. Use it to search listings, open one listing, and learn how to ask about a room on [olahome.jp](https://olahome.jp).

This package contains configuration only. It connects your assistant to the public MCP server at `https://olahome.jp/mcp` (Streamable HTTP, no sign-in, no API key). The server exposes 3 tools:

| Tool | What it does |
|---|---|
| `search_properties` | Search approved public OlaHome listings in Japan. Availability is not real-time. |
| `get_property_details` | Retrieve one approved public listing by its OlaHome public ID. |
| `get_service_information` | Describe OlaHome services and legal limitations; does not create a booking. |

The tools are read-only. They return public listings only and never book or reserve anything.

## Install

| Client | Command |
|---|---|
| Claude Code | `/plugin marketplace add dang13021993/olahome-plugin` then `/plugin install olahome@olahome` |
| Gemini CLI | `gemini extensions install https://github.com/dang13021993/olahome-plugin` |
| Qwen Code | `qwen extensions install dang13021993/olahome-plugin` |
| Kimi Code | `/plugins install https://github.com/dang13021993/olahome-plugin` |
| DeepSeek Harness | `dsh plugin --profile <profile> add github:dang13021993/olahome-plugin` |
| Any MCP client | Streamable HTTP URL `https://olahome.jp/mcp` |

## Example prompts

- "Find homes in Tokyo listed on OlaHome for a foreign resident."
- "Show me the details of this OlaHome listing."
- "What does OlaHome do, and can it reserve a room for me?"

## Contact

booking@olahome.jp · https://olahome.jp · License: MIT.
